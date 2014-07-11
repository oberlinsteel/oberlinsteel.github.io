---
layout: default
bg: alumni.jpg
title: Alumni
heading: Alumni
---
<table class="table table-condensed table-hover">
	<thead>
		<tr>
			<th class="col-sm-3">Name</td>
			<th class="col-sm-3">Instruments</td>
			<th class="col-sm-2">Years</td>
			<th class="col-sm-4">About</td>
		</tr>
	</thead>
	<tbody>
		{% for member in site.data.alumni.members %}	
			<tr>
				<td class="col-sm-3 xs-strong">{{ member.name }}</td>
				<td class="col-sm-3">{{ member.instruments }}</td>
				<td class="col-sm-2">{{ member.years }}</td>
				<td class="col-sm-4 xs-em">{{ member.etc }}</td>
			</tr>
		{% endfor %}
	</tbody>
</table>
