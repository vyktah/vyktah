---
# front matter tells Jekyll to process Liquid
---
{{ "Hello world!" | number_of_words }}
{% for article in site.articles %}
    {{ forloop.index  }}yes
{% endfor %}
{{site.posts}}
{{site.collections}}
{{site.documents}}
{{site.articles}}
<image src="images/foo.jpg" alt="foo" width="500">
