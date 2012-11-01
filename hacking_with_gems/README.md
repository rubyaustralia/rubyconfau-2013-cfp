# Hacking with Gems

## Summary

What's the worst that could happen if your app has a dependency on a malicious gem? How easy would it be to write a gem that could compromise a box?

Much of the Ruby community blindly trusts our gems. This talk will make you second guess that trust. It will also show you how to vet gems that you do choose to use.

## Notes

There are four malicious gems I will be presenting:

- Harvesting passwords from requests going through a Rails app
- Exposing the contents of a Rails app's database
- Compromising the source code of a Rails app
- Providing SSH access to a box a 'gem install' time and stealing gem cutter credentials (and going viral)

My talk will increase awareness that these sort of gems can exist in the wild, show how easy it is for anyone to build malicious gems, and give easy techniques for identifying these gems.

At Aloha Ruby Conf I also wrote a "malicious" gem and social engineered people into installing it by distributing business cards with some info on the gem printed on them. It collected usernames from attendees who installed it, and I showed them on a side of my talk. Proving that if I had actually wanted to, I could have hacked their boxes.

## Benjamin Smith

Benjamin Smith is a developer at Pivotal Labs. He has a strong passion for TDD, pairing, Agile and using technologies that get out of the programmer's way. When not writing code, he follows his other passions into the outdoors to rock climb, back country snowboard, kayak and surf.

![Profile picture](https://raw.github.com/benjaminleesmith/rubyconfau-2013-cfp/master/hacking_with_gems/profile_picture.jpg)
- [My website](http://pivotallabs.com/users/bsmith/blog)
- [My twitter](https://twitter.com/benjamin_smith)
- [Past talk slides](https://speakerdeck.com/u/benjaminleesmith/p/hacking-with-gems)
- [Past talk video](http://www.confreaks.com/videos/1243-aloharuby2012-hacking-with-gems)
