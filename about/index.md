---
title: "About"
layout: default
---

# Our Team

<ul>
{% for member in site.data.team %}
<li>{{ member.name }}</li>
{% endfor %}
</ul>
