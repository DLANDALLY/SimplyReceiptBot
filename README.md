<p align="center">
  <img 
    width="200" 
    alt="simplyReceiptBot" 
    src="https://github.com/user-attachments/assets/7591ab2f-3556-467b-9d41-e442191d215a" />
</p>

# Simply Receipt Bot

Un système automatisé de gestion des notes de frais via **Telegram** combinant OCR et IA générative — conçu pour les **indépendants, TPE et PME**.

[![Java Version](https://img.shields.io/badge/Java-21-brightgreen)](https://www.oracle.com/java/)

---

<p align="center">
  <img src="https://github.com/user-attachments/assets/3e7e32fa-175a-416e-bbdb-a55ae27b1af5" width="250"/>
</p>




## 🚀 Aperçu

Simply Receipt Bot permet à l’utilisateur de **prendre une photo de son ticket de caisse via Telegram**, d’en extraire automatiquement les données importantes (montant, date, taxes, fournisseur), de les analyser grâce à l’IA, puis de les valider avant un **envoi automatique par email** aux contacts comptables configurés (comptable, entreprise, utilisateur).

Cette solution réduit significativement le temps consacré à la saisie des notes de frais, minimise les erreurs humaines et s’intègre dans le workflow quotidien de l’utilisateur via une interface simple — **sans application supplémentaire à installer**.

---

## 📌 Fonctionnalités principales

### 📍 Interaction utilisateur
- 📸 Capture des tickets de caisse directement via Telegram
- 🔄 Workflow simple : réception → extraction → validation → envoi

### 🤖 Traitement automatique
- 🔍 Extraction OCR des informations clés du ticket
- 🧠 Structuration et analyse via IA générative
- ✅ Confirmation utilisateur avant traitement final

### 📤 Communication & contacts
- 📧 Envoi automatique des notes de frais par email
- 👥 Gestion des contacts comptables (comptable, entreprise, utilisateur)

### 📊 Architecture extensible
- 🧱 Conception microservices prête pour :
  - Archivage sécurisé
  - Reporting et statistiques
  - Export comptable (CSV/PDF)

---

## 🧠 Valeur apportée

- ⏱ **Réduction du temps administratif** lié aux notes de frais  
- ❌ **Diminution des erreurs de saisie manuelle**  
- 📱 Utilisation d’un canal **connu et accessible (Telegram)**  
- 🔁 **Automatisation complète** du processus métier  
- 🧩 Solution légère adaptée à des structures sans outils complexes

---

## 🧱 Architecture technique

Le projet repose sur une **architecture microservices**, favorisant la séparation des responsabilités, la scalabilité et la maintenabilité.

```mermaid
graph TD
    A[Utilisateur Telegram] --> B[Telegram Bot API]
    B --> C[ms-telegram-bot]
    C --> D[ms-ocr]
    C --> E[ms-ai-resume]
    E --> F[Validation utilisateur]
    F --> G[Service Email]
    G --> H[Contacts comptables]
```


