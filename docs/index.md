---
layout: default
---

# Regional Coupled Models

<table>
  <thead>
    <tr>
      <th>Model</th>
      <th>Description</th>
      <th>Extended label</th>
    </tr>
  </thead>
  <tbody>
    {% for model in site.models %}
    <tr>
      <td><a href="{{ model.url }}">{{ model.title }}</a></td>
      <td>{{ model.description }}</td>
      <td>{{ model.label_extended }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>

