---
title: "Discounts"
layout: default
---
# Discounts

We offer several discounts to people and causes we believe in.
Here are some of the most important causes we support.
You may only apply one discount at a time.

<ul>
  {% for discount in site.data.discounts %}
    <li><a href="#{{ discount.name | replace: ' ', '-' }}">{{ discount.name }}</a></li>
  {% endfor %}
</ul>

{% for discount in site.data.discounts %}
  <h2 id="{{ discount.name | replace: ' ', '-' }}">{{ discount.name }}</h2>
  {% for par in discount.paragraphs %}
  <p>{{ par }}</p>
  {% endfor %}
{% endfor %} 
