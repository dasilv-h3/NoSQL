# NoSQL & ELK - Exercices et Déploiements

Bienvenue dans ce repository regroupant plusieurs exercices et configurations pour les bases de données NoSQL ainsi que la stack ELK. Vous y trouverez des projets pour **Redis, MongoDB, Neo4j et ELK**, avec des fichiers de configuration et des guides d'installation pour chaque technologie.

## Contenu du repository

### **Redis**
- Concepts de base : clés, valeurs, types de données.
- Commandes essentielles : `SET`, `HSET`, `LPUT`, `SADD`, `ZADD`...
- Scripts d'initialisation.
- Fichier Docker pour le déploiement.

### **MongoDB**
- Introduction aux collections et documents.
- Requêtes CRUD avec MongoDB.
- Configuration et scripts d'exécution.

### **Neo4j**
- Modélisation des données en graphe.
- Langage Cypher : création et requêtes de graphes.
- Scripts d'exemples et configuration Docker.

### **ELK (Elasticsearch, Logstash, Kibana)**
- Déploiement de la stack ELK via Docker.
- Indexation et requêtes Elasticsearch.
- Analyse et visualisation des logs avec Kibana.

---

## Installation et Exécution
Chaque dossier contient un fichier **docker-compose.yml** pour faciliter le déploiement.

### Prérequis
- [Docker](https://www.docker.com/get-started) installé.
- [Python](https://www.python.org/downloads/) si vous utilisez les scripts d'interaction.

### 📦 Lancer un service spécifique
1. **Se positionner dans le bon dossier**
   ```sh
   cd redis  # ou mongo, neo4j, elk
   ```
2. **Démarrer le service**
   ```sh
   docker-compose up -d
   ```
3. **Accéder au service**
   - Redis : `redis-cli`
   - MongoDB : `mongo`
   - Neo4j : Accès via le navigateur à `http://localhost:7474`
   - Kibana : Accès via `http://localhost:5601`

### Arrêter les services
```sh
docker-compose down
```

