---
layout: page
title: AutoOfficers
permalink: /officers-temp/
published: false
---

{% for officer in site.officers %}
  <h2>
    <a href="{{ officer.permalink }}">
      {{ officer.name }} - {{ officer.position }}
    </a>
  </h2>
  <!-- <p>{{ staff_member.content | markdownify }}</p> -->
{% endfor %}