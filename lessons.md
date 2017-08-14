---
title: Lessons
description: Lessons for all students.
layout: default
permalink: /lessons/
---

# Intermediate
<div>
	{% for lesson in site.junior %}
		<a href="{{ lesson.url }}">{{ lesson.title }}</a><br>
	{% endfor %}
</div>

# Advanced
<div>
	{% for lesson in site.senior %}
		<a href="{{ lesson.url }}">{{ lesson.title }}</a><br>
	{% endfor %}
</div>
