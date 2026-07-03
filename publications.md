---
layout: default
title: Publications
---

# Publications

Peer-reviewed publications, preprints, and theses spanning computational materials science and molecular quantum chemistry. Current work focuses on vacancy–solute coupling and grain-boundary segregation in nuclear alloys using DFT and ML potentials, building on earlier contributions in noncovalent molecular interactions and colorimetric sensing.

{% if site.data.publications %}
<div class="publications-list">
{% assign sorted_pubs = site.data.publications | sort: "year" | reverse %}
{% assign current_year = "" %}
{% for pub in sorted_pubs %}
  {% capture pub_year %}{{ pub.year }}{% endcapture %}
  {% if pub_year != current_year %}
    {% assign current_year = pub_year %}
<h3 class="pub-year-heading">{{ pub.year }}</h3>
  {% endif %}
  <div class="publication">
    {% if pub.image %}
    <img src="{{ pub.image | relative_url }}" alt="Graphical abstract for {{ pub.title }}">
    {% endif %}
    <div class="pub-details">
      <h3>{{ pub.title }}</h3>
      {% if pub.authors %}
      <p class="pub-authors">{{ pub.authors }}</p>
      {% endif %}
      <p class="pub-venue"><em>{{ pub.venue }}</em></p>
      {% if pub.type %}
      <p class="pub-type"><strong>{{ pub.type | capitalize }}</strong></p>
      {% endif %}
      {% if pub.link %}
      <a href="{{ pub.link }}" class="pub-link" target="_blank">PDF</a>
      {% endif %}
      {% if pub.talk_page %}
      <a href="{{ pub.talk_page | relative_url }}" class="pub-link" style="margin-left: 1rem;">Talk / Presentation Page →</a>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>
{% else %}
<p>Publications will be listed here soon. Please check back later or contact me for information about my research.</p>
{% endif %}
