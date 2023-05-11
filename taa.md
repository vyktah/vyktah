---
# front matter tells Jekyll to process Liquid
---
{{ "Hello world!" | number_of_words }}
{% for file in site.static_files %}

    {{ forloop.index  }}
    {{file.path}} 
    {% render file.path %}
    {{file.modified_time}} 
    {{file.name}} 
    {% render file.name %}
    {{file.basename}}
    {% render file.basename %}
    {{file.extname}}
    
{% endfor %}

<image src="images/foo.jpg" alt="foo" width="500">
