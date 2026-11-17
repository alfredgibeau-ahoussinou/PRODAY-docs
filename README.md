<div align="center">

<img src="./.github/hero-banner.svg" alt="ProDay — L'infrastructure du football moderne" width="100%" />

<br/><br/>

[![Site Web](https://img.shields.io/badge/Site-proday75.fr-C5A059?style=for-the-badge&logo=googlechrome&logoColor=090D16)](https://proday75.fr)
[![Bêta iOS & Android](https://img.shields.io/badge/Bêta-iOS%20%26%20Android-10B981?style=for-the-badge&logo=apple&logoColor=white)](https://proday75.fr/beta/inscription)
[![Tarifs Clubs](https://img.shields.io/badge/Tarifs-Clubs%20Amateurs-090D16?style=for-the-badge)](https://proday75.fr/tarifs)
[![Issues](https://img.shields.io/badge/Feedback-Ouvrir%20une%20Issue-38BDF8?style=for-the-badge&logo=github&logoColor=white)](../../issues/new/choose)

</div>

---

## ⚡ Une seule donnée football, trois pôles connectés

**ProDay** remplace les groupes WhatsApp éparpillés et les tableaux Excel par une infrastructure unifiée :

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>🏛️ Pôle Club</h3>
      <p><strong>Présidents & Secrétaires</strong></p>
      <ul>
        <li>Import & suivi des licences FFF</li>
        <li>Cotisations & certificats médicaux</li>
        <li>Planning des terrains & vestiaires</li>
        <li>Effectifs U7 à Seniors</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <h3>📋 Pôle Coach</h3>
      <p><strong>Entraîneurs & Éducateurs</strong></p>
      <ul>
        <li>Tableau tactique & séances</li>
        <li>Convocations en 1 clic</li>
        <li>Feuilles de match & présences</li>
        <li>Suivi du temps de jeu</li>
      </ul>
    </td>
    <td width="33%" valign="top">
      <h3>🌍 Pôle Community</h3>
      <p><strong>Joueurs, Parents & Supporters</strong></p>
      <ul>
        <li>Convocations & réponses directes</li>
        <li>Covoiturage entre familles</li>
        <li>Scores en direct le week-end</li>
        <li>Carte & passeport joueur <em>(100 % gratuit)</em></li>
      </ul>
    </td>
  </tr>
</table>

---

## 🏗️ Architecture Multi-Dépôts

```mermaid
flowchart LR
    Docs["🌍 PRODAY-docs (Public)<br/>Docs · Roadmap · Issues · Releases"]
    App["🔒 proday-app (Privé)<br/>Expo React Native · iOS & Android"]
    Back["🔒 proday-backend (Privé)<br/>Firebase Functions · Firestore · Workers FFF"]
    Web["🔒 proday-website (Privé)<br/>Next.js 16 · proday75.fr"]

    Docs -.->|Releases & Feedback| App
    App <-->|API & Realtime| Back
    Web <-->|Waitlist & Admin| Back
```

| Dépôt | Visibilité | Rôle |
| :--- | :---: | :--- |
| **[`PRODAY-docs`](https://github.com/alfredgibeau-ahoussinou/PRODAY-docs)** | 🌍 Public | Vitrine technique, documentation publique, roadmap, changelog & suivi des retours. |
| **`proday-app`** | 🔒 Privé | Application mobile & web Expo React Native + TypeScript. |
| **`proday-backend`** | 🔒 Privé | Cloud Functions Node 22, règles Firestore/Storage et workers FFF. |
| **`proday-website`** | 🔒 Privé | Site vitrine `proday75.fr` et Control Center interne. |

---

## 📚 Documentation & Retours

<details>
<summary><strong>📂 Explorer les documents publics du dépôt</strong></summary>

* [`ARCHITECTURE.md`](./ARCHITECTURE.md) — Stack technique et principes de conception.
* [`ROADMAP.md`](./ROADMAP.md) — Fonctionnalités livrées et chantiers en cours.
* [`CHANGELOG.md`](./CHANGELOG.md) — Historique des versions (`v1.0.10`).
* [`SECURITY.md`](./SECURITY.md) — Politique de divulgation responsable.
* [`LICENSE`](./LICENSE) & [`COPYRIGHT.md`](./COPYRIGHT.md) — Mentions de propriété intellectuelle.

</details>

<div align="center">
  <br/>
  <img src="./.github/wave-footer.svg" alt="ProDay Footer" width="100%" />
</div>
