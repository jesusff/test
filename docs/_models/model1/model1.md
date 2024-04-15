---
layout: model
label: Model 1
label-extended: My model 1 extended label
source-id: Model1
atmosphere:
  label: ALADIN 6.5
  resolution: 0.25 degree
  levels: 30
ocean:
  label: ORCA 5.2
  resolution: 0.25 degree
  levels: 40
land:
  label: ORCHIDEE 7
  resolution: 1/12 degree
  levels: 10
---

Intro on the coupled model

## Atmosphere
Resolution: {{ page.atmosphere.resolution }}
Levels: {{ page.atmosphere.levels }}

Describe atmos

## Ocean
Resolution: {{ page.ocean.resolution }}
Levels: {{ page.ocean.levels }}

## Land
Resolution: {{ page.land.resolution }}
Levels: {{ page.land.levels }}

