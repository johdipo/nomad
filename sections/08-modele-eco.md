# 8. Modèle économique & logique financière

La viabilité de Nomad repose sur une mécanique de revenus simple à comprendre, difficile à contourner, et qui s'améliore avec l'échelle. Cette section détaille qui paie quoi, pourquoi chaque partie accepte de payer, et comment les leviers de croissance conduisent à la rentabilité.

---

## 8.1 Mécanique de revenus — Qui paie quoi ?

Nomad est une marketplace bi-face. Le modèle économique repose sur quatre flux de revenus complémentaires, activés progressivement.

### 8.1.1 Flux 1 — Commission sur réservations (cœur du modèle)

**Structure proposée : commission partagée ~15 % du montant brut de la réservation**

| Composante | Taux | Payé par | Justification |
|---|---|---|---|
| Frais de service voyageur | 10-12 % | Voyageur | Couvre la plateforme, l'assurance, le support 24/7, la médiation |
| Frais hôte | 3-5 % | Propriétaire | Couvre le traitement des paiements, la visibilité, les outils de gestion |
| **Total prélevé** | **~15 %** | **Réparti** | **Aligné sur le standard du marché (voir §8.2)** |

**Pourquoi le propriétaire accepte :**
- Zéro coût d'entrée — listing gratuit, paiement uniquement sur transaction effective
- Pas de marketing à faire — Nomad amène les clients
- Gestion administrative déléguée — factures, conformité, encaissement
- Alternative : démarchage direct, gestion des conflits, aucun cadre légal
- Le terrain serait inutilisé sans la plateforme → le coût d'opportunité est nul

**Pourquoi le voyageur accepte :**
- Garantie de qualité (spots vérifiés, photos validées)
- Assurance intégrée (protection en cas de problème)
- Simplicité de la réservation (vs arrangements informels)
- Comparaison : 15-40 €/nuit sur Nomad vs 80-150 € en hôtel, 100-200 € en Airbnb
- Le surcoût de ~10 % est invisible face à l'économie vs hébergement classique

**Mécanique de paiement :**
- Le voyageur paie le montant total (prix affiché + frais de service) au moment de la réservation
- Nomad retient les fonds en escrow jusqu'au lendemain du check-in
- Le propriétaire reçoit son paiement (prix - frais hôte) par virement hebdomadaire
- Annulation : selon politique choisie par l'hôte (flexible / modérée / stricte)

### 8.1.2 Flux 2 — Services additionnels

Les propriétaires peuvent proposer des extras facturés via la plateforme :

| Service | Prix indicatif | Commission Nomad | Marge |
|---|---|---|---|
| Électricité (branchement 10A) | 5-8 €/nuit | 15 % | 0,75-1,20 € |
| Eau potable (remplissage) | 3-5 €/service | 15 % | 0,45-0,75 € |
| Vidange eaux grises/noires | 5-10 €/service | 15 % | 0,75-1,50 € |
| Petit-déjeuner / panier local | 8-15 €/pers | 15 % | 1,20-2,25 € |
| Bois de feu | 5-8 €/fagot | 15 % | 0,75-1,20 € |
| Activité (balade, visite ferme) | 10-25 €/pers | 15 % | 1,50-3,75 € |

**Estimation :** les services additionnels représentent en moyenne **~20-25 % du panier moyen** d'une nuitée. Sur un panier moyen de 30 €/nuit, cela ajoute ~6-8 € de services, soit ~0,90-1,20 € de revenu additionnel par nuitée pour Nomad.

### 8.1.3 Flux 3 — Mise en avant payante (à partir de Y2)

Inspiré du modèle Booking.com / Google Ads :

| Produit | Cible | Prix estimé | Activation |
|---|---|---|---|
| "Spot en vedette" | Propriétaires | 2-5 €/jour ou 30-80 €/mois | Affichage prioritaire dans les résultats de recherche |
| Bannière régionale | Offices de tourisme, marques outdoor | 200-500 €/campagne | Sponsoring de zones géographiques |
| Badge "Coup de cœur" | Propriétaires premium | Inclus dans le forfait premium | Distinction visuelle dans le catalogue |

**Condition clé :** la mise en avant ne doit pas dégrader l'expérience utilisateur. Maximum 10-15 % de résultats sponsorisés par page. La qualité du spot reste le facteur de classement principal.

### 8.1.4 Flux 4 — Forfait Premium propriétaire (à partir de Y2-Y3)

| Forfait | Prix | Contenu |
|---|---|---|
| **Standard** (gratuit) | 0 € | Listing, réservation, paiement, support de base |
| **Pro** | 15-25 €/mois | Analytics avancés, pricing dynamique assisté, réponse prioritaire au support, badge Pro |
| **Business** | 40-60 €/mois | Multi-emplacements, calendrier sync (Airbnb, Booking), outils yield management, assurance étendue, account manager dédié |

**Adoption estimée :** 10-15 % des hôtes actifs souscrivent au forfait Pro, 3-5 % au Business.

---

## 8.2 Benchmark des commissions — Comparaison concurrentielle

| Plateforme | Commission totale | Structure | Détail | Source |
|---|---|---|---|---|
| **Nomady** | ~15 % | Host-only | Le propriétaire paie la totalité ; prix affiché = prix net pour le voyageur | nomady.camp (conditions générales, mars 2026) |
| **HomeCamper / Campspace** | ~15 % | Host-only | Commission déduite du paiement au propriétaire | campspace.com (page hôte, mars 2026) |
| **AlpacaCamping** | ~12-15 % | Host-only (estimé) | Pas de frais annoncés côté voyageur ; commission hôte estimée sur base des prix observés | alpacacamping.de (estimation mars 2026) |
| **Hipcamp** | ~15-20 % | Split | ~10 % hôte (pour terrains privés) + frais de service voyageur variables | hipcamp.com (page host, FAQ, mars 2026) |
| **Airbnb** (split fee) | ~17-20 % | Split | 3 % hôte + 14,1-16,5 % voyageur | airbnb.com/help/article/1857 (mars 2026) |
| **Airbnb** (single fee) | ~14-16 % | Host-only | 14-16 % déduit du paiement hôte ; pas de frais voyageur visible | airbnb.com/help/article/1857 (mars 2026) |
| **Booking.com** | 15-20 % | Host-only | Commission variable selon marché et catégorie | booking.com (programme partenaire) |
| **Park4Night** | 0 % | Freemium | Pas de transaction ; app premium ~10 €/an | park4night.com |

**Analyse :**

Le taux de **15 % total** est le consensus du marché pour les plateformes de camping nature. Nomad se positionne dans cette fourchette, ce qui est :
- **Compétitif vs Airbnb** (17-20 % en split, ou ~15 % en single fee — mais Airbnb n'est pas spécialisé camping)
- **Aligné avec Nomady et Campspace** (standards du segment)
- **Légèrement au-dessus de Hipcamp** côté hôte (~10 % pour les terrains privés chez Hipcamp, mais le voyageur paie des frais additionnels)

**Recommandation Nomad :** Adopter le modèle **split** (10 % voyageur + 5 % hôte) plutôt que host-only (15 %). Raison : les propriétaires comparent leur net sur différentes plateformes. Un frais hôte de 5 % est psychologiquement plus acceptable que 15 %, même si le prix final voyageur est identique. C'est la stratégie d'Airbnb (split fee par défaut) et elle fonctionne.

---

## 8.3 Unit economics — CAC, LTV, marge par transaction

### 8.3.1 Panier moyen et marge par transaction

| Métrique | Valeur estimée | Source / Calcul |
|---|---|---|
| **Prix moyen par nuit** | 30 € | Moyenne pondérée (terrain nu 15-20 €, terrain équipé 25-35 €, glamping 60-120 €) — cf. section 4 |
| **Durée moyenne de séjour** | 2,5 nuits | Benchmarks Nomady (~2 nuits) et Airbnb rural (~3 nuits), pondéré |
| **Panier moyen par réservation** | 75 € | 30 € × 2,5 nuits |
| **Services additionnels** | +18 € (~24 % du panier) | Électricité, eau, extras |
| **Valeur brute par réservation** | **93 €** | Panier + services |
| **Revenu Nomad par réservation** | **~14 €** | 15 % × 93 € |
| **Coût de traitement paiement** | ~2,5 € | Stripe/Adyen : ~2,5-3 % du brut |
| **Marge brute par réservation** | **~11,5 €** | 14 € - 2,5 € |
| **Marge brute (%)** | **~82 %** | 11,5 / 14 |

La marge brute de ~82 % par transaction est caractéristique des marketplaces digitales (Airbnb : ~80 %, Booking.com : ~85 %). Le coût marginal d'une réservation supplémentaire est quasi-nul (hébergement cloud, pas de stock physique).

### 8.3.2 Coût d'acquisition client (CAC)

**Côté voyageur (demand-side) :**

| Canal | CAC estimé | Part du mix Y1-Y2 | Part du mix Y3-Y5 |
|---|---|---|---|
| **SEO / contenu** | 2-5 € | 20 % | 35 % |
| **Social media organique** | 1-3 € | 25 % | 20 % |
| **Google Ads / Meta Ads** | 8-15 € | 30 % | 25 % |
| **Parrainage / referral** | 5-8 € | 10 % | 15 % |
| **Influenceurs** | 5-12 € | 15 % | 5 % |
| **CAC moyen pondéré** | **~6-8 €** (Y1-Y2) | | **~5-7 €** (Y3-Y5) |

**Benchmarks :** Le CAC dans le secteur voyage en ligne se situe entre 5 € et 25 € selon la compétition. Le segment camping nature est moins saturé que l'hôtellerie → CAC inférieur. Nomady et AlpacaCamping, bootstrapés, ont probablement un CAC <5 € (forte composante organique).

**Côté propriétaire (supply-side) :**

| Canal | CAC estimé | Commentaire |
|---|---|---|
| **Démarchage direct** (terrain) | 50-100 € | Temps commercial + déplacement, mais conversion élevée (~30-40 %) |
| **Partenariats** (chambres agriculture, réseaux agritourisme) | 20-40 € | Coût par lot, onboarding groupé |
| **SEO / inbound** | 10-20 € | "Gagner de l'argent avec son terrain" — requêtes à forte intention |
| **Referral hôte-à-hôte** | 5-15 € | Bouche-à-oreille entre agriculteurs voisins |
| **CAC moyen supply** | **~30-50 €** | Diminue avec l'effet réseau et la notoriété |

**Benchmark :** Airbnb a historiquement dépensé ~50-100 $ pour acquérir un hôte dans ses premières années. Pour des terrains de camping (moins compétitif, propriétaires moins sollicités), un CAC de 30-50 € est réaliste.

### 8.3.3 Valeur vie client (LTV)

**Voyageur :**

| Métrique | Valeur | Calcul |
|---|---|---|
| Réservations/an (moyenne) | 2,5 | Soft vanlifers : 4-6/an, familles : 2-3/an, occasionnels : 1-2/an |
| Revenu Nomad/réservation | 14 € | cf. §8.3.1 |
| Revenu annuel/voyageur | 35 € | 2,5 × 14 € |
| Durée de rétention | 3-4 ans | Benchmark marketplaces voyage |
| **LTV voyageur** | **~105-140 €** | 35 € × 3-4 ans |
| **Ratio LTV/CAC** | **~15-23x** | 105-140 / 6-8 |

**Propriétaire :**

| Métrique | Valeur | Calcul |
|---|---|---|
| Nuitées/an (moyenne) | 50 | Saisonnier mai-sept, cf. section 4 |
| Revenu Nomad/nuit | ~4,5 € | 30 € × 15 % |
| Revenu annuel/propriétaire | 225 € | 50 × 4,5 € (commission seule) |
| Premium/ads additionnel | +30-60 €/an | 15-20 % des hôtes souscrivent Pro |
| Durée de rétention | 4-6 ans | Les hôtes restent tant que la plateforme génère des réservations |
| **LTV propriétaire** | **~1 000-1 700 €** | (225 + 40) × 4-6 ans |
| **Ratio LTV/CAC** | **~20-56x** | 1 000-1 700 / 30-50 |

**Analyse :** Les ratios LTV/CAC sont excellents (>3x est le seuil de viabilité SaaS/marketplace). Cela s'explique par :
- La faible compétition sur l'acquisition (niche peu saturée)
- La forte rétention (une fois qu'un propriétaire est actif, le coût de switch est élevé)
- La croissance du panier dans le temps (plus de nuitées, plus de services)

---

## 8.4 Projection financière — Y1 à Y5

Les projections ci-dessous reprennent et affinent le modèle bottom-up de la section 4 (SOM), en ajoutant la structure de coûts opérationnels.

### 8.4.1 Revenus

| Métrique | Y1 | Y2 | Y3 | Y4 | Y5 |
|---|---|---|---|---|---|
| **Marchés actifs** | CH romande | CH + FR | CH+FR+DE | CH+FR+DE+AT/IT | 8 marchés |
| **Terrains actifs** | 200 | 1 200 | 4 000 | 8 500 | 15 000 |
| **Nuitées/terrain/an** | 25 | 35 | 45 | 50 | 55 |
| **Prix moyen/nuit (€)** | 30 | 28 | 28 | 29 | 30 |
| **Volume brut réservations (M€)** | 0,15 | 1,18 | 5,04 | 12,33 | 24,75 |
| **Commission 15 % (M€)** | 0,02 | 0,18 | 0,76 | 1,85 | 3,71 |
| **Services additionnels (M€)** | 0,01 | 0,06 | 0,25 | 0,62 | 1,24 |
| **Premium + ads (M€)** | — | 0,02 | 0,10 | 0,30 | 0,60 |
| **Revenu total (M€)** | **0,03** | **0,26** | **1,11** | **2,77** | **5,55** |

### 8.4.2 Structure de coûts

| Poste | Y1 | Y2 | Y3 | Y4 | Y5 | % du CA (Y5) |
|---|---|---|---|---|---|---|
| **Équipe** (fondateurs + premiers recrutements) | 120K | 280K | 550K | 900K | 1 400K | 25 % |
| **Traitement paiements** (~2,5 % du brut) | 4K | 30K | 126K | 308K | 619K | 11 % |
| **Acquisition marketing** | 30K | 120K | 300K | 500K | 700K | 13 % |
| **Infrastructure tech** (cloud, CDN, API) | 12K | 30K | 60K | 100K | 150K | 3 % |
| **Support client** | — | 20K | 80K | 180K | 300K | 5 % |
| **Assurance & juridique** | 10K | 40K | 100K | 200K | 350K | 6 % |
| **Onboarding terrain** (démarchage, photos, validation) | 20K | 60K | 120K | 200K | 300K | 5 % |
| **Divers** (bureau, compta, admin) | 15K | 30K | 60K | 100K | 150K | 3 % |
| **Coûts totaux (K€)** | **211** | **610** | **1 396** | **2 488** | **3 969** | **72 %** |

### 8.4.3 Résultat opérationnel

| Métrique | Y1 | Y2 | Y3 | Y4 | Y5 |
|---|---|---|---|---|---|
| **Revenus (K€)** | 30 | 260 | 1 110 | 2 770 | 5 550 |
| **Coûts (K€)** | 211 | 610 | 1 396 | 2 488 | 3 969 |
| **Résultat opérationnel (K€)** | **-181** | **-350** | **-286** | **+282** | **+1 581** |
| **Marge opérationnelle** | -603 % | -135 % | -26 % | +10 % | **+28 %** |
| **Cash cumulé brûlé (K€)** | -181 | -531 | -817 | -535 | +1 046 |

### 8.4.4 Besoin en financement

| Phase | Période | Besoin | Usage |
|---|---|---|---|
| **Pre-seed** | Y0-Y1 | 200-300 K€ | MVP, premiers 200 terrains, validation CH romande |
| **Seed** | Y1-Y2 | 500K-1 M€ | Expansion France, équipe produit + terrain, marketing |
| **Série A** (optionnel) | Y3 | 2-5 M€ | Scaling DACH, tech avancée (IA, pricing dynamique), 4 000 terrains |

**Cash runway :** Avec un seed de 800 K€ en Y1, la plateforme atteint le breakeven opérationnel en Y4 (mois ~36-42). Le besoin cumulé maximum est de ~817 K€ (fin Y3) avant que les revenus couvrent les coûts.

**Scénario sans Série A :** Si la plateforme reste sur CH + FR uniquement et croît organiquement, le breakeven est atteint en Y3-Y4 avec des coûts plus faibles (pas d'expansion DACH). La Série A est un accélérateur, pas une nécessité de survie.

---

## 8.5 Leviers de croissance et effets d'échelle

### 8.5.1 Effet réseau bi-face

Le levier le plus puissant de Nomad est l'**effet de réseau bi-face** :

```
Plus de terrains → plus de choix → plus de voyageurs
     ↓                                    ↓
Plus de revenus pour les hôtes ← plus de réservations
```

**Seuil critique estimé :** L'effet réseau devient auto-entretenu à partir de ~500-1 000 terrains actifs par marché géographique. En-dessous, l'offre est trop maigre pour retenir les voyageurs. Au-dessus, la croissance organique (bouche-à-oreille, SEO, referral) commence à dominer l'acquisition payante.

**Preuve par l'analogie :** Airbnb a identifié le seuil de ~300 listings/ville pour que l'effet réseau s'enclenche. Pour le camping nature (rayon de recherche plus large, ~100-200 km), le seuil est ~500-1 000 par pays/région.

### 8.5.2 Amélioration des marges avec l'échelle

| Métrique | Y1 | Y3 | Y5 | Tendance |
|---|---|---|---|---|
| CAC voyageur | ~8 € | ~6 € | ~5 € | ↘ SEO + referral prennent le relais |
| CAC propriétaire | ~50 € | ~35 € | ~25 € | ↘ Notoriété + inbound + referral hôte-à-hôte |
| Coût support / réservation | ~2 € | ~0,80 € | ~0,40 € | ↘ Automatisation + FAQ + IA |
| Marge opérationnelle | -603 % | -26 % | +28 % | ↗ Levier opérationnel classique |

**Explication :** Les coûts fixes (équipe tech, infrastructure) se répartissent sur un volume croissant de transactions. Les coûts variables (paiement, support) diminuent en % grâce à l'automatisation et au pouvoir de négociation (tarifs Stripe/Adyen baissent avec le volume).

### 8.5.3 Expansion géographique comme levier

Chaque nouveau marché géographique (Allemagne, Italie, Espagne) réplique le playbook suisse/français avec un coût marginal décroissant :
- **Tech :** la même plateforme, déjà construite
- **Process :** les mêmes outils d'onboarding, déjà rodés
- **Marque :** la crédibilité acquise en CH/FR accélère la confiance
- **Coût spécifique :** conformité légale locale (~20-50 K€ par pays) + équipe terrain locale

Le coût d'entrée par nouveau marché est estimé à **~100-200 K€** (juridique + marketing lancement + premiers 200 terrains), soit un investissement récupéré en 12-18 mois par les commissions générées.

### 8.5.4 Services à haute marge (Y3+)

| Service | Marge brute | Potentiel |
|---|---|---|
| **Premium propriétaire** (SaaS) | ~90 % | Revenu récurrent, prévisible, non lié au volume de réservations |
| **Mise en avant payante** | ~95 % | Coût marginal quasi-nul (affichage), forte élasticité prix |
| **Assurance intégrée** (courtage) | ~20-30 % | Commission sur primes, partenariat avec assureur (ex : AXA, Allianz) |
| **Location véhicules** (Phase 2) | ~15 % | Commission P2P, panier moyen 80-200 €/jour → ~12-30 €/jour de revenu |

La Phase 2 (intégration véhicules) est le levier de croissance le plus important à moyen terme. Le panier moyen d'une location de van (80-200 €/jour) est 3-7x supérieur à une nuitée terrain (30 €). Même avec une commission plus faible (~10-12 %), le revenu par transaction est multiplié.

---

## 8.6 Quand la plateforme devient-elle rentable ?

### 8.6.1 Breakeven opérationnel

| Scénario | Terrains | Nuitées/an | Volume brut | CA Nomad | Breakeven |
|---|---|---|---|---|---|
| **Conservateur** (CH+FR seuls) | 3 000 | 120K | 3,6 M€ | 680 K€ | ~Y3 (mois 30-36) |
| **Base** (CH+FR+DE) | 5 000 | 225K | 6,3 M€ | 1,2 M€ | ~Y3-Y4 (mois 36-42) |
| **Accéléré** (8 marchés) | 8 000+ | 400K+ | 12 M€+ | 2,4 M€+ | ~Y3 (mois 28-34) |

**Le seuil de rentabilité se situe à environ 3 000-5 000 terrains actifs** et **120 000-225 000 nuitées/an**, correspondant à un CA de ~700 K€ - 1,2 M€. Ce seuil est atteignable en Y3 dans le scénario base.

### 8.6.2 Comparaison avec les pairs

| Plateforme | Année de rentabilité | Terrains au breakeven | Funding avant breakeven |
|---|---|---|---|
| **Nomady** | Non rentable (estimé) | 1 600 (insuffisant) | ~125 K CHF |
| **Airbnb** | Y10+ (2022, IPO 2020) | >6 M listings | ~6 Md$ |
| **Booking.com** | Y5 (profitable dès 2001) | ~50 000 hôtels | ~3,7 M€ (IPO 2004) |
| **Nomad (cible)** | Y3-Y4 | 3 000-5 000 | ~1-1,5 M€ |

Nomad vise une trajectoire plus proche de **Booking.com** (breakeven rapide, capital-efficient) que d'**Airbnb** (hypercroissance financée par le VC). C'est un choix stratégique : la profitabilité rapide offre de l'indépendance et réduit la dilution.

---

## 8.7 Risques et sensibilités

### 8.7.1 Sensibilité aux hypothèses clés

| Variable | Hypothèse base | Variation -20 % | Impact sur CA Y5 |
|---|---|---|---|
| Terrains actifs | 15 000 | 12 000 | -20 % (4,4 M€ vs 5,5 M€) |
| Nuitées/terrain/an | 55 | 44 | -20 % (4,4 M€) |
| Prix moyen/nuit | 30 € | 24 € | -20 % (4,4 M€) |
| Taux de commission | 15 % | 12 % | -20 % (4,4 M€) |

Le modèle est linéairement sensible à chacune de ces variables. Le risque principal est le **recrutement de terrains** : si l'acquisition d'offre est plus lente que prévu, tout le modèle ralentit proportionnellement.

### 8.7.2 Risque de désintermédiation

Le risque classique des marketplaces : après une première réservation via Nomad, le voyageur et le propriétaire se contactent directement et contournent la plateforme.

**Atténuations :**
- **Assurance** : couvre uniquement les réservations Nomad → forte incitation à rester sur la plateforme
- **Facilité** : paiement, facturation, annulation, avis — tout est automatisé via Nomad
- **Découverte** : un voyageur visite 3-5 spots différents par an → la valeur de la plateforme est dans le catalogue, pas dans un spot unique
- **Benchmark** : Airbnb a montré que la désintermédiation reste marginale (~5-10 %) quand la plateforme apporte une vraie valeur (assurance, support, trust)

### 8.7.3 Guerre des prix

Si Campspace ou un nouvel entrant baisse ses commissions à 10 % ou moins :
- **Réponse :** la différenciation de Nomad repose sur la qualité (curation, confiance, assurance), pas sur le prix. Les propriétaires paient pour la tranquillité, pas pour le taux le plus bas.
- **Protection :** les forfaits Premium et les services additionnels diversifient les revenus au-delà de la commission pure.

---

## 8.8 Synthèse du modèle économique

```
┌─────────────────────────────────────────────────────────────────┐
│                    FLUX DE REVENUS NOMAD                        │
│                                                                 │
│  Y1 ──────────────────────────────────────────────────── Y5     │
│                                                                 │
│  ████████████████████████████████████████  Commission 15 %      │
│  ████████████████████████                 Services (+24 %)      │
│  ████████████                             Premium / Ads         │
│  ████                                     Phase 2 (véhicules)  │
│                                                                 │
│  Breakeven : Y3-Y4 │ ~3 000-5 000 terrains │ CA ~1 M€          │
│  Y5 : CA ~5,5 M€  │ Marge opérationnelle ~28 %                 │
└─────────────────────────────────────────────────────────────────┘
```

**Le modèle Nomad en 5 points :**

1. **Simple :** commission de 15 % partagée (10 % voyageur + 5 % hôte), alignée sur le marché
2. **Défendable :** assurance, confiance et qualité rendent la désintermédiation peu attractive
3. **Scalable :** coûts marginaux quasi-nuls par transaction, effet réseau bi-face auto-entretenu
4. **Capital-efficient :** breakeven en Y3-Y4 avec ~1 M€ de funding cumulé (pre-seed + seed)
5. **Extensible :** services additionnels, premium SaaS, et Phase 2 véhicules ouvrent des flux à haute marge

---

## Sources

1. Airbnb — Service fees (airbnb.com/help/article/1857, consulté mars 2026)
2. Hipcamp — Host page et FAQ (hipcamp.com/en-US/host, consulté mars 2026)
3. Campspace — Host page (campspace.com/en/host, consulté mars 2026)
4. Nomady — Conditions générales hôtes (nomady.camp, consulté mars 2026)
5. AlpacaCamping — Site officiel (alpacacamping.de, consulté mars 2026)
6. Booking.com — Partner programme, commission structure
7. Section 4 (Taille de marché) du présent whitepaper — projections Y1-Y5
8. Section 5 (Analyse concurrentielle) du présent whitepaper — données concurrents
9. Stripe — Tarification standard Europe (stripe.com/pricing, 2,5-3 % + fixe)
10. Crunchbase — Données funding Airbnb, Booking Holdings, Hipcamp
