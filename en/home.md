---
layout: default
title: "Welcome"
lang: "en"
---
## Welcome!
Welcome to this online Escape game about Sci-Fi and Fantasy books !<br>

Instead of searching a room, you will search this blog : “Space Queen Starla’s bookquest” in order to find 5 books to highlight on her special post for the Utopiales.<br>
This escape game is not linear, you have all the informations right at the start which can be overwhelming especially when you’re not sure what you’re looking for.<br>
Don’t hesitate to look at the clues below to help you out as you go along.
If there’s a technical problem or you really are stuck you can always “contact a human” and get some help.

{% assign filtered_puzzle_lang = site.puzzles | where: 'lang', page.lang %}
<ul>
  {% for puzzle in filtered_puzzle_lang %}
    <li>
      <h5><a href="{{ puzzle.url | absolute_url}}">{{ puzzle.title }}</a></h5>
    </li>
  {% endfor %}
</ul>