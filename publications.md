---
layout: default
title: Publications
---

# Publications

A selection of peer-reviewed publications, preprints, talks, and posters. For full citations or PDFs, see each entry. If you need a copy, please contact me.

{% if site.data.publications %}
<div class="publications-list">
{% for pub in site.data.publications %}
  <div class="publication">
    {% if pub.image %}
    <img src="{{ pub.image | relative_url }}" alt="Graphical abstract for {{ pub.title }}">
    {% endif %}
    <div class="pub-details">
      <h3>{{ pub.title }}</h3>
      {% if pub.authors %}
      <p class="pub-authors">{{ pub.authors }}</p>
      {% endif %}
      <p class="pub-venue"><em>{{ pub.venue }}</em> ({{ pub.year }})</p>
      {% if pub.type %}
      <p class="pub-type"><strong>{{ pub.type | capitalize }}</strong></p>
      {% endif %}
      {% if pub.link %}
      <a href="{{ pub.link }}" class="pub-link" target="_blank">View Publication →</a>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>
{% else %}
<p>Publications will be listed here soon. Please check back later or contact me for information about my research.</p>
{% endif %}
