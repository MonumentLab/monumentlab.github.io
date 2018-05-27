---
layout: default
title: Proposal text
permalink: /mlab-data/
---


{% for proposal in site.data.mlab %}
{% include proposal.html %}
{% endfor %}

{% for lab in site.data.labs %}
  <h2> {{ lab.name }} </h2>
{% endfor %}
