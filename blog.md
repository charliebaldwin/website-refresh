---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Blog 
---

<div class="blog-links-grp">
  {% for post in site.blogposts %}
    <a class="blog-link" href="{{ post.url }}">
        <div class="blog-link-container">
            <div class="blog-link-title-grp">
                <h2 class="blog-link-title">{{ post.title }} </h2>
                <p class="blog-link-date">{{ post.date | date:"%b %-d, %Y" }} </p>
            </div>
            <p class="blog-link-desc">{{ post.content | strip_html | truncatewords: 30 }} </p>
        </div>
    </a>
  {% endfor %}
</div>