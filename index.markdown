---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Gallery index
layout: index
---

{% for exhibit in site.exhibits %}
<img src="{{ exhibit.image-url }}" width = 256>
<p>{{ exhibit.title }} by {{exhibit.creator }}</p>
<p><a href= "{{ exhibit.licence-url }}">{{ exhibit.licence }}</a></p>

{% endfor %}