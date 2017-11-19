---
layout: default
title: Proposal text
permalink: /mlab-data/
---


{% for proposal in site.data.mlab2017 %}
  <div>
    <h3><strong>{{ proposal.title }}</strong></h3>
    <h4>{{ proposal.transcription }}</h4>
    <h4>zip: {{ proposal.zipcode }} age: {{ proposal.age }} {% if proposal.credit %}, {{ proposal.credit }} {% endif %}</h4>
    <p><a href="http://monumentlab-research.muralarts.org/resourcespace/plugins/leaflet_rs/pages/direct_view.php?ID={{ proposal.ID }}" target="blank">View Proposal</a> </p>
    <hr />
  </div>

  {% if proposal.lab == 'City Hall' %}
    Hello tobi
  {% endif %}


{% endfor %}
