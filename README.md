### Diffusion de Données en Temps Réel | Projet d'Ingénierie des Données de Bout en Bout

---

#### Table des Matières
1. Introduction  
2. Architecture du Système  
3. Ce Que Vous Allez Apprendre  
4. Technologies  
5. Commencer  
6. Regardez le Tutoriel Vidéo  

---

### Introduction

Ce projet est un guide complet pour construire un pipeline d'ingénierie des données de bout en bout. Il couvre chaque étape, de l'ingestion des données au traitement, et enfin au stockage, en utilisant une pile technologique robuste comprenant **Apache Airflow**, **Python**, **Apache Kafka**, **Apache Zookeeper**, **Apache Spark**, et **Cassandra**. L'ensemble est conteneurisé avec **Docker** pour une facilité de déploiement et une grande scalabilité.

---

### Architecture du Système
![Data engineering architecture](https://github.com/user-attachments/assets/55045241-3be8-439c-91de-3f03d61f11e7)

#### Architecture du Système

Le projet est conçu avec les composants suivants :

- **Source de Données** : Nous utilisons l'API [randomuser.me](https://randomuser.me) pour générer des données d'utilisateur aléatoires pour notre pipeline.  
- **Apache Airflow** : Responsable de l'orchestration du pipeline et du stockage des données récupérées dans une base de données PostgreSQL.  
- **Apache Kafka et Zookeeper** : Utilisés pour le streaming des données de PostgreSQL vers le moteur de traitement.  
- **Centre de Contrôle et Registre de Schéma** : Aide à la surveillance et à la gestion des schémas de nos flux Kafka.  
- **Apache Spark** : Pour le traitement des données via ses nœuds master et worker.  
- **Cassandra** : Où les données traitées seront stockées.  

---

### Ce Que Vous Allez Apprendre

- Mettre en place un pipeline de données avec **Apache Airflow**  
- Diffusion de données en temps réel avec **Apache Kafka**  
- Synchronisation distribuée avec **Apache Zookeeper**  
- Techniques de traitement des données avec **Apache Spark**  
- Solutions de stockage de données avec **Cassandra** et **PostgreSQL**  
- Conteneurisation de l'ensemble de votre configuration d'ingénierie des données avec **Docker**  

---

### Technologies

- **Apache Airflow**  
- **Python**  
- **Apache Kafka**  
- **Apache Zookeeper**  
- **Apache Spark**  
- **Cassandra**  
- **PostgreSQL**  
- **Docker**  

---

### Commencer

1. Clonez le dépôt :  
   ```bash
   git clone https://github.com/airscholar/e2e-data-engineering.git
   ```
2. Accédez au répertoire du projet :  
   ```bash
   cd e2e-data-engineering
   ```
3. Lancez Docker Compose pour démarrer les services :  
   ```bash
   docker-compose up
   ```  
