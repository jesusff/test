---
layout: default
---

# Regional Coupled Models

<table>
  <thead>
    <tr>
      <th>Model</th>
      <th>source_id</th>
      <th>Extended label</th>
      <th>Atmosphere</th>
      <th>Land</th>
      <th>Ocean</th>
    </tr>
  </thead>
  <tbody>
    {% for model in site.models %}
    <tr>
      <td><a href="{{ site.baseurl }}{{ model.url }}">{{ model.label }}</a></td>
      <td>{{ model.source_id }}</td>
      <td>{{ model.label_extended }}</td>
      <td>{{ model.atmosphere.label }}</td>
      <td>{{ model.land.label }}</td>
      <td>{{ model.ocean.label }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>

## Atmospheric components

<table>
  <thead>
    <tr>
      <th>Model</th>
      <th>Atmosphere</th>
      <th>Resolution</th>
      <th>Levels</th>
      <th>Radiation</th>
      <th>...</th>
    </tr>
  </thead>
  <tbody>
    {% for model in site.models %}
    <tr>
      <td><a href="{{ site.baseurl }}{{ model.url }}">{{ model.label }}</a></td>
      <td>{{ model.atmosphere.label }}</td>
      <td>{{ model.atmosphere.resolution }}</td>
      <td>{{ model.atmosphere.levels }}</td>
      <td>{{ model.atmosphere.physics.radiation.label }}</td>
      <td>...</td>
    </tr>
    {% endfor %}
  </tbody>
</table>


