---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  "摇摇，走走，摆摆。只有这一个办法能摆脱他。他统治世界，但没有权力统领移动中的东西，他知道，我们身体的移动是神圣的，只有动起来、离开原地的时候，你才能逃脱他的魔掌。他统治的是一切静止的、冻结的物事，每一样被动的、怠惰的东西。" </br>摘自奥尔加·托卡尔丘克 《云游》
</p>
<strong>All notes</strong>

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
