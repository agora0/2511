---
title: 朝鮮日報
layout: page
permalink: /chosun/
---
{% for category in site.categories %}
  {% if category.first == "chosun" %}
  <div>
    {% for post in category.last %}
    <span class="postdate">{{ post.date | preserve_timezones }}</span> • <span class="author">CHOSUN</span>
    <h4><a href="{{site.url}}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h4>
    {% endfor %}
  </div>
  {% endif %}
{% endfor %}


