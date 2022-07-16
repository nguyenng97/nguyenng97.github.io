---
layout: default
title: Home
nav_order: 0
has_children: false
has_toc: false
permanent_link: /
---

# Nguyen Nguyen's Blog
{: .fs-9}

Welcome to my **technical blog** slash **personal notes** from various topics I am researching in Data Science, Mathematics, and Sofware Engineering.
{: .fs-6 .fw-300}

[About me](/about){: .btn .btn-purple .mr-2} [View it on GitHub](https://github.com/nguyenntt97){: .btn }
{: .fs-5 .fw-250}
***

<h1>Recent Posts</h1>
<ul class="posts">
{% for post in site.docs limit:20 %}
    <li>
        <span class="post-date">{{ post.date | date: "%d %b %Y"}}</span>
        <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
        <br/>
        {{ post.description }}
    </li>
{% endfor %}
</ul>