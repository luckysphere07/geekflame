---
title: "Home Assistant : premiers contrôles après une panne Zigbee2MQTT"
description: "Checklist pour diagnostiquer un réseau Zigbee2MQTT indisponible, sans réinitialiser tout le réseau."
date: 2026-11-20
draft: true
translationKey: zigbee2mqtt-first-checks
slug: "home-assistant-zigbee2mqtt-diagnostic"
categories: ["Domotique"]
---
> **Brouillon éditorial :** à tester sur une installation de laboratoire avant publication.

## 1. Observer avant de modifier

Vérifier si le problème touche un seul appareil ou l'ensemble du réseau. Consulter les logs de Zigbee2MQTT et l'état de son broker MQTT.

## 2. Contrôler l'adaptateur

Vérifier que la clé Zigbee est toujours détectée par le système, que le chemin série n'a pas changé et qu'aucun autre service ne monopolise le périphérique.

## 3. Vérifier sans tout réinitialiser

Faire une sauvegarde de la configuration avant tout changement. Éviter d'effacer la base Zigbee ou de réappairer tous les appareils sans diagnostic.

## 4. Valider

Observer la reconnexion des équipements, les messages MQTT et l'état de Home Assistant. Documenter la cause avant de conclure.
