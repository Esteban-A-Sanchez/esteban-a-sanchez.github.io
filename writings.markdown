---
layout: default
title: "Writings"
permalink: /writings/
---
<h3 style="text-align:center;">some things i've written</h3>


<html>
    <ul class="post-list">
        {% for post in site.posts %}
            <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                <br>
                <small>{{ post.date | date: "%B %d, %Y" }}</small>
            </li>
        {% endfor %}
    </ul>
</html>