---
lang: us
ref: skills

description: >-
    Driven by my technical curiosity, I bring my experience and expertise to my clients, to support them in their digital transformation.
    I build data architectures and shares my vision through big data consulting missions to my clients.
    Autonomous, perseverant and deeply adaptable, I can intervene on various technological domains and tasks.
    I am passionate about technology and enjoy sharing my discoveries.
---

# My Skills

## Certifications

<table>
    <thead><tr><th></th><th>Certification</th><th>Date</th></tr></thead>
    <tbody>
        {% assign skills=site.data.skills | where:"type", "certification" %}
        {% for s in skills[0].list  %}
        <tr>
            <td><img src="/assets/images/skills/{{ s.logo }}.png" alt="cert" width="100"/></td>
            <td><a href="{{ s.accredible }}">{{ s.name }}</a></td>
            <td>{{ s.date }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

## Technical

<table>
    <thead><tr><th></th><th>Techno</th><th>Level</th><th>Latest reference</th></tr></thead>
    <tbody>
        {% assign skills=site.data.skills | where:"type", "tech" %}
        {% assign skills_sorted=skills[0].list | sort: "interest" | reverse %}
        {% for s in skills_sorted %}
        <tr class="skill_active_{{ s.active }}">
            <td><img src="/assets/images/skills/{{ s.name }}.png" alt="{{ s.name }}" width="100"/></td>
            <td>{{ s.name }}</td>
            <td>{% for index in (1..s.knowledge) %}:star:{% endfor %}</td>
            <td>
            {% if s.ref %}
            {% assign posts=site.posts | where:"lang", page.lang | where:"ref", s.ref %}
            <a href="{{posts[0].url | prepend: site.baseurl}}">{{ posts[0].client }}</a>
            {% endif %}
            </td>
        </tr>
        {% endfor %}
    </tbody>
</table>

## Global

<ul>
    {% assign skills=site.data.skills | where:"type", "global" %}
    {% for s in skills[0].list %}
    <li>
      <span>{{ s.name }}</span>
    </li>
    {% endfor %}
</ul>

## Other

2018: Sophia Connected Objects Trophy (TOCS)

Design award + Audience award for our WellNest connected box

"Wellnest is an autonomous, discreet and stylish box to place in an environment in order to monitor its quality (noise pollution, brightness, air quality, etc.)."

Sources :
- [Press release](http://www.sofab.tv/2018/07/dry-it-yourself-remporte-la-3eme-edition-3-autres-projets-primes/)
- [Présentation](https://youtu.be/gkcNFQsuiCQ?t=461)

Scholarship : Engineer, Ecole Centrale Marseille, 2011

:fr: native

:us: fluent

:es: fluent