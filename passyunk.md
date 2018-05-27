---
layout: default
title: passyunk
permalink: /passyunk/
---


{% for proposal in site.data.mlab %}
  {% if proposal.zipcode_cleaned == "19147" %}
  {% include proposal.html %}
  {% endif %}
{% endfor %}
