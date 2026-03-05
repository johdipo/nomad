# 6. La solution Nomad — Produit & parcours utilisateur

Nomad est une marketplace bi-face qui connecte les voyageurs en quête de nature avec les propriétaires de terrains privés et les campings, dans un cadre légal, sécurisé et simple. Cette section décrit concrètement le fonctionnement de la plateforme et les parcours utilisateur des deux côtés du marché.

---

## 6.1 Le produit en une phrase

Nomad est le **Airbnb du camping nature** : une application mobile-first qui permet de découvrir, réserver et payer un emplacement nature — terrain privé, ferme, domaine viticole ou camping — en quelques minutes, avec assurance intégrée, avis vérifiés et un tiers de confiance qui gère tout le reste.

---

## 6.2 Architecture fonctionnelle

La plateforme repose sur trois piliers :

| Pilier | Fonction | Pour qui |
|---|---|---|
| **Marketplace** | Recherche, réservation, paiement | Voyageurs & propriétaires |
| **Infrastructure de confiance** | Assurance, médiation, conformité légale | Les deux côtés |
| **Outils de gestion** | Dashboard hôte, calendrier, analytics, pricing | Propriétaires |

**Mobile-first, web-responsive.** L'app native (iOS/Android) est le canal principal — les voyageurs cherchent un spot en déplacement, souvent sur la route. Le web desktop sert au parcours propriétaire (onboarding, gestion) et au SEO (acquisition organique).

---

## 6.3 Parcours voyageur — De la découverte à l'avis

### Étape 1 — Découverte : « Où dormir ce soir ? »

**Le besoin :** Le voyageur arrive dans une région et cherche un endroit pour la nuit (ou planifie un séjour en amont).

**L'expérience Nomad :**
- Ouverture de l'app → carte interactive centrée sur sa position GPS (ou recherche par destination)
- **Filtres intelligents** : type de terrain (ferme, vignoble, forêt, bord de lac, alpage), services disponibles (eau, électricité, sanitaires, douche), prix, note, type de véhicule accepté (van, camping-car, tente), animaux admis, nombre de places restantes
- **Résultats visuels** : chaque spot affiche photo principale, prix/nuit, note moyenne, distance, et un badge de vérification (✓ Vérifié Nomad)
- **Fiches détaillées** : galerie photos validées par Nomad, description du lieu et de l'hôte, services et tarifs détaillés, règlement intérieur, avis vérifiés des voyageurs précédents, situation légale claire (« Terrain déclaré, accueil autorisé »)
- **Recommandations IA** (Phase 2) : suggestions personnalisées basées sur l'historique, les préférences et le profil du voyageur

**Friction supprimée :** Plus besoin de jongler entre 3-5 apps (Park4Night pour les spots, Booking pour les campings, Google Maps pour vérifier). Un seul point d'entrée, un seul catalogue, une seule expérience.

**Temps : 2-5 minutes** (vs 1-2 heures dans le parcours actuel — cf. section 2.3).

---

### Étape 2 — Réservation : « Je prends celui-là »

**Le besoin :** Le voyageur a trouvé un spot qui lui convient. Il veut confirmer et payer rapidement.

**L'expérience Nomad :**
- Sélection des dates (arrivée/départ) → affichage du prix total (nuitées + services choisis + frais de service)
- **Ajout de services optionnels** : électricité, eau, petit-déjeuner local, panier de produits de la ferme — chaque extra est tarifé clairement et ajouté en un tap
- **Réservation instantanée** (mode par défaut) ou demande de réservation (si l'hôte préfère valider manuellement)
- **Paiement sécurisé** : carte bancaire, Apple Pay, Google Pay. Le montant est débité et retenu en escrow par Nomad jusqu'au lendemain du check-in
- **Confirmation instantanée** : notification push + email avec les détails du séjour, l'adresse exacte, les instructions d'accès, et un canal de messagerie direct avec l'hôte
- **Politique d'annulation transparente** : flexible (remboursement intégral jusqu'à 24h avant), modérée (50 % jusqu'à 48h), stricte (pas de remboursement < 7 jours) — choisie par l'hôte, visible avant la réservation

**Friction supprimée :** Plus de téléphone, d'email sans réponse, de prix flou. Le voyageur connaît le coût exact, a une confirmation en temps réel, et dispose d'un contact direct avec l'hôte — le tout en 2 minutes.

---

### Étape 3 — Séjour : « Bienvenue chez nous »

**Le besoin :** Le voyageur arrive sur le terrain. Il veut se garer, se brancher, et profiter.

**L'expérience Nomad :**
- **Navigation guidée** : l'app affiche le chemin GPS jusqu'à l'emplacement exact (coordonnées précises, pas juste une adresse postale)
- **Check-in digital** : confirmation d'arrivée en un tap → l'hôte est notifié. Optionnellement, code d'accès ou boîte à clés pour les arrivées tardives
- **Guide du séjour** : l'app affiche les informations pratiques — où se brancher, où trouver l'eau, horaires des sanitaires, règles du terrain, recommandations locales de l'hôte (randonnées, restaurants, marchés)
- **Messagerie intégrée** : canal direct avec l'hôte pour toute question. En cas de problème non résolu, escalade vers le support Nomad (chat 7j/7)
- **Signalement de problème** : si le spot ne correspond pas à la description, le voyageur peut signaler un écart → Nomad intervient (médiation, remboursement partiel, relogement si nécessaire)

**Friction supprimée :** Plus d'incertitude. Le voyageur sait exactement où aller, ce qu'il trouvera, et a un recours en cas de problème. C'est la différence entre le camping sauvage (espérer que ça ira) et Nomad (savoir que c'est couvert).

---

### Étape 4 — Avis & fidélisation : « C'était comment ? »

**Le besoin :** Le voyage est terminé. Le voyageur veut partager son expérience et retrouver facilement ses spots favoris.

**L'expérience Nomad :**
- **Notification post-séjour** (J+1) : invitation à laisser un avis (note + commentaire structuré : cadre, propreté, accueil, services, rapport qualité/prix)
- **Avis vérifiés uniquement** : seuls les voyageurs ayant effectivement séjourné peuvent noter → crédibilité maximale (vs Park4Night où n'importe qui peut commenter)
- **Photos du séjour** : le voyageur peut ajouter ses propres photos, qui enrichissent la fiche du spot (avec modération)
- **Favoris et historique** : le voyageur retrouve ses spots aimés, peut les partager avec des amis, et recevoir des alertes (promo, nouveau spot similaire dans la zone)
- **Programme de fidélité** (Phase 2) : points cumulés → réductions sur les prochains séjours, badges voyageur (« Explorateur », « Habitué », « Ambassadeur »)

**Friction supprimée :** Un cercle vertueux de confiance. Les avis vérifiés rendent les prochains voyageurs plus sereins. Les propriétaires bien notés attirent plus de réservations. L'effet de réseau s'enclenche.

---

### Résumé du parcours voyageur

```
📱 Ouvrir Nomad
    │
    ▼
🗺️ Découvrir — carte, filtres, recommandations
    │                                              ⏱️ 2-5 min
    ▼
📋 Comparer — fiches détaillées, avis, photos
    │
    ▼
💳 Réserver — dates, services, paiement sécurisé
    │                                              ⏱️ 2 min
    ▼
📍 Arriver — GPS, check-in digital, guide du séjour
    │
    ▼
🏕️ Séjourner — confort, messagerie hôte, support Nomad
    │
    ▼
⭐ Évaluer — avis vérifié, photos, favoris
    │
    ▼
🔄 Revenir — historique, recommandations, fidélité
```

**De 1-2 heures de galère quotidienne à 5 minutes de tranquillité.** C'est la promesse.

---

## 6.4 Parcours propriétaire — De l'inscription au revenu

### Étape 1 — Inscription : « J'ai un terrain, par où je commence ? »

**Le besoin :** Le propriétaire a entendu parler de Nomad (bouche-à-oreille, pub, article) et veut explorer l'option d'accueillir des campeurs.

**L'expérience Nomad :**
- **Page d'inscription dédiée** (« Devenir hôte ») : processus en 5 minutes, pas en 5 semaines
- **Informations de base** : nom, adresse du terrain, type de propriété (ferme, domaine, terrain privé, camping), nombre d'emplacements envisagés
- **Vérification d'identité** : pièce d'identité + justificatif de propriété (extrait cadastral ou titre de propriété). Nomad vérifie que le propriétaire a le droit d'accueillir sur ce terrain
- **Guide réglementaire personnalisé** : en fonction du pays, de la commune et du type de terrain, Nomad affiche les obligations légales applicables (déclaration en mairie, normes sanitaires, capacité max sans permis). Un résumé clair, pas un document juridique de 40 pages
- **Assurance incluse** : dès l'inscription validée, le propriétaire est couvert par l'assurance responsabilité civile collective Nomad (pour les dommages causés aux voyageurs sur le terrain). Pas de démarche supplémentaire, pas de surcoût visible — c'est intégré dans la commission

**Friction supprimée :** Le parcours actuel (mairie → juriste → assureur → site web → marketing) est remplacé par un onboarding guidé de 5-10 minutes. Nomad absorbe la complexité administrative et assurantielle.

---

### Étape 2 — Création du listing : « Montrer ce que j'ai à offrir »

**Le besoin :** Le propriétaire veut présenter son terrain de façon attractive sans être graphiste ni copywriter.

**L'expérience Nomad :**
- **Assistant de création** : formulaire étape par étape avec des questions simples (« Décrivez votre terrain en 2-3 phrases », « Qu'est-ce qui rend votre endroit spécial ? »)
- **Photos guidées** : l'app demande des photos spécifiques (vue d'ensemble, emplacement, sanitaires, accès) avec des exemples de bonnes photos. Option : demander une visite photo par un photographe Nomad local (Phase 2)
- **Services et équipements** : checklist à cocher — eau potable, électricité, douche, toilettes, Wi-Fi, barbecue, table de pique-nique, ombre, vue, accès rivière/lac
- **Pricing assisté** : Nomad suggère un prix/nuit basé sur la région, la saison, les services et la concurrence locale. Le propriétaire peut ajuster librement
- **Disponibilités** : calendrier synchronisable (iCal) ou gestion manuelle. Possibilité de bloquer des dates (usage personnel, travaux, etc.)
- **Validation Nomad** : avant publication, l'équipe Nomad vérifie les photos (conformité, qualité minimum) et la description (cohérence, clarté). Objectif : qualité constante du catalogue

**Friction supprimée :** Le propriétaire n'a pas besoin de compétences digitales. L'assistant guide chaque étape, et la validation Nomad garantit que le listing sera attractif. Pas de listing « fantôme » comme sur Campspace — chaque spot publié est vivant et vérifié.

---

### Étape 3 — Réception des réservations : « On me trouve, on me réserve »

**Le besoin :** Le propriétaire veut recevoir des réservations sans effort marketing et garder le contrôle sur qui vient.

**L'expérience Nomad :**
- **Deux modes de réservation** au choix :
  - *Instantané* : le voyageur réserve directement, le propriétaire est notifié → friction minimum, conversion maximum
  - *Demande* : le voyageur envoie une demande, le propriétaire accepte ou refuse dans un délai de 24h → plus de contrôle, moins de conversion
- **Notification push + email** à chaque réservation confirmée : dates, profil du voyageur (note, nombre de séjours, véhicule), montant, instructions spéciales
- **Messagerie pré-séjour** : le voyageur et l'hôte peuvent échanger avant l'arrivée (heure d'arrivée, accès, questions)
- **Gestion du calendrier** : vue semaine/mois, occupation en temps réel, revenus projetés
- **Alertes intelligentes** (Phase 2) : « Vous avez un week-end libre dans 2 semaines et la demande est forte dans votre zone — voulez-vous activer une promotion ? »

**Friction supprimée :** Fini le marketing. Nomad amène les voyageurs. Le propriétaire n'a qu'à attendre les notifications et préparer le terrain. C'est le modèle « zéro effort marketing » identifié dans l'analyse JTBD (section 2.2, JTBD 6).

---

### Étape 4 — Paiement : « Je suis payé sans me soucier de rien »

**Le besoin :** Le propriétaire veut recevoir ses revenus de façon fiable, régulière et sans gestion comptable complexe.

**L'expérience Nomad :**
- **Paiement automatique** : Nomad verse les revenus nets (prix de la nuitée - commission hôte de 3-5 %) par virement bancaire, chaque semaine
- **Relevé détaillé** : pour chaque virement, un relevé en ligne indiquant chaque réservation, les montants bruts, les commissions, les services additionnels, et le net versé
- **Factures conformes** : Nomad génère automatiquement les factures pour chaque transaction — le propriétaire n'a rien à produire
- **Aide fiscale** : un guide par pays (Suisse, France, Allemagne, etc.) expliquant comment déclarer ces revenus — régime applicable, seuils, exonérations éventuelles. Pas de conseil fiscal personnalisé, mais un cadre clair pour éviter le flou
- **Dashboard de revenus** : revenus du mois, comparaison avec le mois précédent, projection annuelle, taux d'occupation

**Friction supprimée :** Le propriétaire reçoit un virement hebdomadaire avec un relevé complet. La question « comment déclarer ? » a une réponse claire dans l'app. Fini le flou fiscal qui freine 95 % des propriétaires potentiels (cf. section 2.2, JTBD 7).

---

### Résumé du parcours propriétaire

```
🏡 S'inscrire — 5-10 min, vérification, assurance incluse
    │
    ▼
📸 Créer son listing — assistant guidé, photos, prix suggéré
    │
    ▼
✅ Validation Nomad — qualité garantie, listing publié
    │
    ▼
📩 Recevoir des réservations — notifications, messagerie, calendrier
    │
    ▼
🏕️ Accueillir — check-in digital, guide du séjour
    │
    ▼
💰 Être payé — virement hebdomadaire, relevé, aide fiscale
    │
    ▼
📊 Optimiser — dashboard, avis, promotions
```

**De « 95 % d'abandon avant la première nuitée » à « première réservation en moins d'une semaine. »**

---

## 6.5 Le rôle de tiers de confiance — L'infrastructure invisible

Ce qui distingue fondamentalement Nomad d'un simple annuaire (Park4Night) ou d'un catalogue non curé (Campspace), c'est son rôle de **tiers de confiance**. Nomad ne se contente pas de mettre en relation : il garantit, sécurise et intervient.

### Ce que « tiers de confiance » signifie concrètement

| Fonction | Ce que fait Nomad | Ce que ça remplace |
|---|---|---|
| **Vérification** | Identité du propriétaire vérifiée, droit d'accueil confirmé, photos validées | Croire sur parole un listing anonyme |
| **Assurance** | RC collective pour hôtes et voyageurs, couverture dommages, protection annulation | Chaque propriétaire cherche seul un assureur (souvent sans succès) |
| **Paiement sécurisé** | Escrow : fonds retenus jusqu'après le check-in, virement automatique à l'hôte | Paiement en espèces, virement manuel, risque d'impayé |
| **Médiation** | En cas de litige (spot non conforme, dégradation, bruit), Nomad intervient comme arbitre neutre | Propriétaire seul face au problème, voyageur sans recours |
| **Conformité légale** | Guide réglementaire par pays/commune, cadre contractuel standard | Chaque propriétaire réinvente la roue juridique |
| **Qualité** | Standards minimums (photos, description, services), avis vérifiés, suspension des listings en-dessous du seuil | Marketplace « Far West » où tout coexiste |

### Pourquoi c'est un moat

L'infrastructure de confiance est le **moat le plus défensif** de Nomad (cf. section 5.4, Gap 3). Construire un système d'assurance collective multi-pays, un cadre juridique par juridiction, et une équipe de médiation prend du temps et de l'expertise. Un concurrent qui lance une app de réservation sans cette couche de confiance n'offre qu'un Park4Night avec un bouton « payer » — insuffisant pour convaincre les propriétaires frileux et les familles soucieuses de sécurité.

---

## 6.6 Ce que Nomad n'est PAS

Pour éviter toute confusion, voici ce que Nomad ne fait pas :

- **Nomad n'est pas un guide communautaire** (≠ Park4Night) : les spots sont vérifiés, pas crowdsourcés. On ne trouvera pas de parking de supermarché dans le catalogue.
- **Nomad n'est pas un agrégateur de campings** (≠ PiNCAMP, ACSI) : Nomad inclut des campings classiques mais se différencie par les terrains privés et l'expérience nature authentique.
- **Nomad n'est pas un annuaire sans transaction** : chaque spot listé est réservable et payable en ligne. Pas de « contactez le propriétaire par email ».
- **Nomad n'est pas réservé aux vans** : tentes, camping-cars, caravanes, et même hébergements insolites (cabane, tipi, yourte proposés par l'hôte) — le format de séjour est flexible.

---

## Sources

- Concept brief Nomad (Johan, janvier 2026) — vision produit, parcours utilisateurs, USP
- Business Model Canvas Nomad (Johan, janvier 2026) — proposition de valeur, segments, activités clés
- Section 2 (Problème utilisateur — JTBD) du présent whitepaper — frictions identifiées et workarounds
- Section 5 (Concurrence) du présent whitepaper — analyse des acteurs et gaps exploitables
- Section 8 (Modèle économique) du présent whitepaper — mécanique de commission et paiement
- Nomady.camp — modèle d'assurance intégrée et parcours hôte (consulté mars 2026)
- Campspace.com — UX réservation et limites qualitatives (consulté mars 2026)
- Park4Night.com — modèle communautaire et limites transactionnelles (consulté mars 2026)
