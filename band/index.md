---
layout: default
bg: band.jpg
title: Band
heading: The Band
---
<table class="table">
	{% for member in site.data.band.members %}	
		<tr>
			<td>{{ member.name }}</td>
			<td>{{ member.instrument }}</td>
			<td>{{ member.hometown }}</td>
		</tr>
	{% endfor %}
</table>

###Officers
<ul class="unstyled">
	{% for position in site.data.band.officers %}
		<li><strong class="inline-h">{{ position.title }}</strong> {{ position.name }}</li>	
	{% endfor %}
</ul>
