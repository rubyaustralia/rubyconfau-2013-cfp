# Down the rb_newobj() Rabbit Hole: Garbage Collection in Ruby

New Relic recently made the big move to Ruby 1.9.3 which showed meaningful
improvements over 1.8, particularly in garbage collection. So this talk is 
taking a look at what changed in Ruby's garbage collection that caused much 
of the improvements. We will start with the fundamentals of garbage collection 
but work down to the nitty gritty C code to get to the details of what's going 
on, starting with rb_newobj(). You should walk away with an understanding of how
garbage collection works in MRI and a nice appreciation for the overall
lifecycle of Ruby objects.

## Chris Kelly

Chris Kelly is a Developer and Evangelist at New Relic. He is a self-identified
happiness engineer, writing code that makes someone else's day better. He's
blogged, talked, or written code on everything from Ruby and Rails, to front-end
best practices and DevOps. He spends a lot of time thinking about how our tools
and processes effect our teams and our code, you may have seen him on a soap box
recently at OSCON, QCon, or PuppetConf.

![Profile picture](https://raw.github.com/rubyaustralia/rubyconfau-2013-cfp/master/example/profile_picture.jpg)

- [My website](http://amateurhuman.com)
- [My twitter](https://twitter.com/amateurhuman)
- [Past talk slides](http://speakerdeck.com/amateurhuman)
