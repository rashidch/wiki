---
layout: post
title: "Introducing Popolo, an open government data standard"
type: article
author: James McKinney
permalink: 2013/02/21/update-on-opengovernment.html
---
Last November, we wrote about [our partnership](http://blog.opennorth.ca/2012/11/30/this-week-in-open-government/) with the [Participatory Politics Foundation](http://www.participatorypolitics.org/) (PPF) to lead the development and expansion of their [OpenGovernment.org](http://opengovernment.org/) project to three US cities.

As part of our work on OpenGovernment.org, we have researched, re-used and contributed to a number of open source, open government projects, including [mySociety](http://www.mysociety.org/)’s [PopIt](http://popit.mysociety.org/), a service for building a database of people, organizations and positions, and the [Sunlight Foundation](http://sunlightfoundation.com/)’s [Billy](https://github.com/sunlightlabs/billy), a framework for scraping, storing and sharing government data. A major barrier to increased re-use of these great open-source civic tools is the lack of agreement on how to name things. To give a very simple example: if one project calls a person’s name `name` and another calls it `full_name`, then if you want to write a project that builds on what mySociety and Sunlight have done, you need to write an adapter for each, which increases the overhead, complexity and maintenance costs of your project. Wouldn’t it be better if we all committed to a standard way of naming things, to maximize interoperability and make re-use that much easier?

To address this problem, we’ve published a working draft of **[Popolo](http://popoloproject.com/), an open government data standard**. In its first draft, Popolo is *deliberately unambitious*. It proposes a standard naming scheme for the basic pieces of any government monitoring website: people, organizations and the relationships between the two. The idea is that if the groups working on open source, open government tools can agree on a data standard for these basic pieces, then we can expand the project to cover things like bills, agendas and minutes, which have much less in common across jurisdictions and on which it is much harder to find agreement.

The ultimate goal of the project is to make it easier and quicker for civic developers to create government transparency and civic engagement websites, by offering them re-usable, well-documented open-source code. We want developers to be able to focus on what's special about the governments they want to monitor, not on re-implementing features commonly found in open government websites. For example, we plan on reusing the Popolo standard ourselves to build [MyCityHall.ca and MaMairie.ca](http://blog.opennorth.ca/2013/02/19/introducing-mycityhall/) sites in several Canadian cities. 

This project is in line with (and inspired by) Tom Steinberg of mySociety’s proposals for a [component strategy](http://www.mysociety.org/2012/07/04/mysocietys-components-strategy-our-take-on-small-pieces-loosely-joined/) last July, in which he wrote, "The Components will talk to each other, and to the rest of the web using simple open schemas which will evolve as they are built. Where possible we’ll pick up popular data standards and re-use those, rather than building anything ourselves." Indeed, Popolo re-uses at least *nine* existing standards.

We have begun reaching out to other groups to make Popolo a truly community-driven standard, and we hope to move out of draft into version 1.0 in time for [Transparency Camp](http://transparencycamp.org/). We’ve already got early feedback on our [News Challenge idea](https://www.newschallenge.org/open/open-government/inspiration/make-government-monitoring-projects-easier-to-re-use) about better data standards. Popolo’s documentation is licensed under Creative Commons and is managed on [GitHub](https://github.com/opennorth/popolo-standard/tree/gh-pages). For the Ruby on Rails enthusiasts out there, there is an implementation of the Popolo standard as a [Ruby on Rails engine](https://github.com/opennorth/popolo) on GitHub as well, for you to re-use in your projects.

If you’re heading to SxSW, come find Open North’s [James McKinney](https://twitter.com/@mckinneyjames) and PPF’s [David Moore](https://twitter.com/ppolitics) for an alpha preview of the next version of OpenGovernment.org at SxSW Interactive from March 8th-12th!

*Check out PPF’s corresponding announcement on [their blog](http://blog.opengovernment.org/2013/02/20/introducing-the-popolo-standard/).*