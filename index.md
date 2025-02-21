---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
[Submit New Page](https://github.com/peers8862/reboot/issues/new?template=content_form.yml) - Add your own content to this site!

<h2>Site Pages</h2>
<ul>
  {% for page in site.pages %}
    {% if page.path contains '_pages/' %}
      <li><a href="{{ page.url | relative_url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

