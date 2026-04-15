layout: page
title: people
permnalink: /people/
nav: true
nav_order: 2

<style>
.people-section {
  margin-bottom: 3rem;
}

.people-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.5rem;
  margin-top: 1rem;
}

.person-card {
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 1rem;
  text-align: center;
  background: #fff;
}

.person-card img {
  width: 140px;
  height: 180px;
  object-fit: cover;
  border-radius: 10px;
  margin-bottom: 0.8rem;
}

.person-name {
  font-size: 1.05rem;
  font-weight: 600;
  margin-bottom: 0.3rem;
}

.person-role {
  color: #555;
  margin-bottom: 0.4rem;
}

.person-email,
.person-research {
  font-size: 0.92rem;
  margin-bottom: 0.3rem;
}
</style>

## Principal Investigator

<div class="people-grid">
{% raw %}{% for person in site.data.people.pi %}{% endraw %}
  <div class="person-card">
    <img src="{% raw %}{{ '/assets/img/photos' | append: pic_prof.png | relative_url }}{% endraw %}" alt="{% raw %}{{ person.name }}{% endraw %}">
    <div class="person-name">{% raw %}{{ person.name }}{% endraw %}</div>
    <div class="person-role">{% raw %}{{ person.role }}{% endraw %}</div>
    <div class="person-email">{% raw %}{{ person.email }}{% endraw %}</div>
    <div class="person-research">{% raw %}{{ person.research }}{% endraw %}</div>
  </div>
{% raw %}{% endfor %}{% endraw %}
</div>


## PhD Students

<div class="people-grid">
{% raw %}{% for person in site.data.people.pi %}{% endraw %}
  <div class="person-card">
    <img src="{% raw %}{{ '/assets/img/photos' | append: pic_jihun.jpg | relative_url }}{% endraw %}" alt="{% raw %}{{ person.name }}{% endraw %}">
    <div class="person-name">{% raw %}{{ person.name }}{% endraw %}</div>
    <div class="person-role">{% raw %}{{ person.role }}{% endraw %}</div>
    <div class="person-email">{% raw %}{{ person.email }}{% endraw %}</div>
    <div class="person-research">{% raw %}{{ person.research }}{% endraw %}</div>
  </div>
{% raw %}{% endfor %}{% endraw %}
</div>
