---
permalink: /
title: "Tarun Prakash"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a Mission Operations Engineer at [Nominal](https://www.nominal.io/), where I deploy and operate telemetry systems for aerospace and defense customers. Before joining Nominal, I spent a year in the U.S. government as a [NobleReach Scholar](https://noblereach.org/), working on national security space launches at Space Systems Command and supporting dual-use startup investments at SpaceWERX.

I studied mechanical engineering at Purdue University and interned at SpaceX before my time in government. I'm interested in space systems, defense technology, and building bridges between the tech industry and the public sector.

## Featured
{% assign all_items = site.posts | concat: site.media | sort: 'date' | reverse %}
{% for item in all_items limit:3 %}
{% if item.collection == 'media' %}- [{{ item.title }}]({{ item.link }}) — *{{ item.venue }}*
{% else %}- [{{ item.title }}]({{ item.url }}){% if item.subtitle %} — {{ item.subtitle }}{% endif %}
{% endif %}{% endfor %}
