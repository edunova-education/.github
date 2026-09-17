
# Edunova — Infrastructure Scolaire Numérique B2B

> La plateforme pédagogique interactive en marque blanche pour les collèges et lycées en Afrique.

🌐 **Site officiel** : [https://edunova.cm](https://edunova.cm)  
🎯 **Démonstration active** : [https://demo.edunova.cm](https://demo.edunova.cm)  
📧 **Contact partenariats** : contact@edunova.cm

---

## 🏛️ Vision & Mission
Edunova permet aux établissements scolaires du secondaire de déployer leur propre environnement numérique de travail sans investissement matériel lourd. Notre coeur de mission : garantir la continuité pédagogique et les révisions même dans les zones à faible connectivité Internet.

## ⚙️ Architecture Système & Choix Techniques

Edunova est conçu selon une architecture moderne, découplée et résiliente :

- **Multi-Tenant White-Label** : Chaque établissement bénéficie de son sous-domaine isolé (`[ecole].edunova.cm`) avec sa propre identité visuelle.
- **Résilience Offline-First** : Utilisation d'un Service Worker sur-mesure couplé à **IndexedDB** pour permettre aux élèves de s'exercer et réviser en mode avion sans connexion.
- **Synchronisation Silencieuse (*Ghost Sync*)** : Ingestion asynchrone des devoirs hors-ligne dès le retour d'une connexion réseau.
- **Stack Technologique** :
  - Backend : NestJS, GraphQL API, Prisma ORM, BullMQ (tâches de fond), Redis.
  - Frontend : Next.js 16 (App Router), React, Tailwind CSS.
  - Administration : React, Vite.
  - Données & Stockage : PostgreSQL, S3/Cloudflare R2, Docker.

---
© Edunova Education — Tous droits réservés.
