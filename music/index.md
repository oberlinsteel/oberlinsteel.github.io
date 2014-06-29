---
layout: default
title: Music
bg: music.jpg
body-class: inverse
---
Oberlin Steel has recorded eight albums, five under its former name, The Can Consortium, and three under its current; the band’s newest album, Pan on the Moon, was released in February 2009.

Each album the band has produced has a unique style all its own. As veteran members graduate and new members bring their own influences and musicality to the band, Oberlin Steel redefines itself each year with a new sound. The band’s current repertoire focuses mostly on traditional steelband music—calypso and soca tunes from the past and present, with some pop, jazz, and bossa mixed in.

For track listings and more information, click on the album titles below. Many of our albums (as noted below) can also be found [on bandcamp(http://oberlinsteel.bandcamp.com).

<ul class="media-list">
	{% for post in site.categories.music %}
		<li class="media">
			<a class="pull-left" href="{{ site.baseurl }}{{ post.url }}">
				<img class="media-object" src="{{ site.baseurl }}{{ site.image_url }}/albums/{{ post.image }}" width="100">
			</a>
			<div class="media-body">
				<h4 class="media-heading"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h4>
				<p>{{ post.year }}, {{ post.medium }}{% if post.bandcamp %}, <a href="http://oberlinsteel.bandcamp.com/album/{{ post.bandcamp }}">on bandcamp</a>{% endif %}</p>
			</div>
		</ul>
	{% endfor %}
</ul>
