# Fact-based programming using the ActiveFacts API

We talk about real situations using facts about things. So why do we allow
object-orientation to force us to divide things into objects and attributes?
The same happens when we design relational databases, except worse, especially
if we're using Active Record.

Although Ruby uses objects for attribute values, many values have their own
behaviours. These behaviours should not be forced into owner objects.
Meaningless object identifiers and surrogate DB keys (isolated from attribute
values) also create data quality problems like data duplication and
contradiction.

This talk shows how a fact-based approach to programming can avoid these
problems.  Unlike an object, a fact cannot be duplicated, just re-asserted -
it's still the same fact.  The constellation data structure implemented by
the activefacts-api (gem) provides a radical new approach to data semantics
and program function, and is the core of a new database definition and query
language (CQL) and a new O/RM (under development).

## Clifford Heath

Clifford has been a software designer and toolmaker for three decades, having
been inventor and architect of multiple major software products that have brought
over a hundred million dollars into Australia.  He was also one of the first
locals to make the switch to Ruby, and his gem downloads outnumber any other
Australian author. His work in semantic (fact-based) modelling holds enormous
promise for a renewal of trust in the IT industry by its clients.

![Profile picture](https://raw.github.com/cjheath/rubyconfau-2013-cfp/master/clifford_heath-fact-based-programming/profile_picture_640x480.jpg)

- [My website](http://dataconstellation.com)
- [My twitter](https://twitter.com/cliffordheath)
- [Past talk slides](http://dataconstellation.com/ActiveFacts/CQL%20Slides%202009.pdf)
- [Past talk video](http://dataconstellation.com/screencasts/CQL.shtml)
