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

<a name="{{ idea.name }}"></a>
{% if idea.packageName %}
### {{ idea.title }} - DONE
<a href="https://play.google.com/store/apps/details?id={{ idea.packageName }}">
<img alt="Get it on Google Play" src="https://developer.android.com/images/brand/en_generic_rgb_wo_45.png" />
</a>
{% else %}
### {{ idea.title }}
{% endif %}

{{ idea.content }}

<script type="text/javascript">
function show_idea_link{{ forloop.index }}() {
	document.getElementById('idea_link{{ forloop.index }}').style.display = 'block';
	document.getElementById('show_idea_link{{ forloop.index }}').style.display = 'none';
}
</script>
<div class="idea-share">
<a class="ideas-share-button" id="show_idea_link{{ forloop.index}}" onClick="show_idea_link{{ forloop.index }}()">Link</a>
<a class="ideas-share-link" id="idea_link{{ forloop.index }}" href="#{{ idea.name }}">{{ site.url }}{{ site.baseurl }}ideas#{{ idea.name }}</a>
</div>


{% endfor %}
