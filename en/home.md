---
layout: default
title: "Welcome"
lang: "en"
---
## Welcome!
Welcome to this online Escape game about Sci-Fi and Fantasy books !<br>

Instead of searching a room, you will search this blog : “Space Queen Starla’s bookquest” in order to find 5 books to highlight on her special post for the Utopiales.<br>

{% assign filtered_puzzle_lang = site.puzzles | where: 'lang', page.lang %}
<ul>
  {% for puzzle in filtered_puzzle_lang %}
    <li>
      <h5><a href="{{ puzzle.url | absolute_url}}">{{ puzzle.title }}</a></h5>
    </li>
  {% endfor %}
</ul>