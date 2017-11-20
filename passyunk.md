---
layout: default
title: passyunk
permalink: /passyunk/
---


{% for proposal in site.data.mlab2017 %}
  {% if proposal.zipcode == "19147" %}
  <div>
    <h3><strong>{{ proposal.title }}</strong></h3>
    <h4>{{ proposal.transcription }}</h4>
    <h4>zip: {{ proposal.zipcode }} age: {{ proposal.age }} {% if proposal.credit %}, {{ proposal.credit }} {% endif %}</h4>
    <h4> <strong>type:</strong> {{ proposal.type }} <strong>topic:</strong> {{ proposal.topic }} </h4>
    <p><a href="http://monumentlab-research.muralarts.org/resourcespace/plugins/leaflet_rs/pages/direct_view.php?ID={{ proposal.ID }}" target="blank">View Proposal</a> </p>
    <hr />
  </div>
  {% endif %}


{% endfor %}
