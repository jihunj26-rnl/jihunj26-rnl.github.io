layout: page
title: people
permnalink: /people/
nav: true
nav_order: 2

## Principal Investigator

{% raw %}
{% for person in site.data.people.pi %}
- **{{ person.name }}**  
  {{ person.role }}  
  {{ person.email }}
{% endfor %}
{% endraw %}

## PhD Students

{% raw %}
{% for person in site.data.people.phd %}
- **{{ person.name }}**  
  {{ person.role }}  
  {{ person.research }}
{% endfor %}
{% endraw %}
