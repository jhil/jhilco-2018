---
layout:   post
type:     list
title:    "Board Games"
date:     2016-09-03
link:     www.boardgamegeek.com/user/jhilmd
color:    "#1d265c"
hero:     false
---

I love collecting board games and sharing fun times with friends and family. These are the games in my personal collection right now. Check out my [BoardGameGeek profile](https://www.boardgamegeek.com/user/jhilmd) for more games and ratings.

<ul class="list post-list list-photo list-numbered">
{% for boardgame in site.data.boardgames %}
  <li class="list-item">
    <div class="list-row">
      <a href="{{ boardgame.link }}">
        <img src="/img/board-games/{{ boardgame.title | slugify }}.jpg" class="list-image">
      </a>
      <a href="{{ boardgame.link }}">
        <h3 class="list-title">{{ boardgame.title }}</h3>
      </a>
      <h4 class="list-detail"><em>{{ boardgame.rating }}</em>&#8202;/&#8202;10</h4>
    </div>
    <p>{{ boardgame.description }}</p>
  </li>
{% endfor %}
</ul>

{% include button-link.html text="See more games on BoardGameGeek" %}
