---
layout: default
title: News
permalink: /news/
---

# {{ page.title }}

Any big, newsworthy announcements are made here and on [the Facebook page](https://www.facebook.com/HobartMakers/).

Content that's more immediate, such as project documentation goes onto the [liveblog](/liveblog).

---

{% for post in site.posts %}

**{{ post.title | escape }}** - {{ post.date | date: "%-d %b %Y" }}
{{ post.content }}
---

{% endfor %}

<!--p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p-->


