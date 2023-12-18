---
layout: page
title: Welcome! 🥬
id: home
---
# Hi, I'm Hemanth 🌱

---
![Image](assets/images/IMG_5994.jpeg)


Welcome to my corner of the internet, a place where I share my thoughts in all shapes and sizes. Here, you'll find an eclectic mix of notes- some are brief sparks of inspiration meant to solve immediate challenges, visible to the world for shared utility. Others are elaborate journeys through the vast landscapes of big ideas, offering a deeper dive into the subjects that fascinate me. This space is not just a collection of words, but a reflection of my intellectual odyssey, constantly evolving and growing."

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
