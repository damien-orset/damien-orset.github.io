---
lang: fr
ref: SNCF-surete

title: SNCF Surete
type: project
client: SNCF
job: Expert IA
date_start: 2021-04-01
date_end: 2021-07-31
description: Mise en place d’une architecture de POC pour de la video intelligence sur une 30aine de caméras
technos:
  - Ipsotek
  - Genetec
---
# Ma mission

Mise en place d’une architecture de POC pour de la video intelligence sur une 30aine de caméras
- Detection d’intrusions : personnes sur des rails, intrusion dans des zones réservées au personnel
- Comptage de foule : détection lorsqu’un seuil de densité est dépassé
Définition des règles dans le moteur Ipsotek.
Transmission des alarmes vers le VMS Genetec.

# Exemples de productions
{% capture folder_path %}/assets/images/customer/{{ page.ref }}{% endcapture %}
{% include image-gallery.html folder=folder_path %}

# Environnement technique
Ipsotek VISuite, PowerEdge, Genetec