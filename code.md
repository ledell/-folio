---
layout: page
permalink: /code/
title: code
description: Code.
---

<ul class="post-list">
{% for code in site.code reversed %}
    <li>
        <h2><a class="code-title" href="{{ code.url | prepend: site.baseurl }}">{{ code.title }}</a></h2>
        <p class="post-meta">{{ code.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>

