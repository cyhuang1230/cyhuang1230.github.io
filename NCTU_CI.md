---
layout: page
title: NCTU Computational Intelligence and Application Projects
permalink: /NCTU_CI/
---

Projects I've worked on in graduate-level course [__Computational Intelligence and Application(計算型智慧與應用)__](https://course.nctu.edu.tw/Course/CrsOutline/show.asp?Acy=104&Sem=2&CrsNo=5239) in NCTU in Spring 2016.<br/>
<small><font color="gray">This course will be completed in June, 2016. Total 4 projects expected.</font></small>

<ul class="post-list">
{% for post in site.posts %}
{% for category in post.categories %}
{% if category == "ci" %}
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
