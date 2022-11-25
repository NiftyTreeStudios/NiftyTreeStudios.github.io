---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
Welcome to the Nifty Tree Studios website. An alias for [Iiro Alhonen](https://www.iiroalhonen.com) used for publishing and developing independent iOS apps.

## Apps

{% for app in site.apps %}
  <h2>
    <a href="{{ app.url }}">
      {{ app.title }}
    </a>
  </h2>
  <p>{{ app.description | markdownify }}</p>
{% endfor %}
