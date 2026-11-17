# Architecture Technique (Vue Publique)

## Stack principale

* **Mobile & Web App (`proday-app`)** : Expo 54 · React Native · TypeScript · React Navigation.
* **Backend & Données (`proday-backend`)** : Firebase Auth · Cloud Firestore · Cloud Storage · Cloud Functions (Node 22, `europe-west1`).
* **Site Vitrine & Admin (`proday-website`)** : Next.js 16 (App Router) · React 19 · Tailwind CSS v4 · Netlify.
* **E-mails transactionnels** : Brevo API v3.
* **Synchronisation sportive** : Workers dédiés pour l'import et la mise à jour des compétitions, classements et licenciés FFF.

## Principes de conception

1. **Source de vérité unique** : une convocation créée par un coach met à jour instantanément la feuille de match du club, la notification du joueur et l'agenda du parent.
2. **Séparation stricte Public / Privé** : aucune clé API, aucun fichier `.env`, aucun certificat et aucune donnée club ne transitent par ce dépôt public.
3. **Conformité mineurs & RGPD** : gestion dédiée des comptes mineurs, du droit à l'image et de l'export des données.
