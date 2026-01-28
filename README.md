# 🎓 UBO Gestion - ADM Project

Bienvenue sur le projet **UBO Gestion**.
Ceci est une application Fullstack micro-services pour la gestion universitaire (Enseignants, Étudiants, Promotions, Formations), orchestrée via Docker.

## 📂 Architecture & Dépôts

Le projet est modulaire et divisé en 4 dépôts distincts :

| Module | Description | Lien GitHub |
| :--- | :--- | :--- |
| **🏗️ Infrastructure** | **(Point d'entrée)** Orchestration Docker & Nginx | [Voir le dépôt](https://github.com/ADM-Project/Infrastracture) |
| **💻 Frontend** | Interface Utilisateur (Vue.js 3 + Vite) | [Voir le dépôt](https://github.com/ADM-Project/Frontend) |
| **☕ Backend** | API RESTful (Jakarta EE + Wildfly 30) | [Voir le dépôt](https://github.com/ADM-Project/Backend) |
| **🗄️ BDD** | Scripts d'initialisation Oracle Database | [Voir le dépôt](https://github.com/ADM-Project/BDD) |

---

## 🚀 Guide d'Installation (Quick Start)

Pour faire fonctionner le projet, nous allons créer un dossier racine, y cloner tous les modules, puis lancer l'orchestrateur.

### 1. Prérequis
* **Docker** & **Docker Compose** (Installés et en cours d'exécution).
* **Git** (Installé).

### 2. Script d'Installation
Ouvrez votre terminal et copiez/collez l'ensemble des commandes ci-dessous :

```bash
# 1. Création du dossier racine du projet
mkdir ADM-Project
cd ADM-Project

# 2. Clonage des 4 modules (Frontend, Backend, BDD, Infra)
git clone [https://github.com/ADM-Project/Infrastracture.git](https://github.com/ADM-Project/Infrastracture.git)
git clone [https://github.com/ADM-Project/Frontend.git](https://github.com/ADM-Project/Frontend.git)
git clone [https://github.com/ADM-Project/Backend.git](https://github.com/ADM-Project/Backend.git)
git clone [https://github.com/ADM-Project/BDD.git](https://github.com/ADM-Project/BDD.git)

# 3. Déplacement dans le dossier d'infrastructure
cd Infrastracture

# 4. Lancement de l'environnement Docker
docker compose up -d --build
