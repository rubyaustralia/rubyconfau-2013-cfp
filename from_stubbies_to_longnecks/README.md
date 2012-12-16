# From Stubbies to Longnecks - Finding and curing scaling bottlenecks

Every application is different. Every application performs and scales in
a different manner. What stays the same are the tools we use to monitor
and diagnose our applications when they get sick or have a big night
out.

In this talk I'll cover how realestate.com.au monitors and troubleshoots
the performance and scalability of our Ruby and non-Ruby apps. I'll look
at the tools we use to infer when/where things go wrong and several
cases where things *have* gone wrong and how we've dug our way out of
the whole.

Examples of areas covered include:

- Vertical scaling our way out of I/O pain
- Horizontal scaling our apps for throughput and availability
- Using HTTP and CDNs to avoid the reddit-effect
- Tools we use for establishing performance 'baselines'

## Geoffrey Giesemann

Geoffrey is a Technical Lead at realestate.com.au.  When he isn't
wailing away on a keyboard punching out Ruby he daydreams about making
teams operationally excellent with liberal doses of DevOps and building
a cape that will make him nerf-proof.

![Profile picture](https://raw.github.com/geoffwa/rubyconfau-2013-cfp/from_stubbies_to_longnecks/from_stubbies_to_longnecks/profile_picture.jpg)

- [My twitter](https://twitter.com/ggiesemann)
- [Past talk slides](http://www.slideshare.net/ggiesemann)
