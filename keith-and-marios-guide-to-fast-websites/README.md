# Keith and Mario's Guide to Fast Websites

When you talk to most people about Rails performance the conversation usually
turns to concurrency. How can my Rails app handle 60 simultanious requests per
second? How do I webscale?

Although the topic of concurrency is important, we won't be focusing on that
during this talk. We want to focus on end user speed.

For every extra second your application takes to load your conversion rates
will drop by an average of 7%. While most people start tweaking their backends
to squeeze every extra ms in response time, more often than not (80-90%) of the
_actual_ time spent loading your application is on the front end and the network stack.
This is where you should start.

We will cover a range of techniques and provide benchmarks along
the way to show how much performance you can expect from each step along the
way. We'll also cover *some* backend performance tuning as well.

Here's some of the topics we'll cover:

  - How to accurately benchmark performance
  - Asyncronously loading assets
  - Reducing requests per page
  - Rails http streaming (chunked responses)
  - Basic caching
  - What is SPDY - and how to use it
  - What CDN is right for your app?
  - Server location and why it matters

## Mario Visic

Mario is a Ruby on Rails developer from Perth Australia, currently working at Envato in Melbourne. As well as being a Co-Founder of [Desktoppr](https://www.desktoppr.co) he has also worked on some cool projects such as [iMeducate](https://www.imeducate.com) and [Airtasker](https://www.airtasker.com)

He also loves eating assorted types of cheeses.

![Profile picture](https://raw.github.com/mariovisic/rubyconfau-2013-cfp/master/keith-and-marios-guide-to-fast-websites/profile_picture_mario.jpg)

- [Website](http://www.mariovisic.com)
- [Twitter](https://twitter.com/mariovisic)
- [GitHub](https://github.com/mariovisic)
- [Past talk slides - Declarative Cucumber at Sydney roro](http://mariovisic.github.com/declarative_cucumber/)

## Keith Pitt

Keith, previously a Ruby on Rails Developer, now spends his time on the front end of things - working heavily with Javascript and CSS.
Originally from Adelaide, he currently works for Envato in Melbourne. He is the other Co-Founder of [Desktoppr](https://www.desktoppr.co).

In Keith's spare time, he watches many scary movies, and wins Magic Competitons.

He has been involoved with Rails Camp Australia, as well as being on the organisation comittee for the Adelaide Rails Camp 2011.

![Profile picture](https://raw.github.com/mariovisic/rubyconfau-2013-cfp/master/keith-and-marios-guide-to-fast-websites/profile_picture_keith.jpg)

- [Website](http://keithpitt.com/)
- [Twitter](https://twitter.com/keithpitt)
- [GitHub](https://github.com/keithpitt)
- [Past Talk Slides - UI Testin with Frank](http://slidesha.re/SuMD4p)
- [Past Talk Video - VendorKit at Cocoaheads Melbourne](http://www.melbournecocoaheads.com/vendorkit-keith-pitt/)
