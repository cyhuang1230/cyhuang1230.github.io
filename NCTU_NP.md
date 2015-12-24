---
layout: page
title: NCTU Network Programming Projects
permalink: /NCTU_NP/
---

Projects I worked on in graduate-level course [__Network Programming__](https://course.nctu.edu.tw/Course/CrsOutline/show.asp?Acy=104&Sem=1&CrsNo=5247) in NCTU in Fall 2015.<br/>
<small><font color="gray">This course will be completed in Jan., 2016. Total 4-5 projects expected.</font></small>

<ul class="post-list">
{% for post in site.posts %}
{% for category in post.categories %}
{% if category == "network_programming" %}
<li>
<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
<h2>
<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
</h2>
{{ post.excerpt }}
</li>
{% endif %}
{% endfor %}
{% endfor %}
</ul>