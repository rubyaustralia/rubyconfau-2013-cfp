# `bundle install` Y U SO SLOW: Server Edition

If you've ever done anything in ruby, you've probably used rubygems and <rubygems.org> to search or install your favorite gem. On October 17, 2012, rubygems.org went down. A Dependency API was built to be used by Bundler 1.1+ to speed up `bundle install`. Unfortunately, it was a bit too popular and the service caused too much load on the current infrasture. In order to get rubygems.org back up the API had to be disabled. You can watch the [post-mortem](http://youtu.be/z73uiWKdJhw) for details.

Members in the community stepped up and built a compatible Dependency API service called the Bundler API. Working with the rubygems.org team, we were able to bring the API up for everyone within a week. In this talk, I will cover the process we went through of extracting the API out into a separate Sinatra app that now runs on Heroku. I'll go over how the API works and how Bundler itself uses it. Since we don't have direct access to their database, we needed to build a syncing service to keep our local cache up to date. We'll discuss the original sequential implementation of the sync code and how we improved performance through the use of a consumer thread pool. The sync time down was cut from 16 mins to 2-3 mins. Next, we'll talk about the productization steps we took for visibility to make sure the app is performing well.

We're prototyping a replay service, to replay production traffic to different Heroku apps. With this we can compare the performance between the current MRI app in production and the same app running on JRuby. This will also allow us to test any changes/features against real production load. We'll go over how to set this up.

## Terence Lee

Terence works at Heroku maintaining the Ruby stack and a slew of OSS projects such as Bundler and Resque, as well as helping with the Rails Girls movement. When he's not going to an awesome Heroku or Ruby event, he lives in Austin, TX, the taco capital of America.

(Terence loves Friday hugs, EVERY DAY OF THE WEEK! Give him a big one when you see him!)

![Profile picture](https://raw.github.com/rubyaustralia/rubyconfau-2013-cfp/master/terence_lee-rescuing_resque/profile_picture.jpg)

- [My website](http://hone.heroku.com)
- [My twitter](https://twitter.com/hone02)
- [Slides - Railsconf 2012](http://a-polyglot-heroku.herokuapp.com/)
- [Slides - Red Dot Rubyconf 2012](http://bundle-y-u-so-slow-rdrc2012.herokuapp.com/)
- [Slides - Boston.rb](http://rails-3-1-on-heroku.herokuapp.com/)
- [Speakerdeck](https://speakerdeck.com/hone)
- [Video - Boston.rb](http://bostonrb.org/presentations/heroku-and-rails-31)
- [Video - EuRuKo 2012](http://vimeo.com/44028326)
- [Video - Sapporo Ruby Kaigi 2012](http://www.ustream.tv/recorded/25443102)
