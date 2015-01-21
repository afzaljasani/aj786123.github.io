---
layout: page
title: Photos
---

<p class="message">
	Hey there! This is my Photos page. I will be updating it with photos I have taken.
</p>


<div class="posts">
    {% for post in site.photos %}
    <div class="post">
        <a href="{{ post.url | prepend: site.baseurl }}">
          <h1 class="post-title">
            {{ post.title }}
          </h1>
        </a>

    <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>

      {{ post.content }}
    </div>
    {% endfor %}
</div>
