---
layout: page
title: School Projects (NCTU)
permalink: /NCTU_Projects/
---

Projects I worked during the time in CS, NCTU.<br/>


<ul class="post-list">
{% for category in site.categories %}
		{% assign now_cat = (category | first) %}
		{% case now_cat %}
			{% when 'network_programming' %}
				{% assign link = "/NCTU_NP/" %}
				{% assign cat = "Network Programming (2015 Fall)" %}
			{% when 'bdataa' %}
				{% assign link = "/NCTU_BDATAA/" %}
				{% assign cat = "Big Data Analytics Techniques and Applications (2016 Spring)" %}
			{% else %}
				{% continue %}
		{% endcase %}
		<li>
			<a href="{{ link }}">{{ cat }}</a>
			<ul>
				{% for posts in category %}
					{% for post in posts %}
						{% if post.url %}
							<li><a href="{{ post.url }}">{{ post.title }}</a></li>
						{% endif %}
					{% endfor %}
				{% endfor %}
			</ul>
		</li>
{% endfor %}

</ul>