---
layout: default
source-id: Model1
label: Model 1
extended_label: My model 1 extended label
description: A description of Model 1
atmosphere:
  resolution: 1 degree
  levels: 30
ocean:
  resolution: 0.5 degree
  levels: 40
land:
  resolution: 0.25 degree
  levels: 20
---

# Model 1

## Atmosphere
Resolution: {{ page.atmosphere.resolution }}
Levels: {{ page.atmosphere.levels }}

## Ocean
Resolution: {{ page.ocean.resolution }}
Levels: {{ page.ocean.levels }}

## Land
Resolution: {{ page.land.resolution }}
Levels: {{ page.land.levels }}

