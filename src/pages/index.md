---
permalink: '/index.html'
eleventyExcludeFromCollections: true
---

<nav>
<ul>
  {% for post in collections.garden %}
  <li>
    <a href="{{ post.url }}">{{ post.data.title }}</a>
    <time datetime='{{ page.date | datetime }}'>{{ post.date | common }}</time>
  </li>
  {% endfor %}
  </ul>
</nav>
