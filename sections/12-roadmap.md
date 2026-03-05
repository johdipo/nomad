# 12. Roadmap stratégique

La roadmap de Nomad suit une logique d'expansion concentrique : commencer par le cœur (marketplace de terrains privés), puis élargir l'écosystème (véhicules, services, infrastructure). Chaque phase est conditionnée par la validation de la précédente.

---

## 12.1 Vue d'ensemble

```
          Y0-Y1              Y1-Y3              Y3-Y5+
    ┌──────────────┐   ┌──────────────┐   ┌──────────────┐
    │   PHASE 1    │   │   PHASE 2    │   │   PHASE 3    │
    │    LIEUX     │──▶│  VÉHICULES   │──▶│ INFRASTRUCTURE│
    │              │   │              │   │              │
    │ Marketplace  │   │ Location P2P │   │ Écosystème   │
    │ terrains     │   │ de vans +    │   │ du voyage    │
    │ privés +     │   │ intégration  │   │ nature       │
    │ campings     │   │ spots+vans   │   │              │
    └──────────────┘   └──────────────┘   └──────────────┘
     CH → FR             + DACH              + 8 marchés
     200 → 2 500         2 500 → 8 000       8 000 → 20 000+
     terrains            terrains + vans     terrains + vans
                                              + services
```

---

## 12.2 Phase 1 — Lieux (Y0-Y1)

**Objectif :** Valider le product-market fit sur le marché francophone (CH romande + France).

### 12.2.1 Jalons clés

| Jalon | Timeline | Critère de succès |
|---|---|---|
| **MVP live** | M0 | App fonctionnelle : recherche, réservation, paiement, profils hôtes/voyageurs |
| **200 terrains onboardés** | M0 (pré-lancement) | Catalogue suffisant pour la Romandie |
| **Première réservation** | M0+1 semaine | Preuve de concept transactionnelle |
| **100 réservations** | M3 | Validation de la demande |
| **NPS voyageur > 40** | M3 | Satisfaction utilisateur |
| **400 terrains** | M6 | Expansion début France (sud-est) |
| **1 000 réservations cumulées** | M6 | Traction significative |
| **Lancement France** | M6-M8 | Provence, Occitanie, Auvergne-Rhône-Alpes |
| **1 200 terrains** | M12 | CH + FR consolidés |
| **Breakeven unitaire** | M12 | Revenu/réservation > coût variable/réservation |

### 12.2.2 Fonctionnalités MVP (M0)

**Inclus dans le MVP :**
- Recherche par carte + filtres (localisation, dates, prix, équipements)
- Profil terrain (photos, description, équipements, règles, prix)
- Réservation en ligne avec paiement sécurisé (Stripe)
- Messagerie hôte-voyageur
- Système d'avis post-séjour
- Profil hôte avec calendrier de disponibilité
- Dashboard hôte basique (réservations, revenus, calendrier)
- Responsive web app (mobile-first)

**Exclu du MVP (reporté) :**
- App native iOS/Android (web app suffisante pour valider)
- Pricing dynamique / IA
- Campings classiques (terrains privés uniquement au départ)
- Forfait Premium hôtes
- Mise en avant payante (Ads)
- Location de véhicules
- Multi-langue (français uniquement)

### 12.2.3 Stack technique recommandé

| Composant | Choix | Justification |
|---|---|---|
| Frontend | React / Next.js (PWA) | Mobile-first, SEO, pas besoin d'app native au départ |
| Backend | Node.js / Python | Rapidité de développement, écosystème riche |
| Base de données | PostgreSQL + PostGIS | Requêtes géospatiales (recherche par proximité) |
| Paiement | Stripe Connect | Marketplace multi-vendeurs, escrow natif, onboarding hôte simplifié |
| Hébergement | Vercel / Railway + AWS S3 | Coût faible, scaling automatique |
| Maps | Mapbox ou MapTiler | Cartes personnalisables, pricing startup-friendly |

**Estimation développement MVP :** 2-3 mois pour un développeur senior full-stack, ou 6-8 semaines avec une équipe de 2.

---

## 12.3 Phase 2 — Véhicules (Y1-Y3)

**Objectif :** Ajouter la location de vans/camping-cars P2P pour capturer une part plus grande du panier voyageur et créer un écosystème intégré (spot + véhicule en un parcours).

### 12.3.1 Condition d'activation

Phase 2 ne démarre que si Phase 1 valide :
- ✅ >1 000 terrains actifs
- ✅ >5 000 réservations cumulées
- ✅ NPS voyageur > 45
- ✅ Unit economics positifs (revenu/réservation > coût variable)
- ✅ Seed round bouclé (~500K-1M €)

### 12.3.2 Jalons clés

| Jalon | Timeline | Critère |
|---|---|---|
| **Module véhicules live** | M14-M16 | Location P2P de vans intégrée |
| **100 véhicules listés** | M18 | Offre initiale (CH + FR) |
| **Parcours intégré spot+van** | M18 | Un voyageur peut réserver terrain + van dans le même flux |
| **Expansion DACH** | M18-M24 | Lancement Allemagne, Autriche (en allemand) |
| **5 000 terrains** | M24 | Consolidation multi-marchés |
| **Premier partenariat location fleet** | M24 | Accord avec un loueur type Indie Campers pour l'inventaire de départ |

### 12.3.3 Modèle véhicules

- **P2P** : propriétaires de vans sous-utilisés (comme Yescapa/Goboony)
- **Commission** : 10-12 % (panier moyen 80-200 €/jour → revenu 8-24 €/jour)
- **Assurance** : partenariat avec assureur spécialisé (obligatoire pour la location)
- **Différenciation vs Yescapa** : l'intégration spot+van est unique — personne ne propose un parcours "choisis ton spot, loue ton van, pars"

---

## 12.4 Phase 3 — Infrastructure du voyage nature (Y3-Y5+)

**Objectif :** Devenir la plateforme de référence pour tout le voyage nature en Europe — pas seulement la réservation, mais l'écosystème complet.

### 12.4.1 Condition d'activation

- ✅ >8 000 terrains actifs sur 5+ marchés
- ✅ >500 véhicules listés
- ✅ Breakeven opérationnel atteint
- ✅ Série A bouclée (2-5M €) si scaling accéléré

### 12.4.2 Extensions possibles

| Extension | Description | Revenu potentiel |
|---|---|---|
| **Équipement** | Location de matériel camping (tentes, réchauds, sacs de couchage) en point relais ou livraison sur spot | Commission 15-20 % |
| **Expériences** | Activités proposées par les hôtes ou partenaires locaux (randonnée guidée, dégustation, atelier nature) | Commission 15-20 % |
| **Guides & itinéraires** | Contenus premium (routes vanlife, guides régionaux, hors-pistes) | Freemium + premium |
| **B2B tourisme** | Outils pour offices de tourisme : dashboard de fréquentation, gestion de flux, reporting | SaaS mensuel |
| **API partenaires** | Intégration avec des acteurs tiers (agences de voyage, apps outdoor, assureurs) | Revenue share |

### 12.4.3 Vision long terme

À l'horizon Y5+, Nomad n'est plus une "app de réservation de camping" mais **l'infrastructure standard du voyage nature en Europe** :
- Les voyageurs y trouvent spots, véhicules, équipement, expériences
- Les propriétaires y gèrent leur activité d'accueil
- Les offices de tourisme y pilotent le tourisme nature de leur région
- Les acteurs outdoor (marques, loueurs, guides) y connectent leurs services

---

## 12.5 Timeline consolidée

| Trimestre | Activité principale | Terrains | Marchés |
|---|---|---|---|
| **T-1** | Pré-lancement, recrutement supply, MVP | 200 | CH romande |
| **T1-T2** | Lancement, premières réservations, itérations | 200 → 400 | CH romande |
| **T3-T4** | Expansion France (sud-est), seed round | 400 → 1 200 | CH + FR |
| **T5-T6** | Consolidation CH+FR, module véhicules | 1 200 → 2 500 | CH + FR |
| **T7-T8** | Lancement DACH, parcours intégré spot+van | 2 500 → 5 000 | CH + FR + DE/AT |
| **T9-T12** | Scaling, expériences, B2B tourisme | 5 000 → 10 000 | 5-8 marchés |
| **T12-T20** | Infrastructure, API, Phase 3 | 10 000 → 20 000+ | Pan-européen |

---

## Sources

1. Section 8 — Modèle économique (projections Y1-Y5, unit economics)
2. Section 9 — Stratégie GTM (timeline de lancement, acquisition supply/demand)
3. Concept Brief — Roadmap V1/V2/V3 originale
4. Yescapa / Goboony — Modèle P2P location de vans (benchmarks)
5. Stripe Connect — Documentation marketplace multi-vendeurs (stripe.com/connect)
