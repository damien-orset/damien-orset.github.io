---
lang: fr
ref: VDM-move2cloud

title: Migration move2cloud - Ville de Marseille
type: project
client: VDM
job: Architecte Big Data 
date_start: 2021-11-01
date_end: 2023-07-01
description: Mise en place d’une plateforme souveraine de données sur cloud OVH
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
# Ma mission

Mise en place d’une plateforme souveraine de données sur cloud OVH
- Déploiement automatisé de plateformes BigData via des processus GitOps (Gitlab + ArgoCD)
- Cadrage besoin réseau et sécurité


Migration iso-fonctionnelle d’un applicatif BigData/IA sur la tranquillité publique (MPulse)
- Bascule des data entre ancien et nouveau système
- Reprise et refonte technique légère des jobs spark
- Test de performance et Debug des lenteurs
- Portabilité des règles de sécurité sur la data

# Exemples de productions
{% capture folder_path %}/assets/images/customer/{{ page.ref }}{% endcapture %}
{% include image-gallery.html folder=folder_path %}

# Environnement technique
MinIO, ClickHouse, Spark, Superset, Keycloack, ArgoCD, Gitlab