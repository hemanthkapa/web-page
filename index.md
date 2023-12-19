---
layout: default
title: Welcome! 🥬
id: home
---
# Hi, I'm Hemanth 🌱

---

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<div style="display: flex; align-items: flex-start; gap: 30px; margin-top: 20px;">
    <div style="flex: 1; max-width: 700px;">
        <img src="assets/images/IMG_5994.jpeg" alt="Image" style="width: 100%; height: auto; border-radius: 10px;">
    </div>
    <div style="flex: 2; padding: 20px; background-color: rgba(156, 213, 56, .08); border-radius: 10px;">
        Welcome to my corner of the internet, a place where I share my thoughts in all shapes and sizes. Here, you'll find an eclectic mix of notes- some are brief sparks of inspiration meant to solve immediate challenges, visible to the world for shared utility. Others are elaborate journeys through the vast landscapes of big ideas, offering a deeper dive into the subjects that fascinate me. This space is not just a collection of words, but a reflection of my intellectual odyssey, constantly evolving and growing.
    </div>
</div>

<!-- Recently Updated Notes Section -->
<div style="margin-top: 30px;">
    <strong>Recently updated notes</strong>
    <ul style="list-style: none; padding: 0;">
        {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
        {% for note in recent_notes limit: 5 %}
        <li style="margin-bottom: 10px;">
            {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
        </li>
        {% endfor %}
    </ul>
</div>

<style>
  .wrapper {
    max-width: 46em;
    margin: auto;
  }

  /* Flexbox Layout for Larger Screens */
  div {
    display: flex;
    flex-wrap: wrap; /* Allows items to wrap on smaller screens */
    gap: 30px;
  }

  div > div {
    flex: 1; /* Each child takes equal space */
  }

  /* Image Styles */
  img {
    max-width: 100%; /* Ensure image is not larger than its container */
    height: auto; /* Maintain aspect ratio */
    border-radius: 10px;
  }

  /* Responsive Design for Mobile */
  @media (max-width: 768px) {
    div > div {
      flex-basis: 100%; /* Each child takes full width on smaller screens */
    }
  }
</style>