---
lang: es
ref: customers

description: >-
  Impulsado por mi curiosidad tecnológica y gracias a mis numerosas experiencias en diferentes contextos de clientes, he forjado una sólida visión en el campo de los datos.
  Aporto mi experiencia y conocimientos a mis clientes para apoyarlos en su transformación centrada en los datos.
  Autónomo, perseverante y profundamente adaptable, puedo trabajar en diferentes campos y tareas tecnológicas.
  Me apasiona la tecnología, la divulgo y me gusta compartir mis descubrimientos a mi alrededor.
---

# Clientes

Aquí está la lista de clientes para los que he trabajado.

<table>
    <thead>
      <tr>
        <th>Fetcha</th>
        <th>Cliente</th>
        <th>Campo profesional</th>
        <th>Descripción</th>
        <th>Trabajo</th>
      </tr>
    </thead>
    <tbody>
        {% assign clients=site.data.customers | sort: "date" | reverse %}
        {% for client in clients %}
        <tr>
          <td>{{ client.date }}</td>
          <td><img src="/assets/images/customer/{{ client.name }}.png" style="max-width: 100px;"/></td>
          <td>{{ client.vertical }}</td>
          <td>{{ client.description[page.lang] }}</td>
          <td>{{ client.job }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

