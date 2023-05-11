---
# front matter tells Jekyll to process Liquid
---
{{ "Hello world!" | number_of_words }}
{% for blog in blogs %}
  {% for article in blog.articles %}
    {{ article.title }}
  {% endfor %} 
{% endfor %}
<image src="images/foo.jpg" alt="foo" width="500">
