---
title: Foster Parent Licensing Plays
description: Here you will find a collection of some best practices on foster parent licensing from our members.
layout: page
sidenav: sidebar
subnav:
  - text: Kinship
    href: /kinship
  - text: Foster Parent Licensing
    href: /licensing
  - text: Extended Foster Care
    href: /extended-foster-care
  - text: COVID-19
    href: /covid-19
---

{{ page.description }}

<ul>
  {% assign filtered_posts = site.pages | where: 'topic', 'licensing' %}
  {% for post in filtered_posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
	{{ post.description }}
	<p>
	<b>Who can do this?</b> {{ post.audience }}<br />
	<b>Cost:</b> {{ post.cost }}<br />
	<b>Timeframe:</b> {{ post.timeframe }}<br />
	<b>Difficulty:</b> {{ post.difficulty }}<br />
	</p>
  {% endfor %}
</ul>