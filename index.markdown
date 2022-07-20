---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: index
---

<ul class="list-unstyled">
    {% for post in site.posts %}
      <li class="row col-12">
      <h2 class="d-flex">
        <span class="col-3">
            {{ post.date | date: "%m/%d/%Y" }}
        </span>
        <a href="{{ post.url }}" class="col">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
</ul>
