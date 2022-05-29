---
---
{% for category in site.data.categories %}{% assign collection = site.collections | where: "label", category[0] | first %}{% assign name = category[1].name %}{% include category_index.html collection=collection name=name %}
{% endfor %}