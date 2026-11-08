
---
layout: page
title: Weekly Coding Progress
permalink: /progress/
---

# My Coding Journey

Learning by building, experimenting and reflecting.

## Current Focus

- JavaScript and Node.js
- Express.js
- React and Next.js
- Database and API development
- Software security

## Weekly Learning History

{% assign entries = site.posts | where_exp: "post", "post.categories contains 'coding-progress'" %}

{% for post in entries %}

### {{ post.title }}

*{{ post.date | date: "%d %B %Y" }}*

{{ post.excerpt }}

[Read more]({{ post.url | relative_url }})

---

{% endfor %}
