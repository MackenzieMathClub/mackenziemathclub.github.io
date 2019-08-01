---
title: Archived Lessons
description: Lessons from previous years for all members of Math Club.
layout: default
permalink: /archive/
---

[Current Lessons](https://mackenziemathclub.github.io/lessons/)

2018-2019 Lessons coming soon!™

<div class="big">Former Lessons Archive</div>

<div>
	{% for lesson in site.data.archive reversed %}
		<dt>Lesson {{ lesson.id }}. {{ lesson.title }} {{ lesson.date }}</dt>
		{% assign title = lesson.title %}
		{% if lesson.nickname %}
			{% assign title = lesson.nickname %}
		{% endif %}
		<dd>
			<a href="{{ lesson.presentation }}">{{ title }} Presentation</a>
			{% if lesson.worksheet %}
				<br>
				<a href="{{ lesson.worksheet }}">{{ title }} Worksheet</a>
			{% endif %}
			{% if lesson.problems %}
				<br>
				<a href="{{ lesson.problems }}">{{ title }} Problems</a>
			{% endif %}
		</dd>
	{% endfor %}
</div>
