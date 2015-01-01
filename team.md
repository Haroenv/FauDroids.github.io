---
layout: page
title: Team
---

{% for author in site.data.members %}

<div class="empty"></div>

<a name="{{ author[0] }}"></a>
<img class="author-gravatar" src="http://www.gravatar.com/avatar/{{ author[1].gravatar }}?d=mm&s=55" alt="gravatar" />
### {{ author[1].name }}
<div class="author-role">{{ author[1].role }}</div>

{{ author[1].message }}

<div class="author-contact">

{% if author[1].github %}
<a href="https://github.com/{{ author[1].github }}" target="_blank">
<img src="{{ site.baseurl }}/public/imgs/icon_github.svg" with="30" height="30" alt="github"/>
</a>
{% endif %}

{% if author[1].email %}
<a href="mailto:{{ author[1].email }}" target="_top">
<img src="{{ site.baseurl }}/public/imgs/icon_mail.svg" with="30" height="30" alt="email"/>
</a>
{%endif %}

{% if author[1].homepage %}
<a href="{{ author[1].homepage }}" target="_blank">
<img src="{{ site.baseurl }}/public/imgs/icon_home.svg" with="30" height="30" alt="homepage"/>
</a>
{%endif %}
</div>
<br>

{% endfor %}
