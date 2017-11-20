---
layout: default
title: About
permalink: /about.html
---

The analysis of Monument Lab Data is designed to be public. We encourage anyone and everyone to take part. This site is a very early way to quickly share analyses. As we're further along, we'll add more.

[View All Proposals Text](http://monumentlab.github.io/mlab-data.html)

{{ labs.where }}


View Proposals by where they were proposed:
  {% for lab in site.data.labs %}
  <p>  This is the {{ lab.cityhall.name }}.</p>
  {% endfor %}
