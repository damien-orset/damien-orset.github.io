---
lang: es
ref: VDM-move2cloud

title: migración move2cloud - Ciudad de Marsella
type: project
client: VDM
job: Arquitecto de Big Data 
date_start: 2021-11-01
date_end: 2023-07-01
description: Creación de una plataforma de datos soberana en la nube de OVH
technos:
  - Kubernetes
  - MinIO
  - ClickHouse
  - Spark
  - Superset
  - Keycloak
  - ArgoCD
  - Gitlab
---
# Mi misión

Implementación de una plataforma de datos soberanos en la nube de OVH
- Despliegue automatizado de plataformas BigData vía procesos GitOps (Gitlab + ArgoCD)
- Enmarcar las necesidades de red y seguridad.


Migración isofuncional de una aplicación BigData/AI sobre la paz pública (MPulse)
- Cambiar datos entre el sistema antiguo y el nuevo
- Reanudación y revisión técnica ligera de los trabajos de spark.
- Prueba de rendimiento y Debug de lentitud.
- Portabilidad de las reglas de seguridad de los datos.

# Ejemplos de producciones
{% capture folder_path %}/assets/images/customer/{{ page.ref }}{% endcapture %}
{% include image-gallery.html folder=folder_path %}

# Entorno técnico
MinIO, ClickHouse, Spark, Superset, Keycloack, ArgoCD, Gitlab