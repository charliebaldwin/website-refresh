---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home 
---
{% for work in site.works %}
<div class="art-grp" id="art01">
    <div class="art-img-container">
        <a href="{{ work.url }}"><img class="art-img" src="{{ work.image }}"/></a>
    </div>
    <div class="art-label-container">
        <p class="art-label">{{ work.description }}</p>
    </div>
</div>
{% endfor %}
