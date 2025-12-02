---
layout: default
title: Home
---

# Welcome

This is the homepage of your academic portfolio site.

## About

Add your bio and introduction here.

## Research Interests

- Interest 1
- Interest 2
- Interest 3

## Recent Publications

{% if site.data.publications %}
<ul>
{% for pub in site.data.publications %}
  <li>
    <strong>{{ pub.title }}</strong> ({{ pub.year }})
    <br>
    <em>{{ pub.venue }}</em>
    {% if pub.link %}<br><a href="{{ pub.link }}">Link</a>{% endif %}
  </li>
{% endfor %}
</ul>
{% else %}
<p>No publications listed yet.</p>
{% endif %}

## Videos

{% if site.data.videos %}
<ul>
{% for video in site.data.videos %}
  <li>
    <strong>{{ video.title }}</strong>
    {% if video.description %}<br>{{ video.description }}{% endif %}
    {% if video.url %}<br><a href="{{ video.url }}">Watch</a>{% endif %}
  </li>
{% endfor %}
</ul>
{% else %}
<p>No videos listed yet.</p>
{% endif %}

## Contact

Add your contact information here.
