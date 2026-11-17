# ⚽ ProDay — L'infrastructure du football moderne

[![Site Web](https://img.shields.io/badge/Site-proday75.fr-C5A059?style=for-the-badge)](https://proday75.fr)
[![Bêta](https://img.shields.io/badge/Bêta-iOS%20%26%20Android-10B981?style=for-the-badge)](https://proday75.fr/beta/inscription)
[![Version](https://img.shields.io/badge/App-v1.0.10-090D16?style=for-the-badge)](./CHANGELOG.md)

**ProDay** réunit **3 pôles métiers** autour d'une donnée sportive unique pour les clubs de football :

| Pôle | Pour qui ? | Ce qu'il fait |
| :--- | :--- | :--- |
| **Club** | Présidents, Secrétaires, Direction | Licences FFF, cotisations, effectifs U7 à Seniors, créneaux de terrains & certificats médicaux. |
| **Coach** | Entraîneurs & Éducateurs | Tableau tactique, préparation de séances, convocations 1 clic, suivi des présences & temps de jeu. |
| **Community** | Joueurs, Parents & Supporters | Convocations, covoiturage entre familles, scores en direct, carte & passeport joueur (100 % gratuit). |

---

## 🏗 Architecture Multi-Dépôts

Pour garantir la sécurité de la propriété intellectuelle et des données utilisateurs tout en gardant un espace ouvert pour la communauté :

| Dépôt | Visibilité | Rôle |
| :--- | :--- | :--- |
| **`PRODAY-docs`** *(ce dépôt)* | 🌍 **Public** | Vitrine technique, documentation publique, roadmap, changelog, signalement de bugs & releases bêta. |
| **`proday-app`** | 🔒 **Privé** | Application mobile & web (Expo React Native + TypeScript). |
| **`proday-backend`** | 🔒 **Privé** | Firebase Cloud Functions, règles Firestore/Storage et workers de synchronisation FFF. |
| **`proday-website`** | 🔒 **Privé** | Site vitrine `proday75.fr` et Control Center interne (Next.js 16 + Tailwind CSS v4). |

---

## 🔗 Liens utiles

* **Site officiel** : [proday75.fr](https://proday75.fr)
* **Programme Bêta (iOS TestFlight & Android)** : [proday75.fr/beta](https://proday75.fr/beta)
* **Tarifs clubs** : [proday75.fr/tarifs](https://proday75.fr/tarifs)
* **Signaler un bug / Proposer une idée** : [Ouvrir une Issue](../../issues/new/choose)
* **Sécurité** : Voir [SECURITY.md](./SECURITY.md)

---

© ProDay · Voir [LICENSE](./LICENSE) et [COPYRIGHT.md](./COPYRIGHT.md).
