---
layout: page
title: Ideas
---

<div class="message">
	<cite>
		The best way to get a good idea is to get a lot of ideas. &mdash; Linus Pauling
	</cite>
</div>

This is a loosely organized list of potential Android app ideas, their
intentions and target groups.

{% for idea in site.data.ideas %}
### {{ idea.title }}
{{ idea.content }}
{% endfor %}
