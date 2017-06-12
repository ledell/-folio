---
layout: page
permalink: /docs/
title: poetry
description: Documents
---

<ul class="post-list">
{% for doc in site.docs reversed %}
    <li>
        <h2><a class="poem-title" href="{{ doc.url | prepend: site.baseurl }}">{{ doc.title }}</a></h2>
        <p class="post-meta">{{ doc.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>