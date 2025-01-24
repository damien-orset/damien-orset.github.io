---
lang: es
ref: SNCF-surete

title: SNCF Süréte
type: project
client: SNCF
job: experto en IA
date_start: 2021-04-01
date_end: 2021-07-31
description: Implementación de una arquitectura POC para videointeligencia en alrededor de 30 cámaras
technos:
  - Ipsotek
  - Genetec
---
# Mi misión

Implementación de una arquitectura POC para videointeligencia en unas 30 cámaras
- Detección de intrusiones: personas sobre raíles, intrusión en zonas reservadas al personal
- Recuento de multitudes: detección cuando se supera un umbral de densidad
Definición de reglas en el motor Ipsotek.
Transmisión de alarmas al VMS de Genetec.

# Ejemplos de producciones
{% capture folder_path %}/assets/images/customer/{{ page.ref }}{% endcapture %}
{% include image-gallery.html folder=folder_path %}

# Entorno técnico
Ipsotek VISuite, PowerEdge, Genetec