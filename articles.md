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
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

## カテゴリー別

### 基礎知識
<ul>
{% for post in site.categories.basics %}
  <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>

### 実践
<ul>
{% for post in site.categories.practice %}
  <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>

### 比較
<ul>
{% for post in site.categories.comparison %}
  <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
