---
layout: page
title: 記事一覧
permalink: /articles/
---

## すべての記事

<ul>
  {% for post in site.posts %}
    <li>
      <span>{{ post.date | date: "%Y-%m-%d" }}</span> » 
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

## カテゴリー別

### 基礎知識
{% for post in site.categories.基礎知識 %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}

### 実践
{% for post in site.categories.実践 %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}

### 比較
{% for post in site.categories.比較 %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
