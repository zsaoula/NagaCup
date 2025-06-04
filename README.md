# 🏆 NagaCup

La **NagaCup** est un événement compétitif sur Minecraft organisé depuis plusieurs années par le streamer Nagatow.  
Ce dépôt contient l'application web officielle de la compétition.

👉 Le site est accessible ici : [https://nagacup.fr](https://nagacup.fr)

## ⚙️ Stack technique

Cette application web est développée à l’aide de technologies modernes :

<table>
  <tr>
    <td><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angular/angular-original.svg" width="40" /></td>
    <td><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg" width="40" /></td>
    <td><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nginx/nginx-original.svg" width="40" /></td>
    <td><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="40" /></td>
  </tr>
</table>


## 🚀 Fonctionnalités

- **Interface responsive** : Interfaces utilisateur réactive, fluide et responsive  
- **Déploiement simplifié** : Configuration Docker et Nginx pour une mise en production efficace.
- **Proxy de développement** : Facilite les appels API durant le développement.
- **Structure modulaire** : Organisation du code facilitant la maintenance et l'évolution du projet.
- **Intégration d'API REST** : L'application interagit avec des API REST pour récupérer et afficher dynamiquement les données relatives aux compétitions, aux participants et aux résultats.

## 🛠️ Installation et développement

### Prérequis

- Node.js et npm installés  
- Angular CLI (v18.2.7 recommandé)

### Installation

```bash
git clone https://github.com/zsaoula/NagaCup.git
cd NagaCup
npm install
```

### Lancer le serveur de développement

```bash
ng serve
```

L'application sera accessible à l'adresse `http://localhost:4200/` et se rechargera automatiquement à chaque modification.

## 📦 Déploiement

Le projet contient :
- Un `Dockerfile` pour builder l’image de l’application Angular
- Un fichier `nginx.conf` pour servir l’application en production

### Exemple rapide de build Docker :

```bash
docker build -t nagacup .
docker run -d -p 80:80 nagacup
```
