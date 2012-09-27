# How Rails Scales:

[Zendesk](http://www.zendesk.com/) is among the largest RoR SaaS application currently running. It is currently ranked in the [top 800 sites worldwide](http://www.alexa.com/siteinfo/zendesk.com) and is in the top 400 sites in Australia.

3 years ago Zendesk was a site handling 3,000 RPM (50 queries per second) on some fully managed VMs. This talk will explain how Zendesk scaled to become a site that now handles over 60,000 RPM (1000 real application queries per second), running on dedicated hardware at multiple data centers. However our response time is unchanged at less than 150 milliseconds per request.

This talk will cover many of the issues that Zendesk encountered while scaling with a focus on pragmatic solutions to the real problems we faced. 

### The topics that will be covered:

* Scaling: What we had to watch out for and what we dealt with first
* Architecture: KISS. An overview of simple things that have worked really well for us and some that have not worked quite so well.
* Sharding MySQL. The approach we took, the tradeoffs it entailed.
* Caching with Memcache: Coherency and failure. It's the details that matter here.
* Reliability: What were our single points of failure and how we addressed them
* Performance: Where we found the biggest gains.

Expect this talk to be heavy on specifics and technical detail.

## Tim Sturge

I'm the Director of Infrastructure at Zendesk. I manage the teams responsible for backend engineering (including ruby library development, search, chat, analytics, sharding) and also previously managed the operations and DBA groups. I'm also the public face of Zendesk's [uptime](http://www.zendesk.com/support/system-status)

I grew up in New Zealand but have been working in Silicon Valley and San Francisco for 15 years. My focus has been on the development of extremely high volume internet applications, including My Yahoo!, Yahoo Mail, Google AdWords and now Zendesk.

![Profile picture](https://raw.github.com/tsturge/rubyconfau-2013-cfp/master/how-rails-scales/profile_picture.jpg)

The genesis of this talk is a [panel discussion](http://blog.newrelic.com/2012/07/02/more-on-managing-real-world-rails-apps-at-massive-scale-an-interview-with-tim-sturge-director-of-engineering-at-zendesk/)  [(video with controls)](http://blog.newrelic.com/2012/06/27/more-on-managing-real-world-rails-apps-at-massive-scale-an-interview-with-pitr-vernigorov-senior-architect-of-uken-games/) given at RailsConf in Austin Texas early in 2012. This discussion was well received and I realized as a result that there is desire in the Rails community to know more about how larger sites work.

- [LinkedIn](http://www.linkedin.com/pub/tim-sturge/0/a2/409)



