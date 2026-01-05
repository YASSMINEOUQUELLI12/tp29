# TP 29 : RabbitMQ (Management) avec Docker + Exchange/Queue/Binding + Publish/Consume


## 🎯 Objectif

Mettre en place **RabbitMQ via Docker**, puis manipuler l’interface Web pour :

- créer un **exchange**
- créer une **queue**
- réaliser un **binding**
- publier un **message**
- lire les messages depuis la queue

---

## ✅ Prérequis

- Docker installé  
  (Docker Desktop – Windows | Docker Engine – Linux)
- Accès Internet (téléchargement de l’image)
- Navigateur Web (Chrome, Firefox, …)

---
<img width="1912" height="872" alt="Capture d’écran 2025-12-23 143610" src="https://github.com/user-attachments/assets/2b14fc76-25d6-4ab9-a532-dfbe1a15641f" />
<img width="1918" height="873" alt="image" src="https://github.com/user-attachments/assets/3b75f33d-6cbb-4d20-bce4-f17b47a6ae32" />
## 1️⃣ Lancer RabbitMQ avec Docker

Télécharger et démarrer RabbitMQ (avec l’interface Web activée) :

```bash
docker run -d --name rabbitmq \
  -p 5672:5672 \
  -p 15672:15672 \
  rabbitmq:3-management


