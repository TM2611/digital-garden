---
layout: page
title: Home
id: home
permalink: /
---

# 🌱 **Step Into Taylor's Digital Garden!** 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
You've discovered my curated space of reflections and ideas. It is important to note that EVERYTHING you see here are my own personal thoughts- they may be 'right' or 'wrong' and should not be treated as fact. I will often give my understanding of a word or concept, but these are by no means official definitions (I tend to try to avoid those). Wander through, absorb the insights, and let them stir your own thoughts. If a seedling here resonates or provokes, I'd love to hear your perspective. After all, this garden flourishes best with diverse views and insights.
</p>

## Notes

My digital garden consists of 4 kinds of notes.
#### 1. **Fleeting Notes** 🍂

Prefixed with 'F - ' (or F), these are the initial seeds of thought. They capture the essence of a fleeting idea, an inspiration from a book I've read, a conversation I've had, or a concept I've encountered. Think of them as the raw, unpolished gems that are waiting to be refined - or simply a 'to explore' list. They're spontaneous and often succinct, serving as placeholders for deeper exploration later on.

#### 2. **Permanent Notes** 🌳

As ideas mature and grow, they find their way here. Permanent notes represent a more thorough exploration, synthesis, and understanding of concepts. They're the result of nurturing fleeting thoughts, connecting them with other ideas, and letting them take root in a more structured form. Permanent notes are by no means 'complete', all notes in the digital garden will evolve over time.

#### 3. Templates 📄
Templates are the blueprints for note-taking in the garden, ensuring consistent formatting and structure. Primarily designed to streamline the note-creation process in my Obsidian vault, they help maintain uniformity across all entries.

#### 4. Maps of Content (MOCs) 🌐
MOCs are the compasses of the digital garden, providing an overview of specific knowledge areas. They link related notes and chart out interconnected ideas, serving as essential navigational tools within my Obsidian vault

Each Fleeting and Permanent note has a section for 'Thoughts and Questions', this section is primarily to prompt my own thoughts so that I can expand on the note in future - however they may also serve as prompts for the potential reader. Templates and MOCs are not direct reflections of thoughts, readings, or experiences like the Fleeting and Permanent notes - they're just used to help my structure my Obsidian vault.

<br> <strong>Recently updated notes</strong>

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