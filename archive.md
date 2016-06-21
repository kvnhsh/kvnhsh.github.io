---
title: Archive
permalink: archive/
---


{% if page.archive %}
    <ul id="post-list" class="archive readmore">
        <h3>Read more</h3>
        {% for post in site.posts %}
            <li>
                <a href="{{ site.baseurl }}{{ post.url | remove_first: '/' }}">{{ post.title }}<aside class="dates">{{ post.date | date:"%b %d" }}</aside></a>
            </li>
        {% endfor %}
    </ul>
{% endif %}
