---
source-id: model2A
label: Model2 A
label-extended: Model 2 title
atmosphere:
  label: WRF v3.8.1
  resolution: 1 degree
  levels: 30
  TOA: 20 hPa
  physics:
    radiation:
      label: Myrad 7.1
      description: blah blah
      reference: Lopez (2002)
      reference-url: http://doi.org/XXXX
    convection:
      label: Kain-Fritsch
      description: Mass flux scheme with ...
      reference: Kain et al. (2009)
      reference-url: http://doi.org/XXXX
    microphysics:
      label: WSM5

ocean:
  label: NEMO v12.4
  resolution: 0.5 degree
  levels: 40
land:
  label: CLM 4.8
  resolution: 0.25 degree
  levels: 20
---

## Atmosphere
Resolution: {{ page.atmosphere.resolution }}
Levels: {{ page.atmosphere.levels }}

{% include physics-atm.html name=page.name %}

## Ocean
Resolution: {{ page.ocean.resolution }}
Levels: {{ page.ocean.levels }}

## Land
Resolution: {{ page.land.resolution }}
Levels: {{ page.land.levels }}

