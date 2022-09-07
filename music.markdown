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
    <td> <a href="https://github.com/{{ arr.recording }}">link</a> </td>
    <td> <a href="https://github.com/{{ arr.sheet }}">link</a> </td>
  </tr>
{% endfor %}
</table>
