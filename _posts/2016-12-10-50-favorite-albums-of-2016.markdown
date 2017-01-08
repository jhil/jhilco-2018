---
layout:   post
type:     list
title:    "50 Favorite Albums of 2016"
date:     2016-12-10
tag:      music
thumb:    Lunacy.jpeg
hero:     false
color:    "#FEEE35"
link:     https://open.spotify.com/user/1211985885/playlist/14xZS8LcVMQ59SRG8k2FQU
---

<ul class="list article-list list-photo list-photo-big list-shadow list-numbered">
{% for 2016-album in site.data.2016-albums limit:50 %}
  <li class="list-item">
    <div class="list-row">
      <a href="{{ 2016-album.link }}">
        <img src="/img/{{ page.title | slugify }}/{{ 2016-album.album }}.jpeg" class="list-image">
      </a>
      <a href="{{ 2016-album.link }}" target="_blank">
        <h3 class="list-title">{{ 2016-album.album }}<span class="subsub"> – </span><span class="sub">{{ 2016-album.artist }}</span></h3>
      </a>
      <h5 class="list-detail">{{ 2016-album.genre }}</h5>
    </div>
  </li>
{% endfor %}
</ul>

{% include button-link.html text="Spotify Playlist" dark=true %}
