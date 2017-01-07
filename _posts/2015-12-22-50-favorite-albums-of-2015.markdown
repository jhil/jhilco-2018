---
layout:   post
type:     list
title:    "50 Favorite Albums of 2015"
date:     2015-12-22
thumb:    Currents.png
hero:     false
color:    "#6D8D3D"
---

I keep a tight playlist on Spotify called "[Albums To Listen To](https://open.spotify.com/user/1211985885/playlist/14xZS8LcVMQ59SRG8k2FQU)." I drop in new and new-found albums to… well… listen to. Here are my favorite picks from the list that were released in 2015. Scroll all the way to the bottom to see my top choices!

A few quick and cursory observations:

- Pop is hot. The radio is infectious. Dancing makes pop videos werk.
- Metropolis / indie electronic is a really cool new sound that seems to be universally enjoyed. The genre is starting to get mature, so it will be interesting to see where it goes next year.
- Based on the nature of these playlists, I listen to the first few tracks of an album way more than the last few tracks. But my favorites-of-favorites are all albums where I can groove with each and every song.
- EPs, mixtapes, and unofficial releases make up much of my top picks. Maybe these outlets reduce the pressure on artists to meet studio expectations and ultimately increase creativity.

<span class="sub">Note. This isn’t the People’s Choice Awards, just what I enjoyed the most :)</span>

---

<ul class="list article-list list-photo list-shadow list-numbered">
{% for 2015-album in site.data.2015-albums limit:50 %}
  <li class="list-item">
    <div class="list-row">
      <a href="{{ 2015-album.link }}">
        <img src="/img/{{ page.title | slugify }}/{{ 2015-album.album }}.jpg" class="list-image">
      </a>
      <a href="{{ 2015-album.link }}">
        <h3 class="list-title">{{ 2015-album.album }}<span class="subsub"> – </span><span class="sub">{{ 2015-album.artist }}</span></h3>
      </a>
      <h5 class="list-detail">{{ 2015-album.genre }}</h5>
    </div>
  </li>
{% endfor %}
</ul>
