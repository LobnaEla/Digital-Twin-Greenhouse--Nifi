# 🌱 Digital Twin - Surveillance de Température dans une Serre Agricole

Ce projet simule un **jumeau numérique (Digital Twin)** d’une serre connectée.  
Il permet de collecter, traiter et visualiser les données de **température** et **humidité** issues de capteurs simulés.

## 🧠 Contexte

L’agriculture moderne repose de plus en plus sur des capteurs pour optimiser les conditions de croissance.  
Ce projet vise à reproduire ces conditions dans un environnement numérique afin de :
- **Surveiller** en temps réel la température et l’humidité
- **Détecter** les alertes (ex : température trop élevée)
- **Analyser** l’évolution historique via dashboards

---

## 🔧 Technologies utilisées

- **Apache NiFi** → Orchestration et traitement des flux de données
- **Python** → Simulateur de capteurs (données JSON toutes les 10s)
- **InfluxDB** → Base de données time-series
- **Grafana** → Visualisation des données

---

## 🔢 Modèle de données JSON

Les données générées par le capteur ont la forme suivante :

```json
{
  "deviceId": "sensor-001",
  "timestamp": "2025-05-06T10:00:00Z",
  "temperature": 28.6,
  "humidity": 60.2
}
