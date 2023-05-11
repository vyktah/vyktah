---
# front matter tells Jekyll to process Liquid
---
{{ "Hello world!" | number_of_words }}
{% for file in site.static_files %}

    {{ forloop.index  }}
    {{file.modified_time}} 
    {{file.name}} 
    {{file.basename}}
    {{file.extname}}
    
{% endfor %}
{% include_relative test.md %}
<image src="images/foo.jpg" alt="foo" width="500">
