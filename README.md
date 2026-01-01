<div align="center">

# 🚀 Flask App – Dockerized

### _Simple • Clean • Production Ready_

![Docker](https://img.shields.io/badge/Docker-Ready-blue?logo=docker)
![Python](https://img.shields.io/badge/Python-3.9-yellow?logo=python)
![Flask](https://img.shields.io/badge/Flask-App-black?logo=flask)
![Status](https://img.shields.io/badge/Status-Stable-success)
![License](https://img.shields.io/badge/License-MIT-green)

</div>

---

## 🌍 Présentation

**Flask App – Dockerized** est une application Flask légère, entièrement conteneurisée avec Docker.  
Elle est conçue pour servir de **base solide** pour :
- APIs REST
- microservices
- prototypes rapides
- déploiements cloud

> 💡 *Build once, run anywhere.*

---

## 🧠 Pourquoi ce projet ?

✅ Environnement reproductible  
✅ Déploiement rapide  
✅ Zéro configuration locale  
✅ Compatible **Docker Hub / Cloud / VPS**

---

## 🛠️ Stack technique

| Technologie | Description |
|------------|------------|
| 🐍 Python | Langage principal |
| 🌶️ Flask | Framework web |
| 🐳 Docker | Conteneurisation |
| ☁️ Docker Hub | Registry d’images |

---

## 📁 Structure du projet


.
├── Dockerfile
├── requirements.txt
├── app.py
└── docker-compose.yml

## 🐋 Dockerfile
FROM python:3.9-slim

WORKDIR /app
COPY requirements.txt .
COPY app.py .
RUN pip install -r requirements.txt

EXPOSE 5000
CMD ["python", "app.py"]

## ⚙️ Build de l’image Docker
docker build -t app_flask .

## 🔐 Connexion à Docker Hub
docker login

## 🏷️ Tag de l’image
docker tag app_flask hackira66/app_flask:1.0


### ⚠️ Le username Docker Hub doit être en minuscules.

## 📤 Push vers Docker Hub
docker push hackira66/app_flask:1.0


## ✅ Image publiée avec succès 🎉

## 📥 Pull & Run (n’importe où)
docker pull hackira66/app_flask:1.0
docker run -p 5000:5000 hackira66/app_flask:1.0


## 🌐 Accès :

http://localhost:5000

## 🧪 Lancer avec Docker Compose
docker compose up --build

## 📈 Bonnes pratiques intégrées

✔️ Image légère (python:slim)

✔️ Versioning (1.0, latest)

✔️ Prêt pour CI/CD

✔️ Structure scalable

## 🚀 Roadmap (idées)

CI/CD GitHub Actions → Docker Hub

Multi-stage build

Support FastAPI

Déploiement cloud (Render / AWS / Railway)

## 👨🏽‍💻 Auteur

Hackira Tech
🚀 Ingénierie logicielle & systèmes d’information
💡 Cloud • DevOps • IA • Web & Mobile

🔗 Building impactful tech solutions

📜 Licence

Ce projet est sous licence MIT.
Libre d’utilisation, de modification et de distribution.

<div align="center">

✨ Si ce projet t’aide, pense à laisser une ⭐ sur GitHub ! ✨

</div> ```

```bash# app_flask_dockerized
