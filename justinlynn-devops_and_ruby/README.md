# DevOps and Ruby - A Match Made in vi *... :dw* emacs *... M-d* your editor.

In recent years we've seen many tools come and fight for centre stage in the arena of
'DevOps' - Chef, and of course, Puppet. Some are written in Ruby and some are not but this 
isn't just about Configuration Management. This talk explores many of the concepts and benefits
DevOps provides and surveys many tools and work flows which directly enable Ruby developers to
get more control and insight into how their applications are delivered in production.

## Outline

### Just what is 'DevOps'?

This section explores the question "What is 'DevOps' anyway and why should I care. Our 
ops guys won't stop going on about it and it sounds annoying. Why do they want to write code anyway?"

Specifically, it introduces the key concepts of DevOps, namely: the 
centralisation of visibility into changes, the decentralisation of operational control,
and the melding of Engineering and Operations into a cooperative unit that we call 'DevOps', 
which is also what the group practices.

### Infrastructure as Code, or, "It's 'pull requests' all the way down"

Here, we discuss the work flow which powers a 'typical' DevOps team and what 
'infrastructure as code' really means. This serves as a general template for the following
discussion on the implementation of said work flow.

### Every specification should have a reference implementation

This is where we discuss the work flow we laid out earlier is more detail, surveying many of the
available tools with which the presenter has had personal experience. The presenter is
a Ruby native and as such tools that are either natively written in Ruby, or which 
natively support ruby will be preferred. Of course, the presenter is polyglot and as such when tools that aren't written
in or which don't necessarily natively support Ruby are absolutely needed, they'll be mentioned and used. This section
will take up the majority of the presentation and will consist of a live demo walking users from bare metal
(actually, a set of VMs on the presenter's laptop) to a working, monitored, and instrumented installation of
an as of yet undecided infrastructure.

Explicitly, the areas of work flow to be surveyed include:

* Revision Control (Git)
* Release Engineering and Pulling from Upstreams (Git)
* Configuration Management (Chef)
* Software Deployment and Orchestration (Marionette Collective)
* Systems Monitoring (Nagios and/or Sensu)
* Metric Collection and Evaluation (Graphite)

### Time for Questions

Self explanatory.

## Justin 'J' Lynn

I design, create, and operate systems infrastructure and software delivery systems.
I drive productivity by providing tools and APIs that are stable, expertly engineered, and well-maintained.
I educate to eliminate single points of failure.
I listen to encourage convergence on the correct solution.
I test to ensure the solution is correct.
There are no unquestionable answers.
There are no unanswerable questions.

I'm from the San Francisco Bay Area where I've worked, professionally, for 4 years as a Systems Engineer.
I was born in California in the United States. I've known since the first time I used 
a computer that I wanted to dedicate my life to the study of these machines. Not just
the machines themselves but also to those who use them and of how
to better shift their burden to the machine.

![Profile picture](https://raw.github.com/rubyaustralia/rubyconfau-2013-cfp/master/justinlynn-devops_and_ruby/profile_picture.jpg)

- [My website](http://www.jaesharp.com/)
- [My blog](http://www.jaesharp.com/blog/)
- [My twitter](https://twitter.com/justinrwlynn)
- [An Example Talk - Hurry up And Wait: How I stopped worrying and learned to love the queue](http://www.youtube.com/watch?v=_lOW2MvBKRk)
