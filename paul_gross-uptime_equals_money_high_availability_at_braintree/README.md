# Uptime == Money: High Availability at Braintree

Braintree is a payment gateway, so downtime directly costs both us and our
merchants money. Therefore, high availability is extremely important at Braintree. This talk
will cover how we do HA at Braintree on our Ruby on Rails application.

Specific topics will include:

* Working around planned downtime and deploys:
 * How we pause traffic for short periods of time without failing requests
 * How we fit our maintenance into these short pauses
 * How we do rolling deploys and schema changes without downtime

* Working around unplanned failures:
 * How we load balance across redundant services
 * How the app is structured to retry requests

## Paul Gross

Paul Gross is a developer working at [Braintree](https://www.braintreepayments.com/). Braintree helps businesses accept credit card payments online with great development tools and first class support. Paul has worked on everything at Braintree from their highly available infrastructure to the client libraries that ease integration in seven languages. Before Braintree, Paul worked at [ThoughtWorks](http://www.thoughtworks.com/), a global consultancy, building custom software in many languages, including Java, .NET, Python and Ruby. Paul has worked in software development and delivery for over 10 years. 

![Profile picture](https://secure.gravatar.com/avatar/a6cbdd6473de1af38ef1d8e01588ae7e?s=200)

- [My website](http://www.pgrs.net)
- [My twitter](https://twitter.com/pgr0ss)

I have not done this talk before, but it will incorporate pieces from my talk at PgEast ([Migrating from MySQL to PostgreSQL](https://www.pgrs.net/wp-content/uploads/2011/03/pgeast_presentation.pdf)) and the following blog posts:

- [Scaling PostgreSQL at Braintree: Four Years of Evolution](https://www.braintreepayments.com/braintrust/scaling-postgresql-at-braintree-four-years-of-evolution)
- [How We Moved Our Data Center 25 Miles Without Downtime](https://www.braintreepayments.com/braintrust/switching-datacenters)
