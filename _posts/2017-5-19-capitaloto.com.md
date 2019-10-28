---
layout: post
title:  "CapitalOto.com"
projects: true
tag:
- work
- design
---
Shortly before my first internship ended, a software architect under whom I worked told me,

>Being a software engineer a little funny. It's not like being a building architect or a carpenter, where you can drive by a house and tell your kid, "I built that!"
>
>With websites it's more like, "Well I didn't build this, but I fixed a lot of bugs in it."

## I got to break the mold last semester and rebuild an entire website for a client.

In January, I received a certain job alert from the wonderful CS Department Secretary Chris Coonrad: A local ear, nose, and throat practice was looking for (and willing to pay) "an undergraduate student, versed in website design, to help us update our current webpage".

![original site](/assets/images/site_old.png){: title="Eugh." }
<figcaption class="caption">The original site, last updated circa 2012.</figcaption>

A quick look at the existing website showed that it needed some serious work&mdash;the secondary navigation was nearly invisible; too many pages were dry walls of text; similar information that could've fit in one place was located in separate subpages. Most importantly, the two main functions that the site was supposed to perform, scheduling appointments and guiding the user to their Patient Portal, did not make themselves abundantly distinct on the homepage.

Check out the old site yourself [on the Wayback Machine](https://web.archive.org/web/20170127015216/http://capitaloto.com/), if you dare.

![audiology](/assets/images/audiology.png){: title="the horror" }
<figcaption class="caption">Not pictured: the maze of medical literature accessible from the sidebar on the left.</figcaption>

*Damn,* I thought. *What a great opportunity! Tons of extremely qualified students are definitely gonna apply for this...Oh well, I might as well try.* So I sent over my newly HTML-migrated resume and promptly forgot about it.

Five months later, I'd rebuilt Capital Otolaryngology's website from the ground up with Jekyll, designed them a completely new logo, and written up a pretty detailed README containing maintenance instructions for self-described "non-computer people". Also, the practice administrator told me that I was one of only about three people who'd sent in their resume for the requisition. Go figure.

## Process

TODO import from notes

## Final deliverables

![new site](/assets/images/site_new.png)
<figcaption class="caption">A landing page that will actually make visitors want to continue.</figcaption>

![mobile map](/assets/images/map_mobile.png){: title="delicious responsiveness" }
<figcaption class="caption">Feeling Responsive, the Jekyll template I used, is true to its name.</figcaption>

![new logo](https://github.com/dawneraq/capitaloto/blob/master/assets/img/capitaloto_logo.png?raw=true)
<figcaption class="caption">Perhaps the most challenging part of the whole undertaking.</figcaption>

## What I learned

### On the design side

- Regarding the new logo: client-designer disagreements (and stubornness, on either side) are an inescapable part of the visual design process. Some visual abstraction that makes sense to you may not read the same to someone else.
- Free tools that let you create interactive wireframes of webpages must be a closely guarded industry secret. [Moqups](https://moqups.com/) isn't bad though.
- Content management for a website that hasn't been updated in a while is its own can of worms. Its roadblocks may include an inability to take new high-resolution photos on short notice, or the delicate balancing act between brevity and necessity for large bodies of text.

### On the dev side

- A lot of web templating languages are essentially the same&mdash;Liquid, which Jekyll uses, was easy to pick up after already knowing Angular.
- Internet Explorer is very particular about the order in which Google Maps API resources are loaded.
- DevTools' device emulator alone isn't enough to ensure that mobile views look the way you want them to.

### Also

- That "comic book superhero neck muscle" in the logo is called the sternocleidomastoid.

## What I would've done differently

- Given that the majority of the site's users are on the older side, and therefore may need accessibility accommodations, I would've gone through the front-end and made sure that the site's content was compatible with screen readers.
- User testing of initial designs, especialy with not-so-computer-literate people.

You can see the site for yourself [here](https://capitaloto.com) and the source code [here](https://github.com/dawneraq/capitaloto).
