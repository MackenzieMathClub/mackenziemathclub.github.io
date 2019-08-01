---
title: Lessons
description: Lessons for all members of Math Club.
layout: default
permalink: /lessons/
---

[Former Lessons](https://mackenziemathclub.github.io/archive/)

<div class="big">Lessons Archive</div>

<div>
	{% for lesson in site.data.lessons reversed %}
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
