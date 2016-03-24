---
layout: page
title: NCTU Big Data Analytics Techniques and Applications Projects
permalink: /NCTU_BDATAA/
---

Projects I've worked on in graduate-level course [__Big Data Analytics Techniques and Applications Projects(巨量資料分析技術與應用)__](https://course.nctu.edu.tw/Course/CrsOutline/show.asp?Acy=104&Sem=2&CrsNo=5253) in NCTU in Spring 2016.<br/>
<small><font color="gray">This course will be completed in June, 2016. Total 3-4 projects expected.</font></small>

<ul class="post-list">
{% for post in site.posts %}
{% for category in post.categories %}
{% if category == "bdataa" %}
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