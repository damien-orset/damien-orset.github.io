---
lang: us
ref: customers

description: >-
  Driven by my technological curiosity and thanks to my many experiences in different customer contexts, I have forged a solid vision in the field of data.
  I bring my experience and expertise to my clients to support them in their data-centric transformation.
  Autonomous, persevering and deeply adaptable, I can work on different fields and technological tasks.
  I am passionate about technology, I popularize and like to share my discoveries around me.
---

# Customers

Here's the client list for whom I have worked for

<table>
    <thead>
      <tr>
        <th>Date</th>
        <th>Customer</th>
        <th>Vertical</th>
        <th>Description</th>
        <th>Job</th>
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

