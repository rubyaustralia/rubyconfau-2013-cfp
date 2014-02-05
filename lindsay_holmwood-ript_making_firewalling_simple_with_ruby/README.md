# Ript: making firewalling simple with Ruby

For those of us still encumbered with running our own servers, firewalling is an important but dark art. UNIX hackers traditionally don't care about the UI of their programs, which means that 30 second firewall change you were going to make on a production system ends up taking an hour..

What we need is a simple abstraction that covers 90% of your firewalling needs.

Enter Ript, a clean and opinionated Domain Specific Language for describing firewall rules, that implements database migrations-like functionality for applying these rules with zero downtime.

At Ript's core is an easy to use Ruby DSL for describing both simple and complex sets of iptables firewall rules. After defining the hosts and networks you care about, Ript's DSL provides helpers for all the common use cases: accepting, dropping, & rejecting packets, as well as for performing DNAT and SNAT.

Here is an example ruleset definition:

``` ruby
# partitions/joeblogsco.rb
partition "joeblogsco" do
  label "www.joeblogsco.com", :address => "72.14.191.216"
  label "app-01", :address => "10.60.1.230"

  rewrite "public website + ssh access" do
    ports 80, 22
    dnat "www.joeblogsco.com" => "app-01"
  end
end
```

Ript provides a method to group common sets of rules together called "partitions", which are used at rule application time to perform zero-downtime migrations. This fosters a much more agile approach to firewall changes that limits the size and helps increase the frequency of changes - core principles behind Continuous Delivery.

Ript is designed from the ground up to be easy to use, and is extremely well tested end-to-end. Developed at [Bulletproof Networks](http://bulletproof.net/), it's been in use since 2012 in multi-tenanted firewall platforms as well as standalone systems running some very high profile sites.

In this talk Lindsay Holmwood will take you on a whirlwind tour of the DSL, explain how Ript utilises iptables features to work its magic, analyse testing complexities when writing systems code, and provide some concrete examples of how Ript can help increase the reliability of the services you deliver.

## My Name

Lindsay is sysadmin/developer/toolsmith/engineering manager, living in the New South Wales Blue Mountains.

He is the creator of cucumber-nagios (a tool that helps you describe how a system should work in natural language, and outputs whether it does in the Nagios plugin format), and Visage (a web service + interface for exposing collectd statistics).

Lindsay works at Bulletproof Networks running a distributed infrastructure development team that is strongly focused on testing & automation. He was responsible for keeping Movember up for the 2010 + 2011 + 2012 campaigns, and works on scaling both internal and customer facing systems.

He served as President of the Sydney Linux Users Group from 2006-2008, was on the organising committee of linux.conf.au 2007, and organised the inaugural DevOps Down Under in 2010, and again in 2011. He also organises the monthly Sydney DevOps meetups, and speaks at conferences both in Australia and abroad.


![Profile picture](https://raw.github.com/rubyaustralia/rubyconfau-2013-cfp/master/example/profile_picture.jpg)

- [My website](http://holmwood.id.au/~lindsay/)
- [My twitter](https://twitter.com/auxesis)
- [Past talk slides](http://www.slideshare.net/auxesis/load-testing-13067261)
- [Past talk video](http://www.youtube.com/watch?v=hpHml0QwDhg)
