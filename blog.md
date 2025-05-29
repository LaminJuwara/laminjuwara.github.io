---
layout: singlePage
title: "Blog Posts"
---

<style type="text/css">

body{ /* Normal  */
      font-size: 15px;
  }
td {  /* Table  */
  font-size: 14px;
}
h1.title {
  font-size: 20px;
  color: DarkRed;
}
h1 { /* Header 1 */
  font-size: 20px;
  color: DarkBlue;
}
h2 { /* Header 2 */
    font-size: 20px;
}
h3 { /* Header 3 */
  font-size: 20px;
  font-family: "Times New Roman", Times, serif;
}
code.r{ /* Code block */
    font-size: 15px;
}
pre { /* Code block - determines code spacing between lines */
    font-size: 15px;
}
</style>

###

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
