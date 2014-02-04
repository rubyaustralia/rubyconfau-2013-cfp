# It's not how good your app is, it's how good you want it to be

This talk is part story, part code, and part mustache.

Travis CI is a distributed continuous integration system running over 7,000 tests daily. For us to get a true insight into what is going on behind the scenes we have had to come a long way by integrating and building both tools and libraries so that Travis and its many parts are not just a black box of information.

Reading logs and using NewRelic is not new, but far from enough, especially when it comes to apps which are composed of many smaller apps, like Travis. How do you track and visualize requests being processed by multiple services? How do you silence verbose logs while not losing the core of the message? And how do you aggregate, visualize and share metrics?

A lot of how we track, manage, and visualize what is going on in Travis has been created as a set of internal tools and by using a range of awesome services, but core to a lot of this is ActiveSupport Notifications and Travis Instrumentation.

This session will give insight to how Travis is composed and connected, as well as shedding light on how simple it can be to gain more visibility into even a complex, distributed system like Travis, as well as your applications too.

## Josh Kalderimis

Josh is a traveling coding nomad. Working as a foreman at Travis CI, an open source continuous integration service, he spends his days taming the beast which is VirtualBox while fixing all the builds!

In the past he used to be a top 30 Ruby on Rails contributor, but has since been surpassed and left to wallow in the top 40. Instead he now tests code by hand, while sending personalized emails and Campfire notifications when a build breaks.


![Profile picture](https://raw.github.com/joshk/rubyconfau-2013-cfp/master/josh_kalderimis-its_not_how_good_your_app_is_its_how_good_you_want_it_to_be/profile_picture.jpg)

- [My website](http://travis-ci.org)
- [My twitter](https://twitter.com/j2h)
- [Past talk slides](http://speakerdeck.com/u/joshk)
- [RailsConf](http://www.youtube.com/watch?v=huFeH5BRhUo), [Railsberry](http://www.youtube.com/watch?v=F8Hq6ga7vH8) & [RubyShift](http://www.youtube.com/watch?v=XvuNNxSJUpQ)
