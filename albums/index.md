---
layout: default
title: "Albums & Merchandise"
bg: music.jpg
published: true
---

Oberlin Steel has recorded nine albums: five under its former name, The Can Consortium, and four under its current; the band’s newest album, Welcome to the Swanktuary, was released in May 2013. For track listings and more information, click on the album titles below.

Any albums still in print can either be purchased here through Paypal or by e-mailing the band at [osteel@oberlin.edu](osteel@oberlin.edu). Many of our albums (as noted below) can also be found [on bandcamp](http://oberlinsteel.bandcamp.com). Additionally, we have rad t-shirts and stickers for sale at the end of this page. If you'd like to order multiple items at once, it's most efficient to e-mail your order to the band.

Each album the band has produced has a unique style all its own. As veteran members graduate and new members bring their own influences and musicality to the band, Oberlin Steel redefines itself each year with a new sound. The band’s current repertoire focuses mostly on traditional steelband music—calypso and soca tunes from the past and present, with some pop and jazz mixed in.

<div class="row clearfix margin-leader">
	{% for post in site.categories.albums %}
		<div class="col-xs-12 col-sm-4 card-wrapper">
			<div class="card row clearfix">
				<a href="{{ site.baseurl }}{{ post.url }}" class="col-xs-6 col-sm-12">
					<img class="img-responsive" src="{{ site.baseurl }}{{ site.image_url }}/albums{% if post.thumb %}-small{% endif %}/{{ post.image }}">
				</a>
				<div class="col-xs-6 col-sm-12">
					<a href="{{ site.baseurl }}{{ post.url }}">
						<h4>{{ post.title }}</h4>
					</a>
					<p>
						{% if post.year %}
							{{ post.year }}{% endif %}{% if post.year && post.cost %},
						{% endif %}
						{% if post.cost %}
							{{ post.cost }}
						{% endif %} <span>{% for medium in post.medium %}<span class="slash-list-item">{{ medium }}</span>{% endfor %}</span>
					</p>
					{% if post.paypal %}
						<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_blank">
							<input type="hidden" name="cmd" value="_s-xclick">
							<input type="hidden" name="hosted_button_id" value="{{ page.paypal }}">
								<input type="submit" class="a" name="submit" value="Buy with PayPal">
						</form>
					{% endif %}
					{% if post.bandcamp %}
						<a href="http://oberlinsteel.bandcamp.com/album/{{ post.bandcamp }}">Listen on Bandcamp</a>
					{% endif %}
				</div>
			</div>
		</div>
	{% endfor %}
</div>
