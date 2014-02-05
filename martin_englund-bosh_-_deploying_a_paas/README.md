# BOSH - deploying a PaaS

What does it take to release, deploy and manage a really big Ruby application?

In the beginning of your application's life things are easy - you can use puppet or chef to automate your environment, or you can deploy your application using a PaaS provider, but what happens when your application becomes the next facebook or twitter?

This presentation will show you how VMware operates its [Cloud Foundry](http://cloudfoundry.com/) PaaS using a tool called BOSH, which handles:
- release management
- deployment
- scaling (horizontally & vertically)
- life cycle management

The Cloud Foundry PaaS is a large distributed application written mainly in Ruby, and consists of several hundred virtual machines from over 40 different types of virtual machines classes, all managed from one tool.

BOSH itself is an [open source](https://github.com/cloudfoundry/bosh) Ruby application developed by VMware.

## Martin Englund

Martin is a Staff Engineer at VMware, with over 20 years of experience in large scale datacenter operations, now working on the Cloud Foundry PaaS.

Specifically, Martin works on orchestration tool for Cloud Foundry, called BOSH, which provides end-to-end automation for cloudfoundry.com.

Before joining VMware Martin worked at Sun Microsystems, where he operated the external web sites, like www.sun.com & java.sun.com, using Puppet.

He is a security geek at heart, is passionate about operations automation, and has the firm belief that if you are doing it by hand you are doing it wrong. He has been a contributor to a number of open source projects such as OpenSolaris & Puppet.

![Profile picture](https://raw.github.com/pmenglund/rubyconfau-2013-cfp/master/martin_englund-bosh_-_deploying_a_paas/profile_picture.png)

- [Blog](http://blog.codenursery.com)
- [Twitter](https://twitter.com/pmenglund)
- Past talk slides: [PuppetConf](http://www.slideshare.net/PuppetLabs/martin-puppetconf) [RubyConfBR](http://www.eventials.com/presentation/download/M2UzZTJkMzY2MzdiNTg2NTUxNWM1MzI3NWY1YjRhMzYjIzEyOTE_3D)
- Past talk video: [PuppetConf](http://www.youtube.com/watch?v=14Q0JFEzWXQ) [RubyConfBR](http://www.eventials.com/rubyconfbr2012/recorded/M2UzZTJkMzY2MzdiNTg2NTUxNWM1MzI3NWY1YjRhMzYjIzEyOTE_3D)
