# From Fat Views in ERB to Fly Views in Backbone

Users expectations on the interactivity, speed, and design of websites are steadily increasing. As these demands have increased,
have we as developers been able to keep our focus on the maintainability of the overall solution? Has our rails application
maintained it's well defined lines between Model View and Controller or have we occasionally let some <%= domain_logic.seep %> into the
view in the form of ERB? Have we maintained SOLID principles of all portions of our application or have we shuttled off functional nuggets
of wisdom into obscure helper methods never to be seen or reused again? Have we truly achieved the principle of DRY across all of our models,
views, and controllers or have we fooled ourselves into thinking that we have reuse by breaking down the view into partials which
cannot exist independent of one another? Do we really leverage a test first approach to drive a better design for our views or
do we just slap a fresh coat of Cucumber on the problem to make sure that we feel there's a 50/50 chance that our application
behaves the way we think it should?

As mature Rails applications are entering their third, fourth, or fifth year of maintenance, we are starting to see the need for a
more mature, well factored solution to delivering rich client experiences. Backbone is one of many javascript frameworks that is
currently looking to fill this void, but our solution should not be to just always start re-writing the application whenever we
feel it is starting to fall over from it's own weight!

This session will walkthrough some approaches for migrating an existing, legacy Rails view into a more maintainable, well factored
Backbone solution that still leverages a Rails backend and API. We'll cover the approach from soup to nuts showing how to
progressively refactor the untested ERBs, helper methods, javascript files, and other spaghetti into a well tested and easily maintained
Coffeescript fueled Backbone view.

## Todd Kaufman

Todd Kaufman has developed, coached, and managed software development teams in Java, Ruby and .NET. Regardless of platform, he is
passionate about finding better ways to build systems with low ceremony and high quality. He has been known to occasionally run long
distances and drink scotch, although not necessarily at the same time. Todd delivers outstanding software to his clients through
Test Double, a software studio in Columbus, Ohio.


![Profile picture](https://github.com/tkaufman/rubyconfau-2013-cfp/blob/master/todd_kaufman-erb_to_backbone/profile_picture.jpg)

- [My website](http://testdouble.com)
- [My twitter](https://twitter.com/toddkaufman)
- [Past talk slides](https://speakerdeck.com/toddkaufman)
