---
lang: us
ref: VDM-move2cloud

title: Migration move2cloud - Ville de Marseille
type: project
client: VDM
job: Architecte Big Data 
date_start: 2021-11-01
date_end: 2023-07-01
description: Implementation of a sovereign data platform on OVH cloud
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
# My mission

Implementation of a sovereign data platform on OVH cloud
- Automated deployment of BigData platforms via GitOps processes (Gitlab + ArgoCD)
- Framework for network and security needs


Iso-functional migration of a BigData/IA application on public tranquility (MPulse)
- Switching data between old and new system
- Recovery and slight technical overhaul of spark jobs
- Performance test and Debug of slowness
- Portability of data security rules

# Examples of my work
{% capture folder_path %}/assets/images/customer/{{ page.ref }}{% endcapture %}
{% include image-gallery.html folder=folder_path %}

# Technical environnement
MinIO, ClickHouse, Spark, Superset, Keycloack, ArgoCD, Gitlab