# Ember on Rails — Building desktop-class web applications on Rails

The web technology landscape is constantly changing, and as Rubyists we have a constant supply of new toys to play with. Some of these toys help us write better code or make our lives easier, and others implement entirely new ways of doing things. Regardless, nearly all of them aim to make things faster.

One area where things have traditionally been slow is pushing state changes to the browser in the typical `request => response` pattern. The likes of 37Signals have tried to speed this up using Ajax and `Turbolinks`, but the fundamental design has remained the same: We're still generating HTML on a server and sending down a wire to a browser.

In order to build desktop-class responsiveness we need to take the leap to generating HTML client side, in the browser. This is what Ember.js excels at.

My talk will cover:

- Overview of Ember as a framework
- Getting Rails setup to use Ember
- Strategies for using Ember with Rails
- Sending data to and from Ember
- Handling authentication and other challenges
- Lots of code

## Ivan Vanderbyl

Ivan is the founder and lead developer of [CrashLog.io](http://crashlog.io) which is built entirely in Ember.js and Rails with
full client side rendering.

Ivan has been working with Ruby for nearly 10 years and is constantly exploring better ways of doing things,
and better ways to build software on the web.

![Profile picture](https://twimg0-a.akamaihd.net/profile_images/1280754055/100415_0005_small.jpg)

- [Blog](http://crashlog.io/blog)
- [Twitter](https://twitter.com/ivanvanderbyl)
- Some past slides:
  - [Building the OrionVM API: Video](http://vimeo.com/49304831)
  - [Building the OrionVM API: Slides](https://speakerdeck.com/ivanvanderbyl/building-the-orionvm-api-with-grape)

