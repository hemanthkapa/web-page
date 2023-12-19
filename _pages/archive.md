---
layout: page
title: Archive
---

<h1>Archive</h1>

<table class="archive-table">
  <thead>
    <tr>
      <th>Title</th>
      <th>Category</th>
      <th>Last Updated</th>
    </tr>
  </thead>
  <tbody>
    {% for note in site.notes %}
    <tr>
      <td><a href="{{ note.url }}{%- if site.use_html_extension -%}.html{%- endif -%}" class="internal-link">{{ note.title }}</a></td>
      <td>{% if note.category != null %}{{ note.category }}{% else %}N/A{% endif %}</td>
      <td>{{ note.last_modified_at | date: "%B %Y" }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>

