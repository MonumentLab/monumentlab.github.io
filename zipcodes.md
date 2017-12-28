---
layout: default
title: Zipcodes
permalink: /zipcodes/
---


{% for zipcode in site.data.zipcodes_poly %}
  <div>
    <h1>{{ zipcode.code }}</h1>
      <div>
      {% for proposal in site.data.mlab2017 %}
        {% if proposal.zipcode == zipcode.code %}
          {% include proposal.html %}
          <br />
        {% endif %}
      {% endfor %}  
      </div>
  </div>


{% endfor %}
