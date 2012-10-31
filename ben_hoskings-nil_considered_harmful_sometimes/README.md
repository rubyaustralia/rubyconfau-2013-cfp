# nil considered harmful (sometimes)

It's frustrating to work on a flaky codebase. Ruby is a permissive language -- it gives you the tools to program as brilliantly or as awfully as you want to.

It's my view that one of ruby's most misused components is nil. By leaning heavily on ruby's functional side and avoiding nil (and judiciously unit testing), you can write maintainable code that fails fast, and fails in the right direction.

I'll make the case for eschewing nil and talk through some examples. I'll go into the parallels on the database side, too: how you can design your schema to avoid NULL and map it cleanly to simple, reliable ruby.


## Ben Hoskings

Ben is from Brisbane but these days hails from Melbourne, where he works for The Conversation, a not-for-profit that publishes academia's take on the news of the day. In tech, Ben loves unix, git, postgres and of course the rubies.

![Profile picture](https://raw.github.com/rubyaustralia/rubyconfau-2013-cfp/master/ben_hoskings-nil_considered_harmful_sometimes/profile_picture.jpg)

- [Ben's website](http://benhoskin.gs)
- [Ben on twitter](https://twitter.com/ben_h)
