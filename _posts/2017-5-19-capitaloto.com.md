---
layout: post
title:  "CapitalOto.com"
projects: true
tag:
- work
---
Shortly before my first internship ended, a software architect under whom I worked named Grant Ricklefs told me,

>Being a software engineer a little funny. It's not like being a building architect or a carpenter, where you can drive by a house and tell your kid, "I built that!"
>
>With websites it's like, "Well I didn't build this, but I fixed a lot of bugs in it."

### I got a great opportunity last semester to break the mold and build an entire website for a client.

In January, I received a certain job alert from the wonderful CS Department Secretary Chris Coonrad: A local ear, nose, and throat practice was looking for (and willing to pay) "an undergraduate student, versed in website design, to help us update our current webpage".

![original site](/assets/images/site_old.png){: title="Eugh." }
<figcaption class="caption">The original site, last updated circa 2012.</figcaption>

A quick look at the existing website showed that it needed some serious work.

![audiology](/assets/images/audiology.png){: title="the horror" }
<figcaption class="caption">Not pictured: the maze of medical literature accessible from the sidebar on the left.</figcaption>

*Damn,* I thought. *Tons of extremely qualified students are definitely gonna apply for this. Oh well, I might as well try.* So I sent over my newly HTML-migrated resume and promptly forgot about it.

Five months later, I'd rebuilt Capital Otolaryngology's website from the ground up with Jekyll, designed a completely new logo, and written up a pretty detailed README containing maintenance instructions for self-described "non-computer people". Also, the practice administrator told me that I was one of about three people who'd sent in their resume for the requisition.

![new site](/assets/images/site_new.png){: title="Much better!" }
<figcaption class="caption">A landing page that will actually make visitors want to continue.</figcaption>

![mobile map](/assets/images/map_mobile.png){: title="Delicious responsiveness!" }
<figcaption class="caption">Feeling Responsive, the Jekyll template I used, is true to its name.</figcaption>

![new logo](https://github.com/dawneraq/capitaloto/blob/master/assets/img/capitaloto_logo.png?raw=true){: title="I could see a similar design on a craft beer or something." }
<figcaption class="caption">Perhaps the most challenging part of the whole undertaking.</figcaption>

### Here are some things I learned:
- Disagreements (and maybe stubornness) are an inescapable part of the visual design process.
- Tools that let you create interactive wireframes of webpages must be a closely guarded industry secret. [Moqups](https://moqups.com/) isn't bad though.
- A lot of web templating languages are essentially the same&mdash;Liquid, which Jekyll uses, was easy to pick up after already knowing Angular.
- Content management for a website that hasn't been updated in a while is its own can of worms. Its roadblocks may include an inability to take new high-resolution photos on short notice, or the delicate balancing act between brevity and necessity for large bodies of medicine-related text.
- Internet Explorer is very particular about the order in which Google Maps API resources are loaded.
- DevTools' device emulator alone isn't enough to ensure that mobile views look the way you want them to.
- That "comic book superhero neck muscle" in the logo is called the sternocleidomastoid.

You can see the site for yourself [here](https://capitaloto.com) and the source code [here](https://github.com/dawneraq/capitaloto).
