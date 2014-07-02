---
layout: default
title: Albums
bg: music.jpg
---
Oberlin Steel has recorded eight albums, five under its former name, The Can Consortium, and four under its current; the band’s newest album, Welcome to the Swanktuary, was released in May 2012.

Each album the band has produced has a unique style all its own. As veteran members graduate and new members bring their own influences and musicality to the band, Oberlin Steel redefines itself each year with a new sound. The band’s current repertoire focuses mostly on traditional steelband music—calypso and soca tunes from the past and present, with some pop, jazz, and bossa mixed in.

For track listings and more information, click on the album titles below. Many of our albums (as noted below) can also be found [on bandcamp](http://oberlinsteel.bandcamp.com).

<div class="row clearfix margin-leader">
	{% for post in site.categories.albums %}
		<div class="col-xs-12 col-sm-4 card-wrapper">
			<div class="card row clearfix">
				<a href="{{ site.baseurl }}{{ post.url }}" class="col-xs-6 col-sm-12">
					<img class="img-responsive" src="{{ site.baseurl }}{{ site.image_url }}/albums/{{ post.image }}">
				</a>
				<div class="col-xs-6 col-sm-12">
					<a href="{{ site.baseurl }}{{ post.url }}">
						<h4>{{ post.title }}</h4>
					</a>
					<p>{{ post.year }}, {{ post.medium }}{% if post.bandcamp %} <a href="http://oberlinsteel.bandcamp.com/album/{{ post.bandcamp }}">on bandcamp</a>{% endif %}</p>
				</div>
			</div>
		</div>
	{% endfor %}
</div>
