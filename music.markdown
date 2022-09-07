---
layout: page
title: music
permalink: /music/
---

A collection of all the projects I've worked on.

<table>
  <tr>
    <th> name </th>
    <th> composer </th>
    <th> instrumentation </th>
    <th> recording </th>
    <th> sheet </th>
  </tr>
{% for arr in site.data.arrangements %}
  <tr>
    <td> {{ arr.name }} </td>
    <td> {{ arr.composer }} </td>
    <td> {{ arr.instrumentation }} </td>
    <td> <a href="{{ arr.recording }}">link</a> </td>

    {% assign filename = arr.name | split: "(" | first | downcase | strip | replace: " ", "_" %}
    {% assign sheets = site.static_files | where: "sheet", true %}
    {% for sheet in sheets %}
      {% if sheet.basename == filename %}
        <td> <a href="{{ sheet.path }}">link</a> </td>
      {% endif %}
    {% endfor %}
  </tr>
{% endfor %}
</table>
