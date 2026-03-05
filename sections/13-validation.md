# 13. Stratégie de validation terrain

Un whitepaper ne fait pas un business. Cette section identifie les hypothèses critiques du projet Nomad — celles qui, si elles s'avèrent fausses, tuent le projet — et propose un plan concret pour les tester avant d'investir massivement.

---

## 13.1 Top 5 des hypothèses critiques

### Hypothèse 1 — Les propriétaires de terrains acceptent de lister ⭐⭐⭐ (critique)

**L'hypothèse :** Des propriétaires de terrains ruraux (agriculteurs, vignerons, domaines) accepteront de mettre à disposition un espace pour des voyageurs, via une plateforme en ligne, pour 20-40 €/nuit.

**Pourquoi c'est critique :** Sans offre, pas de marketplace. Tout le modèle repose sur la capacité à recruter des hôtes. Si les propriétaires ne voient pas la valeur, refusent le concept, ou ont peur des risques, le projet s'arrête.

**Risques :**
- Méfiance envers les plateformes ("encore un truc internet")
- Peur des dommages, de la responsabilité, des conflits
- Trop de friction administrative (même simplifiée)
- Revenu perçu comme trop faible (25-38 €/nuit net)
- Résistance culturelle : "mon terrain, c'est privé"

**Comment tester :**
- **Test :** Démarcher 30 propriétaires en Suisse romande (visites physiques, fermes, vignobles)
- **Durée :** 4-6 semaines
- **Coût :** ~500-800 € (déplacements, support visuel/démo)
- **Metric :** Taux de conversion proposition → listing accepté

**Go/No-go :**
- ✅ GO : >30 % de conversion (10+ sur 30 acceptent de lister)
- ⚠️ PIVOT : 15-30 % (intérêt mais freins identifiables et résolvables)
- ❌ STOP : <15 % (le concept ne résonne pas)

---

### Hypothèse 2 — Les voyageurs réservent (et paient) des terrains privés ⭐⭐⭐ (critique)

**L'hypothèse :** Des voyageurs (vanlifers, campeurs, familles) sont prêts à réserver ET payer en ligne pour dormir sur un terrain privé chez un particulier, plutôt que de faire du camping sauvage gratuit ou d'aller en camping classique.

**Pourquoi c'est critique :** L'existence de la demande transactionnelle est la deuxième condition de la marketplace. Park4Night prouve que la demande de spots nature existe, mais pas qu'elle est monétisable.

**Risques :**
- "Pourquoi payer quand le camping sauvage est gratuit ?"
- Prix perçu comme trop élevé pour "un champ"
- Préférence pour les campings classiques (plus de services)
- Barrière de confiance : "dormir chez un inconnu dans la campagne"

**Comment tester :**
- **Test :** Landing page avec 10-15 vrais terrains (photos, prix, localisation) + bouton "Réserver" → mesurer les intentions
- **Variante avancée :** 5-10 vraies réservations sur un MVP minimal (même un formulaire Google + paiement Stripe)
- **Durée :** 6-8 semaines (dont 4 semaines de saison camping)
- **Coût :** ~300-500 € (landing page, ads ciblés, Stripe test)
- **Metric :** Taux de conversion visiteur → clic "Réserver", puis réservation effective

**Go/No-go :**
- ✅ GO : >3 % de conversion clic réservation, >10 réservations réelles sur la période test
- ⚠️ PIVOT : 1-3 % conversion, <10 réservations (demande tiède, revoir le positionnement prix/qualité)
- ❌ STOP : <1 % conversion, 0-2 réservations (pas de demande transactionnelle)

---

### Hypothèse 3 — Le prix moyen de 25-35 €/nuit est accepté ⭐⭐ (important)

**L'hypothèse :** Les voyageurs perçoivent 25-35 €/nuit comme un prix juste pour un terrain privé en nature (sans sanitaires complets, sans piscine, sans animation).

**Pourquoi c'est important :** Si le prix acceptable est <15 €, le modèle économique (commission 15 %) ne génère pas assez de revenu par transaction pour couvrir les coûts.

**Comment tester :**
- **Test :** Proposer les mêmes terrains à 3 prix différents (A/B/C testing) : 15 €, 25 €, 40 € et mesurer le taux de réservation
- **Durée :** Pendant le test de l'hypothèse 2 (mutualisé)
- **Metric :** Élasticité-prix (variation du taux de conversion selon le prix)

**Go/No-go :**
- ✅ GO : Le taux de conversion est similaire à 25 € et 15 € (le prix n'est pas le frein principal)
- ⚠️ AJUSTER : Le taux chute fortement au-dessus de 20 € → repositionner vers le bas, ajuster le mix de terrains
- ❌ STOP : Conversion uniquement à <15 € → marge insuffisante, modèle non viable

---

### Hypothèse 4 — Les hôtes délivrent une bonne expérience ⭐⭐ (important)

**L'hypothèse :** Les propriétaires non professionnels sont capables de fournir une expérience satisfaisante (propreté, accueil, respect de la description, réactivité) sans encadrement lourd.

**Pourquoi c'est important :** Si les premières expériences voyageur sont mauvaises (terrain sale, hôte absent, photos trompeuses), le NPS s'effondre, les avis sont négatifs, et le bouche-à-oreille tue la croissance.

**Comment tester :**
- **Test :** Après les 10 premières réservations, enquête NPS + avis détaillés
- **Durée :** Pendant la phase test (M0-M3)
- **Metric :** NPS, taux de réclamation, taux de repeat booking

**Go/No-go :**
- ✅ GO : NPS > 40, <10 % de réclamations
- ⚠️ AJUSTER : NPS 20-40 → renforcer l'onboarding hôte, ajouter des standards minimum, créer un "kit hôte"
- ❌ STOP : NPS < 20, >25 % de réclamations → le modèle "non professionnel" ne fonctionne pas, pivoter vers les campings uniquement

---

### Hypothèse 5 — La réglementation est navigable ⭐⭐ (important)

**L'hypothèse :** Le cadre légal du camping sur terrain privé en Suisse et en France est suffisamment clair et permissif pour opérer sans risque juridique majeur.

**Pourquoi c'est important :** Si le cadre légal est trop flou, restrictif ou risqué, Nomad ne peut pas promettre la "tranquillité d'esprit" qui est sa proposition de valeur centrale.

**Comment tester :**
- **Test :** Consultation juridique avec un avocat spécialisé (droit de l'urbanisme + tourisme) en Suisse et en France
- **Durée :** 2-4 semaines
- **Coût :** 1 500-3 000 € (2 consultations, CH + FR)
- **Metric :** Avis juridique structuré avec matrice risques/opportunités

**Go/No-go :**
- ✅ GO : Cadre légal clair et permissif (CH : accord propriétaire suffit ; FR : R. 111-42 applicable)
- ⚠️ ADAPTER : Zones grises identifiées → adapter le produit (limiter le nombre d'emplacements, ajouter des disclaimers, géo-fencing des zones interdites)
- ❌ STOP : Risque juridique majeur (interdiction de fait, responsabilité civile non couvrable)

---

## 13.2 Plan de MVP — Le plus petit produit qui valide

### 13.2.1 Le MVP "100 nuits"

**Objectif :** Valider les hypothèses 1, 2, 3 et 4 avec un investissement minimal.

**Le concept :** Faire réserver 100 nuits sur 10-15 terrains en Suisse romande pendant une saison (mai-septembre), avec un produit minimal.

| Composant | Solution MVP | Coût |
|---|---|---|
| **Catalogue** | 10-15 terrains recrutés en personne | 0 € (temps) + 500 € (déplacements) |
| **Site web** | Landing page + fiches terrain (Webflow ou Next.js simple) | 0-500 € |
| **Réservation** | Calendly ou formulaire custom + Stripe Payment Links | 0 € |
| **Messagerie** | WhatsApp ou Telegram direct hôte-voyageur | 0 € |
| **Assurance** | Clause de responsabilité signée par l'hôte + mention dans les CGV | 200 € (avocat) |
| **Marketing** | Instagram + 3-5 micro-influenceurs | 500-1 000 € |
| **Total** | | **1 200-2 200 €** |

### 13.2.2 Ce que le MVP ne fait PAS

- Pas d'app native
- Pas de paiement in-app (Stripe Payment Links / virement)
- Pas de système d'avis automatisé
- Pas de pricing dynamique
- Pas de campings classiques
- Pas de multi-langue

### 13.2.3 Timeline du MVP

| Semaine | Activité |
|---|---|
| **S1-S4** | Recrutement de 10-15 propriétaires (visites physiques) |
| **S3-S5** | Construction landing page + fiches terrain + photos |
| **S5** | Consultation juridique (CH) |
| **S5-S6** | Campagne Instagram + influenceurs, ouverture réservations |
| **S6-S14** | Saison active : réservations, feedback, itérations |
| **S14-S16** | Bilan : NPS, conversion, repeat, taux réclamation |

**Durée totale :** ~4 mois (dont 2 mois de saison active)
**Budget total :** ~2 000-3 000 €
**Objectif :** 100 nuitées réservées, NPS > 40, taux de conversion > 3 %

---

## 13.3 Tests terrain complémentaires

### 13.3.1 Test "Le pitch café" (Hypothèse 1)

**Quoi :** Rencontrer 20 propriétaires potentiels en face-à-face autour d'un café, présenter le concept avec un support visuel (mockup de l'app, exemples de terrains similaires), et noter leur réaction.

**Durée :** 2-3 semaines
**Coût :** ~200 € (cafés + déplacements)
**Résultat attendu :** feedback qualitatif (objections, enthousiasme, freins), estimation du taux de conversion

### 13.3.2 Test "Fake door" (Hypothèse 2)

**Quoi :** Créer une page Instagram @nomad.camping avec 20 posts de beaux spots (photos stock/free + vrais terrains), un lien en bio vers une landing page "Réserve ton spot nature", avec un bouton "Réserver" qui mène vers un formulaire d'intérêt (pas encore de vraie réservation).

**Durée :** 3-4 semaines
**Coût :** ~200-400 € (quelques ads Instagram ciblés)
**Metric :** Nombre de clics "Réserver", taux de remplissage du formulaire d'intérêt

### 13.3.3 Test "Le week-end Nomad" (Hypothèses 2 + 4)

**Quoi :** Organiser 5 week-ends test avec des voyageurs recrutés via Instagram/bouche-à-oreille, sur 5 terrains différents. Expérience complète : réservation, accueil, nuit, feedback.

**Durée :** 5-8 semaines (un week-end par semaine)
**Coût :** ~500-800 € (logistique, incentive voyageurs, photos pro)
**Résultat attendu :** NPS précis, retours qualitatifs, contenu photo/vidéo réutilisable, témoignages

---

## 13.4 Indicateurs de succès/échec — Le tableau de bord go/no-go

| Indicateur | Seuil GO ✅ | Seuil PIVOT ⚠️ | Seuil STOP ❌ |
|---|---|---|---|
| **Conversion propriétaire** (pitch → listing) | >30 % | 15-30 % | <15 % |
| **Conversion voyageur** (visite → réservation) | >3 % | 1-3 % | <1 % |
| **Prix moyen accepté** | >25 €/nuit | 15-25 €/nuit | <15 €/nuit |
| **NPS voyageur** | >40 | 20-40 | <20 |
| **Taux de réclamation** | <10 % | 10-25 % | >25 % |
| **Repeat booking** (en saison) | >15 % | 5-15 % | <5 % |
| **Cadre légal** | Clair et permissif | Zones grises gérables | Risque majeur |

### 13.4.1 Scénario GO

Tous les indicateurs au vert → lancer le développement de la plateforme complète (MVP tech), lever le pre-seed (200-300 K€), recruter les 200 premiers terrains.

### 13.4.2 Scénario PIVOT

Certains indicateurs en orange → identifier les freins, adapter le concept :
- Si conversion prix faible → repositionner vers le bas (terrains "basiques" à 15 €)
- Si NPS faible → renforcer la sélection et l'onboarding hôtes
- Si conversion propriétaire faible → tester d'autres profils (campings, gîtes) ou d'autres incentives
- Si cadre légal flou → se limiter à la Suisse (plus permissif) et adapter pour la France

### 13.4.3 Scénario STOP

Indicateurs critiques au rouge → le marché n'existe pas sous cette forme :
- Les propriétaires ne veulent pas → pas d'offre
- Les voyageurs ne paient pas → pas de demande transactionnelle
- Le cadre légal est bloquant → risque juridique trop élevé

**Coût total de la validation avant abandon :** ~3 000-5 000 €. C'est le prix de la certitude — bien moins cher qu'un échec à 200 K€.

---

## 13.5 Calendrier de validation

```
     Mois 1          Mois 2          Mois 3          Mois 4
  ┌───────────┐   ┌───────────┐   ┌───────────┐   ┌───────────┐
  │ Juridique │   │ Pitch café│   │  MVP live  │   │   Bilan   │
  │ (CH)      │   │ + Fake    │   │  100 nuits │   │  Go/No-go │
  │           │   │ door      │   │  actif     │   │           │
  │ Recrut.   │   │           │   │  Weekend   │   │ Décision  │
  │ hôtes     │   │ Landing   │   │  Nomad x5  │   │ investir  │
  │ (visites) │   │ page      │   │            │   │ ou stop   │
  └───────────┘   └───────────┘   └───────────┘   └───────────┘
```

**Investissement total phase validation :** 3 000-5 000 € + 4 mois de temps
**Résultat :** Décision informée GO/PIVOT/STOP avec données réelles

---

## 13.6 Ce qui n'a PAS besoin d'être validé

Pour éviter la "paralysis by analysis", voici ce qui est déjà validé par le marché existant :

- ✅ **La demande de spots nature existe** (6M+ downloads Park4Night)
- ✅ **Le modèle marketplace terrains privés fonctionne** (Nomady, Hipcamp, Campspace existent et ont du revenu)
- ✅ **Les gens paient pour du camping** (113M nuitées/an en France, marché en croissance)
- ✅ **La commission ~15 % est acceptée** (standard du marché, cf. section 8)

**Ce qui reste à valider :** est-ce que ÇA fonctionne, ICI, MAINTENANT, avec CETTE exécution. C'est exactement ce que le plan ci-dessus teste.

---

## Sources

1. Section 8 — Modèle économique (unit economics, pricing, projections)
2. Section 9 — Stratégie GTM (timeline, acquisition supply, géographie)
3. Section 10 — Stratégie de défense (moats, risques)
4. Eric Ries — *The Lean Startup* (méthodologie MVP et validation)
5. Ash Maurya — *Running Lean* (hypothèses critiques, go/no-go)
6. Lenny's Newsletter — "How to validate marketplace ideas" (frameworks)
