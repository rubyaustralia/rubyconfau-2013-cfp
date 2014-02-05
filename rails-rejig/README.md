# Rails Rejig

This talk is about distributing a Rails Application. No! Not the traditional cluster setup with load balancers and multi-node deployment - its actually chopping up ONE Rails application into several pieces and distributing them separately on different nodes to achieve greater performance and availability.

What the .... !!!

A typical Rails application has various intelligent modules that I call **gigs**. Examples of gigs are the login module, search module, social share module, report-generation module, logs management and any other module you can think of! Each gig has a different type of importance - the search needs to large memory and high CPU, the login module needs a standard setup with moderate memory and CPU, the logs module needs less memory but more disk space. 

Using Rails-Rejig we can distribute these gigs across different nodes! In other words **'rejig the Rails application'**. This results in a highly available system, with the right gigs receiving the right resources.

Among other things, this talk contains a lot of information about rack-rewrite and digs deep into the Ruby part of Rails - not for the weak-hearted! ;) The demo involves the audience who can use their machine as **'gigsters'** (gig hosters) and we can see the availability and performance of a web application!

## Gautam Rege

Gautam is a Rubyist by profession and entrepreneur by choice. He is the co-founder of [Josh Software](http://www.joshsoftware.com), one of the earliest companies in India to embrace Ruby On Rails. He is the author of [Ruby and MongoDB Web Development Guide](http://packtpub.com/ruby-and-mongodb-web-development-beginners-guide/book). He loves to talk, write and has spoken at several Ruby Conferences around the world. He is on the core team that organizes Ruby Conf India every year.

![Profile picture](https://raw.github.com/gautamrege/rubyconfau-2013-cfp/master/rails-rejig/profile_picture.jpg)

- [My website](http://www.joshsoftware.com)
- [My blog](http://blog.joshsoftware.com)
- [@gautamrege](https://twitter.com/gautamrege)

### My Talks and Videos

- [Ruby Conf India - India, 2012 (video)](http://www.youtube.com/watch?v=HDvk9PZx2t8&list=PL50D7368F56665FAE&index=10&feature=plpp_video)
- [Outsourcing Redefined, Singapore, 2011 (slides)](http://outsourcing-rails-reddot.heroku.com)
- [SPlat, Austin, 2010 (slides)](http://josh-splat.heroku.com)
- [Silicon India - WebApps, India, 2011 (slide)](http://webapps2011-ror.heroku.com/)
- [Mirah, GNUify, 2011 (slides)](http://gnuify12-mirah.herokuapp.com)


