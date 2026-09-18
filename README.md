# Proposed Nordic-RSE planet

This is a static-site based, Github-pages deployable "planet" - an
old-style aggregator and viewer of RSS feeds.  It provides a way for
people to share blogs among a community without relying on centralized
social media platforms.  There is the HTML view (for people to browse
and see if it's interesting) and an Atom feed for people to subscribe
to in their own readers.

You can see an example planet at https://planet.debian.org/

The code behind this is https://github.com/rkdarst/pyplanet2

## Everything below is my proposal, please suggest changes

I am making this for Nordic-RSE.  If accepted this readme will be
updated.  I propose that this be put somewhere like
planet.nordic-rse.org (or planet.coderefinery.org if we want to make
it broader) and we add feeds from, for example:

## What can be included

* Blogs of individuals within the community (loosely defined)
* Blogs of organizations within the community (a bit more strictly
  defined)
* Possibly news feeds of organizations within the community, but a
  preference to human-written blog format things, rather than basic
  news stories and press releases.  These can be added but removed if
  they begin dominating too much or are not blog-like enough.

## Content policy

You are allowed and encouraged to post about things not related to
work, including your own hacking, learning, opinions, and hobbies.
(Work stuff is also allowed and encouraged, obviously).  The purpose
of a planet is to build community, not just advertise work stuff that
are mainly communicated through other channels.  If desired, separate
work-only or news-post-only feeds may be added.

Content should be by humans and for humans.  Using content generators
is not explicitly forbidden, but they should not reduce the amount of
work you need to do to create and develop an idea (so at least
proofreading, translation, and so on is OK).  Content shouldn't be
misinformaiton, clickbait, sensationalist, hateful, and so on
(it should follow the Code of Conduct).

It's recommend to use good writing styles so that someone reading only
the first paragraphs can get a good overview of what the post is
about.  This allows people to quickly scan the planet for posts
interesting to them.

The HTML view has images cached.  Feeds, sites, and posts linked
should not have dark patterns with respect to privacy or web security.

## Adding feeds

Feeds are added via editing the config.yaml file, which should be
self-explanatory.

Possible issues:

* I've noticed some feeds have different semantics for how image links
  are resolved, so the `resolve_urls` setting may need adjusting.  Let
  rkdarst know if you see this (until it is known enough to be fully
  documented).
