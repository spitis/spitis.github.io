---
layout: default
permalink: /economics/
---

<h1>Economics</h1>

<p>A collection of older posts I've written on economics (or law and economics). These were automatically converted from word press entries, so latex and other formatting may not display properly.</p>

<br />

<ul class="post-list">
  {% for post in site.economics %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <h5>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h5>
    </li>
  {% endfor %}
</ul>
