---
permalink: /
title: "Tarun Prakash"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a Mission Operations Engineer at [Nominal](https://www.nominal.io/), where I deploy software that accelerates hardware testing for mission-critical systems. Before joining Nominal, I spent a year in the U.S. government as a [NobleReach Scholar](https://noblereach.org/), working on the National Security Space Launch program at Space Systems Command and supporting dual-use startup investments at SpaceWERX.

I studied mechanical engineering at Purdue University and began my career working on hardware programs at SpaceX and Tesla. In parallel, I’ve founded multiple startups, including Nize, an edtech company.

I’m interested in aerospace, particularly space systems, defense tech, and national security, with a focus on how startups and government partners deliver mission-critical capabilities. I’m especially motivated by work at the intersection of innovation, policy, and public service, where engineering rigor and speed directly shape real-world outcomes.

## Featured
{% assign all_items = site.posts | concat: site.media | sort: 'date' | reverse %}
{% for item in all_items limit:3 %}
{% if item.collection == 'media' %}- [{{ item.title }}]({{ item.link }}) — *{{ item.venue }}*
{% else %}- [{{ item.title }}]({{ item.url }}){% if item.subtitle %} — {{ item.subtitle }}{% endif %}
{% endif %}{% endfor %}
