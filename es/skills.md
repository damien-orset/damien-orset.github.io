---
lang: es
ref: skills

description: >-
  Impulsado por mi curiosidad tecnológica y gracias a mis numerosas experiencias en diferentes contextos de clientes, he forjado una sólida visión en el campo de los datos.
  Aporto mi experiencia y conocimientos a mis clientes para apoyarlos en su transformación centrada en los datos.
  Autónomo, perseverante y profundamente adaptable, puedo trabajar en diferentes campos y tareas tecnológicas.
  Me apasiona la tecnología, la divulgo y me gusta compartir mis descubrimientos a mi alrededor.
---

# Mis habilidades

## Certificaciones

<table>
    <thead><tr><th></th><th>Certificaciones</th><th>Fetcha</th></tr></thead>
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

## Technicas

<table>
    <thead><tr><th></th><th>Techno</th><th>Nivel</th><th>Ultima referencia</th></tr></thead>
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

## Globales

<ul>
    {% assign skills=site.data.skills | where:"type", "global" %}
    {% for s in skills[0].list %}
    <li>
      <span>{{ s.name }}</span>
    </li>
    {% endfor %}
</ul>

## Otras

2018: Sophia Connected Objects Trophy (TOCS)

Premio de diseño + Premio del público para nuestra caja conectada WellNest

"Wellnest es una caja autónoma, discreta y elegante que se coloca en un entorno para controlar su calidad (contaminación acústica, luminosidad, calidad del aire, etc.)".

Fuentes:
- [Nota de prensa](http://www.sofab.tv/2018/07/dry-it-yourself-remporte-la-3eme-edition-3-autres-projets-primes/)
- [Presentación](https://youtu.be/gkcNFQsuiCQ?t=461)

Diploma : Engineer, Ecole Centrale Marseille, 2011

:fr: nativo

:us: fuido

:es: fuido