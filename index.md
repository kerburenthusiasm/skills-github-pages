---
layout: default
---

# Kerb Writeups

I'm a security analyst with a focus on offensive security and vulnerability research. Through this blog, I share detailed writeups from CTF competitions and security research I find interesting.

---

## Latest Writeups

{% if site.posts.size > 0 %}
{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
**{{ post.date | date: "%B %d, %Y" }}**

{% if post.excerpt %}
{{ post.excerpt }}
{% endif %}

[Read full writeup →]({{ post.url | relative_url }})

---
{% endfor %}
{% else %}
<p>No posts yet. Check back soon!</p>
{% endif %}