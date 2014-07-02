---
layout: default
bg: alumni.jpg
title: Alumni
heading: Alumni
---
<table class="table table-condensed table-hover">
	{% for member in site.data.alumni.members %}	
		<tr>
			<td class="col-xs-3">{{ member.name }}</td>
			<td class="col-xs-3">{{ member.instruments }}</td>
			<td class="col-xs-2">{{ member.years }}</td>
			<td class="col-xs-4">{{ member.etc }}</td>
		</tr>
	{% endfor %}
</table>
