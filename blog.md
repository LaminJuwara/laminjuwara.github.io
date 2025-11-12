---
layout: singlePage
title: "Blog Posts"
---

<style type="text/css">
body {
  font-size: 16px;
}
td {
  font-size: 8px;
}
h1.title {
  font-size: 20px;
  color: DarkRed;
}
h1 {
  font-size: 20px;
  color: DarkBlue;
}
h2 {
  font-size: 18px;
}
h3 {
  font-size: 20px;
  font-family: "Times New Roman", Times, serif;
}
code.r {
  font-size: 16px;
}
pre {
  font-size: 16px;
}
</style>

--- 

---



### Blog Posts

Welcome to my blog, where I share insights, tutorials, and reflections on topics in biostatistics, data science, reproducible research, and statistical computing. Posts range from practical coding guides in R and Python to deep dives into methodology and applied case studies in health research.

Each entry reflects lessons from my academic projects, collaborative research, or tools I've developed and tested.

Browse the list of published posts below:

<table class="table table-hover">
  {% for post in site.posts %}
    {% unless post.draft %}
    <tr>
      <td><a href="{{ post.url }}">{{ post.title }}</a></td>
      <td class="col-md-3" style="text-align: right;">{{ post.date | date: "%B %e, %Y" }}</td>
    </tr>
    {% endunless %}
  {% endfor %}
</table>
