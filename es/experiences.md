---
lang: es
ref: experiences

description: >-
  Impulsado por mi curiosidad tecnológica y gracias a mis numerosas experiencias en diferentes contextos de clientes, he forjado una sólida visión en el campo de los datos.
  Aporto mi experiencia y conocimientos a mis clientes para apoyarlos en su transformación centrada en los datos.
  Autónomo, perseverante y profundamente adaptable, puedo trabajar en diferentes campos y tareas tecnológicas.
  Me apasiona la tecnología, la divulgo y me gusta compartir mis descubrimientos a mi alrededor.
---

# Mis experiencias

## Proyectos

{% assign posts=site.posts | where:"lang", page.lang | where:"type", "project" | sort: date_start | reverse %}
<table>
    <thead>
      <tr>
        <th>Cliente</th>
        <th>Fetcha</th>
        <th>Trabajo</th>
        <th>Descripción</th>
        <th>Tecnologías</th>
      </tr>
    </thead>
    <tbody>
        {% for post in posts %}
        <tr>
            {% assign date_start_timestamp=post.date_start | date: "%s" %}
            {% assign date_end_timestamp=post.date_end | date: "%s" %}
            <td><a class="post-link" href="{{ post.url | prepend: site.baseurl }}"><img src="/assets/images/customer/{{ post.client }}.png" alt="{{ post.client }}" style="max-width: 100px;"/></a></td>
            <td>{{ post.date_start | date: "%b%y" }}<br>{{ post.date_end | date: "%b%y" }}
              {% if post.date_end %}
                <br>({{ date_end_timestamp | minus: date_start_timestamp | divided_by: 2592000}}m)
              {% else %}
                <br>({{ "today" | date: "%s" | minus: date_start_timestamp | divided_by: 2592000}}m)
              {% endif %}
            </td>
            <td>{{ post.job }}</td>
            <td>{{ post.description | truncate: 200 }} - <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">ver más</a></td>
            <td style="text-align: center;">{% for tech in post.technos %}<img src="/assets/images/skills/{{ tech }}.png" title="{{ tech }}" alt="{{ tech }}" style="max-width: 50px; max-height: 50px; margin: 5px"/>{% endfor %}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

## Preventa

{% assign posts=site.posts | where:"lang", page.lang | where:"type", "presale" | sort: date_start | reverse %}
<table>
    <thead>
      <tr>
        <th>Cliente</th>
        <th>Fetcha</th>
        <th>Trabajo</th>
        <th>Descripción</th>
        <th>Tecnologías</th>
      </tr>
    </thead>
    <tbody>
        {% for post in posts %}
        <tr>
            {% assign date_start_timestamp=post.date_start | date: "%s" %}
            {% assign date_end_timestamp=post.date_end | date: "%s" %}
            <td><a class="post-link" href="{{ post.url | prepend: site.baseurl }}"><img src="/assets/images/customer/{{ post.client }}.png" alt="{{ post.client }}" style="max-width: 100px;"/></a></td>
            <td>{{ post.date_start | date: "%b%y" }}<br>{{ post.date_end | date: "%b%y" }}
              {% if post.date_end %}
                <br>({{ date_end_timestamp | minus: date_start_timestamp | divided_by: 2592000}}m)
              {% endif %}
            </td>
            <td>{{ post.job }}</td>
            <td>{{ post.description | truncate: 200 }} - <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">ver más</a></td>
            <td style="text-align: center;">{% for tech in post.technos %}<img src="/assets/images/skills/{{ tech }}.png" title="{{ tech }}" alt="{{ tech }}" style="max-width: 50px; max-height: 50px; margin: 5px"/>{% endfor %}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>