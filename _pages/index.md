---
layout: page
title: Home
id: home
permalink: /
---

# 🌱 **Step Into Taylor's Digital Garden!** 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
You've discovered my curated space of reflections and ideas. Wander through, absorb the insights, and let them stir your own thoughts. If a seedling here resonates or provokes, I'd love to hear your perspective. After all, this garden flourishes best with diverse views and insights.
</p>

## Templates

All 'Template' notes are not ideas or notes designed to be read, their sole purpose is to speed up the note creation process within my Obsidian vault.

## Maps of Content (MOCs)

Each MOC is a guide to a specific knowledge domain, linking related ideas together. Similarly, they are note designed to be read but are required within my Obsidian vault.<br> <br> <strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>