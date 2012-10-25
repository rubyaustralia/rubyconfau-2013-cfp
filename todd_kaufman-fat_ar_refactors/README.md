# Lean and Mean Domain Objects in Active Record

Rails apps that have been extensively enhanced and maintained over the last few years are starting to fall apart under their own weight.
Developers have struggled trying to find the most appropriate area to place logic within the system. Initially the ease of writing views
in ERB led many developers to stow code at the front of the application. Then we began finding the views to difficult to maintain so we
moved the logic into controllers or helpers. Eventually this also became difficult to maintain so we developed "best practices" like
skinny controllers and fat models. Active Record domain models naturally become the dumping ground of logic within the system but sooner
or later this leads to brittle systems.

Coupling persistence, validation, advanced querying, and business logic all into the same class inevitably leads to extremely fat models
with any system of significance. Skinny controllers are definitely worth striving for, but shoveling all of the business logic into a
class that is already overburdened with persistence, querying, and validation is a recipe for disaster. When you find yourself using
factories, fixtures, or mocks to construct 8 different class dependencies, it's time to admit that fat models are not a solution worth
aspiring to.

This talk will cover some different approaches for segregating the multiple concerns of fat Active Record models into loosely coupled,
cohesive classes with single responsibilities. We'll dive into the both the process for refactoring these plump classes along with
some better patterns of use for common AR bloat.


## Todd Kaufman

Todd Kaufman has developed, coached, and managed software development teams in Java, Ruby and .NET. Regardless of platform, he is
passionate about finding better ways to build systems with low ceremony and high quality. He has been known to occasionally run long
distances and drink scotch, although not necessarily at the same time. Todd delivers outstanding software to his clients through
Test Double, a software studio in Columbus, Ohio.


![Profile picture](https://raw.github.com/rubyaustralia/rubyconfau-2013-cfp/master/todd_kaufman-fat_ar_refactor/profile_picture.jpg)

- [My website](http://testdouble.com)
- [My twitter](https://twitter.com/toddkaufman)
- [Past talk slides](https://speakerdeck.com/toddkaufman)
