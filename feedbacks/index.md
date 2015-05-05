---
layout: page
title: "Категория: Отзывы"
description: "Про бизнес-интернет-вергилия подробнее"
---
<h1>{{ page.tag }}</h1>

<ul>
{% for post in site.categories.feedbacks %}
      <li>
        <span class="post-date">{{ post.date | date: "%-d. %m . %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a><br>
        <span class="post-decription">{{post.description}}</span>
      </li>
{% endfor %}
</ul>