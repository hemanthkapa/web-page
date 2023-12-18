---
layout: default
title: Welcome! 🥬
id: home
---
# Hi, I'm Hemanth 🌱

---

<div style="display: flex; align-items: flex-start; gap: 30px; margin-top: 20px;">
    <div style="flex: 1; margin-right: 10px;">
        <img src="assets/images/IMG_5994.jpeg" alt="Image" style="width: 100%; height: auto; border-radius: 10px;">
    </div>
    <div style="flex: 2; padding: 20px; background-color: rgba(156, 213, 56, .08); border-radius: 10px;">
        Welcome to my corner of the internet, a place where I share my thoughts in all shapes and sizes. Here, you'll find an eclectic mix of notes- some are brief sparks of inspiration meant to solve immediate challenges, visible to the world for shared utility. Others are elaborate journeys through the vast landscapes of big ideas, offering a deeper dive into the subjects that fascinate me. This space is not just a collection of words, but a reflection of my intellectual odyssey, constantly evolving and growing.
    </div>
</div>

<!-- Recently Updated Notes Section -->
<strong style="display: block; margin-top: 30px; margin-bottom: 10px;">Recently updated notes</strong>

<ul style="padding-left: 20px;">
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li style="margin-bottom: 10px;">
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
  
  # Hi, I'm Hemanth 🌱 {
    margin-bottom: 0;
  }
</style>
