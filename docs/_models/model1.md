---
source-id: Model1
label: Model 1
label_extended: My model 1 extended label
atmosphere:
  label: ALADIN 6.5
  resolution: 0.25 degree
  levels: 30
  TOA: 10 hPa
  physics:
    radiation:
      label: Lopez
      description: blah blah
      reference: Lopez (2002)
      reference-url: http://doi.org/XXXX
    convection:
      label: PCMT
      description: blah blah
      reference: Smith et al. (2020)
      reference-url: http://doi.org/XXXX
ocean:
  label: ORCA 5.2
  resolution: 0.25 degree
  levels: 40
land:
  label: ORCHIDEE 7
  resolution: 1/12 degree
  levels: 10
---

Intro on the coupled model. 
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Atmosphere
Resolution: {{ page.atmosphere.resolution }}
Levels: {{ page.atmosphere.levels }}

Describe atmos component. 
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

### Physics

<table>
  <thead>
    <tr>
      <th>Physics</th>
      <th>Scheme</th>
      <th>Details</th>
      <th>Reference</th>
    </tr>
  </thead>
  <tbody>
    {% for phys in page.atmosphere.physics %}
    <tr>
      <td>{{ phys | first }}</td>
      <td>{{ phys[1].label }}</td>
      <td>{{ phys[1].description }}</td>
      <td><a href="{{ phys[1].reference-url }}">{{ phys[1].reference }}</a></td>
    </tr>
    {% endfor %}
  </tbody>
</table>

## Ocean
Resolution: {{ page.ocean.resolution }}
Levels: {{ page.ocean.levels }}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Land
Resolution: {{ page.land.resolution }}
Levels: {{ page.land.levels }}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
