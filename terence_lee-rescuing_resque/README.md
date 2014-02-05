# Rescuing Resque

Resque has been plagued by issues over the past half a year due to inactivity on the project. For instance, resque doesn't handle the cleaning up workers on distributed systems like Heroku. This issue (#319) has been open for over a year. redis.rb 3.0.0 came out on May 23rd which brings improved performance and backward incompatible changes. Also due to this inactivity, other queueing libraries like Sidekiq have come up to fill the void with new features.

We'll use my story of taking over Resque as a case example for maintaining an Open Source project. I made a lot of mistakes along the way that you can hopefully avoid. Some examples include balancing pushing forward with new features and maintaining the latest stable release or getting comfortable with the prior design decisions. I'll cover how we rallied the community and built a team.

As the Ruby community embraces threads with Rails 4, we'll talk about concurrency in Ruby, concurrent data structures, and how we use them in the Resque 2 to build a better queueing library. Finally, I'll close with what the current state of Resque is and what our plans going forward.

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
