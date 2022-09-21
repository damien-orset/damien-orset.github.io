---
lang: fr
ref: customers
---

# Clients

Voici la liste des clients chez qui j'ai pu intervenir

<table>
    <thead>
      <tr>
        <th>Date</th>
        <th>Client</th>
        <th>Secteur</th>
        <th>Description</th>
        <th>Poste</th>
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