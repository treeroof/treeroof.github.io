---
layout: default
---

  <h1>Tutorials</h1>
  <p>{{ site.tutorial }}</p>
  <ul class="tutorials">
    {% for tutorial in site.tutorials %}
    <li>
      <a class="post-link" href="{{ tutorial.url | prepend: site.baseurl }}"
        >{{ tutorial.tutorial | capitalize }}</a
      >
    </li>
    {% endfor %}
  </ul>