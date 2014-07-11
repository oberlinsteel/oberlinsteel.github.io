---
layout: default
bg: band.jpg
title: Band
heading: The Band
---
<table class="table">
	<tbody>
		{% for member in site.data.band.members %}	
			<tr>
				<td class="xs-strong">{{ member.name }}</td>
				<td>{{ member.instrument }}</td>
				<td>{{ member.hometown }}</td>
			</tr>
		{% endfor %}
	</tbody>
</table>

###Officers
<ul class="unstyled ul-xs-table">
	{% for position in site.data.band.officers %}
		<li><strong class="inline-h">{{ position.title }}</strong> {{ position.name }}</li>	
	{% endfor %}
</ul>
