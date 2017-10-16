---
title: Lessons
description: Lessons for all members of Math Club.
layout: default
permalink: /lessons/
---

<div>
	{% for lesson in site.data.lessons %}
		<dt>Lesson {{ lesson.id }}: {{ lesson.title }} {{ lesson.date }}</dt>
		<dd>
			<a href="{{ lesson.presentation }}">{{ lesson.title }} Presentation</a>
			{% if lesson.worksheet %}
				<br>
				<a href="{{ lesson.worksheet }}">{{ lesson.title }} Worksheet</a>
			{% endif %}
		</dd>
	{% endfor %}
</div>
