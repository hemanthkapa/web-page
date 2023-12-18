---
layout: page
title: Welcome! 🥬
id: home
---

<section class="callout">
	Take a look at <a href="/your-first-note.html" class="internal-link">Your First Note</a> to get started on your exploration.
</section>

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>

{% include_relative README.md %}
