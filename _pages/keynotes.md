---
title: Keynotes
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: https://cvis2021.weebly.com/uploads/5/6/3/0/56308869/background-images/236520036.jpg
  actions:
permalink: /keynotes
toc: true
keynotes:
  - title: 
    time:
    url:
    image: 
    abstract:
    author:
      name: 
      description: 
      bio: 

  - title: 
    time:
    url:
    image: 
    abstract:
    author:
      name: 
      description: 
      bio:
  - title:
    time:
    url: 
    image: 
    abstract: 
    author:
      name:
      description: 
      bio:
  - title: 
    time: 
    url: 
    image: 
    abstract: 
 
    author:
      name:
      description:
      bio:

---


{% for keynote in page.keynotes %}
## {{ keynote.title }}
<img src="{{ keynote.image}}" class="align-left" style="width: calc(30% - 0.5em);"/>

{% if keynote.time %} <sub>{{keynote.time}} </sub>  {% endif %}


{% if keynote.url %} <sub> {{keynote.url}}</sub> {% endif %}

{% if keynote.abstract %}
**Abstract:** 
{{keynote.abstract}}
{% endif %}

**Speaker Info:**
{{keynote.author.name}}

{{keynote.author.description}}

{{keynote.author.bio}}

{% endfor %}
