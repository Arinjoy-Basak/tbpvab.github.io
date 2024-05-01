---
layout: page
title: Officers
permalink: /officers/
---

{% for board in site.data.yearly-positions %}
  {% if board.year == site.data.sitewide.current-year %}
  {% for position in board.positions %}
  {% assign position-name = position[0] %}
  {% assign person-name = position[1] %}
  <img class="headshot" src="{{ site.baseurl }}/uploads/headshots/{{ person-name }}.jpg">
  
  [{{ site.data.sitewide.positions-details[position-name] }} - {{ site.data.officers[person-name].name }}]({{ site.baseurl }}/officers/{{ person-name }})

  {% endfor %}
  {% endif %}
{% endfor %}

<br>
<hr>
<br>
[Past Officers]({{ site.baseurl }}{% link past-officers.md %})