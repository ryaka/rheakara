+++
date = "2016-09-15T17:05:15-07:00"
hero = "/img/hello-world.jpg"
title = "Hello World"
description = "A post on how this blog came to be."
tags = []
categories = ["general", "technology"]
+++

For some background, I was previously using Squarespace to host an equivalent
personal site. It started with the very good intentions of making (semi-)regular
blog posts on whatever caught my interests and to also have a place serving as
a portfolio / contact. Squarespace at the time fit the needs of my unjustified urgency
to have something up and running, and just like that, I was a member.

Ignoring the fact that I barely, if at all, used the site, there were two major
points that bothered me greatly. In particular:

* Paying $16/month for a very low traffic website
* Not having reliable backup

After some recent circumstantial changes, I finally found myself with much more
time and decided to finally move off of Squarespace. I eventually settled on [Hugo](https://gohugo.io/) after some research as a nice solution to these problems.

## Paying $0/month for a (insert here) traffic website

Initially I considered moving over to [AWS S3](http://docs.aws.amazon.com/AmazonS3/latest/dev/WebsiteHosting.html)
as it is a familiar part of my
recent past, present, and (likely) near future. However what steered me away from
this was the discovery of [Github Pages](https://pages.github.com/) which offers
free static website hosting. Thankfully I [RTFM'd](https://en.wikipedia.org/wiki/RTFM)
as spending time on [Hugo's docs] (https://gohugo.io/tutorials/github-pages-blog/)
quickly pointed me in the direction of this hosting option.

In contrast to AWS S3, Github Pages offers free hosting for static websites. Given
that I don't expect things to be very high traffic, it at most it saves me literally
"pennies" vs AWS S3 as I estimate the latter would have cost me something like a nickel
a month. But then again I'm already I'm on a roll at cutting expenditures so why not just eek out the rest of the marginal returns right?

But seriously, what really reeled me in was that I'd already planned to use Git so it was
just too convenient of a choice not to go with. As for the reason why I wanted to use
Git, it was because it would serve as both a VCS and my potential backup.

## Having a reliable backup

Using Git to keep track of my changes allows me to easily have a copy of all
past states of my blog. If for some reason I impetuously decided to delete a bunch
of posts or change my layouts dramatically only to regret it the next day, no
problem. It's as simple as reverting those changes to get back everything I want. So
using Git (or any VCS), something I would be unable to do so using
Squarespace, essentially allows me to have a backup of all publications of my
website for any point in time.

So not only do I now have an easy format to copy and transfer around all of my
posts to USB, Dropbox, S3, or whatever, I also have a snapshot of everything
that's been published on the page and the changes made between.

I haven't ignored AWS S3 completely as I store a compressed backup there. According to
their FAQ:

>[if you store 10,000 objects with Amazon S3, you can on average expect to incur a loss of a single object once every 10,000,000 years](https://aws.amazon.com/s3/faqs/#data-protection).

so it's just really nice to have around either way even if I am not using it as
a hosting service and instead just as a compressed dump store instead.

Since the move I no longer have that nagging voice in my head about "that one"
unnecessary expenditure. I also now have a very durable backup(s) of my site, so
I rest much more at ease at knowing I likely won't lose anything or be held hostage
for this data.

For those interested, everything related to this blog can be found in these
two repositories:

* [Website content](https://github.com/ryaka/rheakara)
* [Hugo theme used] (https://github.com/ryaka/mila)

I warn you that there isn't really any documentation(at the time of this writing) but
I do intent to add them. Feel free to use the theme if you'd like however I don't
have any plans to offer support for the theme or any promises against breaking
changes as I'm making changes to it along the way to fit my needs as they come.
