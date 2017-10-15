---
title: Lessons
description: Lessons for all members of Math Club.
layout: default
permalink: /lessons/
---

<div>
	{% for lesson in site.data.lessons %}
		<dt>Lesson {{ lesson.id }}: {{ lesson.date }}</dt>
		<dd>
			<a href="{{ lesson.url }}">{{ lesson.title }}</a>
		</dd>
	{% endfor %}
</div>
