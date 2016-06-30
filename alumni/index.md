---
layout: default
bg: alumni.jpg
title: Alumni
---

This crazy band of ours has a long and very twisted history starting in 1980! Following is a list of the two decades of Obies who have passed through the panyard. The list is nowhere near complete, so if you have any further information, please, please, please send it to the band. Down at the bottom you'll find our founding members, who started something kinda neat, and we all thank you!

<table class="table table-condensed table-hover">
	<thead>
		<tr>
			<th class="col-sm-3">Name
			<th class="col-sm-3">Instruments
			<th class="col-sm-2">Years
			<th class="col-sm-4">About
		
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

