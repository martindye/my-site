---
permalink: index.html
title: blog.codemartin.com
show_description: true
show_counter: true
---

{% include welcometext.html %}

{% for category in site.categories %}

{% assign findcat = category[0] %}
{% assign findcat = findcat | append: '.md' %}
{% assign hascatmenu = false %}

{% for sitepage in site.pages %}
    {% if sitepage.path == findcat %}
	{% assign hascatmenu = true %}
    {% endif %}
{% endfor %}

{% if hascatmenu %}
<h3><a href="/{{ category[0] }}.html">{{ category[0] }}</a></h3>
{% else %}
 <h3>{{ category[0] }}</h3>
{% endif %}
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

