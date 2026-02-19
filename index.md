---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home 
---
{% for project in site.projects %}
    {% if project.public %}
<div class="art-grp" id="art01">
    <div class="art-label-container">
        <p class="art-title">{{ project.title }}</p>
        <p class="art-desc">{{ project.description }}</p>
    </div>
    <!-- <div class="art-img-container"> -->
    <a href="{{ project.url }}" class="art-img-container"><img class="art-img" src=".{{ project.image }}"/></a>
    <!-- </div> -->
    
</div>
    {% endif %}
{% endfor %}
