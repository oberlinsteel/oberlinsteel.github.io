---
layout: default
bg: band.jpg
title: Band
heading: The Band
---
<table class="table">
	{% for member in site.data.alumni.members %}	
		<tr>
			<td>{{ member.name }}</td>
			<td>{{ member.instrument }}</td>
			<td>{{ member.years }}</td>
			<td>{{ member.etc }}</td>
		</tr>
	{% endfor %}
</table>
