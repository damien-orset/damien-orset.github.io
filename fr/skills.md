---
lang: fr
ref: skills
---

# Mes compétences

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

## Techniques

<table>
    <thead><tr><th></th><th>Techno</th><th>Niveau</th><th>Dernière référence</th></tr></thead>
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

## Autres

2018 : Trophée des Objets Connecté de Sophia (TOCS)

Prix du design + Prix du public pour notre boitier connecté WellNest 

"Wellnest est un boitier autonome, discret et design à poser dans un environnement afin d’en monitorer la qualité (nuisance sonore, luminosité, qualité de l’air, etc)."

Sources :
- [Communiqué de presse](http://www.sofab.tv/2018/07/dry-it-yourself-remporte-la-3eme-edition-3-autres-projets-primes/)
- [Vidéo de présentation](https://youtu.be/gkcNFQsuiCQ?t=461)

Formation : Ingénieur généraliste, Ecole Centrale Marseille, 2011

:fr: maternel

:us: fluent

:es: fluent