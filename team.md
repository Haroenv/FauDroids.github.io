---
layout: page
title: Team
---

{% for author in site.authors %}
### {{ author[1].name }}<a name="{{ author[0] }}"></a>
<div class="author-role">{{ author[1].role }}</div>

{{ author[1].message }}

<div class="author-contact">

{% if author[1].github %}
<a href="https://github.com/{{ author[1].github }}" target="_blank">
<img src="{{ site.baseurl }}/public/imgs/icon_github.svg" with="40" height="40" alt="github"/>
</a>
{% endif %}

{% if author[1].email %}
<a href="mailto:{{ author[1].email }}" target="_top">
<img src="{{ site.baseurl }}/public/imgs/icon_mail.svg" with="40" height="40" alt="email"/>
</a>
{%endif %}

{% if author[1].homepage %}
<a href="{{ author[1].homepage }}" target="_blank">
<img src="{{ site.baseurl }}/public/imgs/icon_home.svg" with="40" height="40" alt="homepage"/>
</a>
{%endif %}

</div>

{% endfor %}
