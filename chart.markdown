---
layout: default
title: Chart
permalink: /chart/
---

<table>
  {% for row in site.data.air-pollution-vs-gdp-per-capita %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

		{% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>