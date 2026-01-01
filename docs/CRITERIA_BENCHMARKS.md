# CRITERIA & BENCHMARKS — Seuils d'évaluation

**Version:** 0.1
**Objectif:** Passer de données brutes à jugements clairs (✅ / ⚠️ / ❌)
**Application:** B2B SaaS (focus customs automation, applicable autres secteurs)

---

## 1. CRITÈRES TECHNIQUES

### 1.1 Vitesse du site

| Métrique | ✅ Excellent | ⚠️ Acceptable | ❌ Problématique |
|----------|--------------|---------------|------------------|
| **Temps de réponse serveur (TTFB)** | < 0.5 sec | 0.5-1.5 sec | > 1.5 sec |
| **First Contentful Paint (FCP)** | < 1.8 sec | 1.8-3 sec | > 3 sec |
| **Largest Contentful Paint (LCP)** | < 2.5 sec | 2.5-4 sec | > 4 sec |
| **Cumulative Layout Shift (CLS)** | < 0.1 | 0.1-0.25 | > 0.25 |

**Outil de mesure:** Google PageSpeed Insights
**Seuil minimum acceptable:** LCP < 4 sec (sinon action immédiate requise)

---

### 1.2 Mobile-friendliness

| Critère | ✅ OK | ❌ Problème |
|---------|-------|-------------|
| **Google Mobile-Friendly Test** | Pass | Fail |
| **Responsive design** | Adapté tous écrans | Défilement horizontal |
| **Texte lisible sans zoom** | Oui | Non |
| **Boutons cliquables (espacement)** | > 48px | < 48px |

**Outil de mesure:** Google Mobile-Friendly Test
**Seuil minimum:** DOIT passer Mobile-Friendly Test

---

### 1.3 Crawlabilité

| Élément | ✅ Optimal | ⚠️ À améliorer | ❌ Bloquant |
|---------|-----------|----------------|-------------|
| **robots.txt** | Permet tous crawlers importants | Bloque crawlers mineurs | Bloque Googlebot/GPTBot/ClaudeBot |
| **sitemap.xml** | Présent, < 1000 URLs, à jour (< 30j) | Présent mais ancien | Absent ou 404 |
| **Statut HTTP homepage** | 200 OK | 301 redirect | 404/500/503 |
| **Temps de crawl (10 pages)** | < 5 sec total | 5-15 sec | > 15 sec |

**Outils:** View source, Screaming Frog (gratuit 500 URLs)
**Blocker absolu:** robots.txt interdisant GPTBot/ClaudeBot/PerplexityBot

---

### 1.4 Données structurées (Schema.org)

| Type de markup | ✅ Présent et valide | ⚠️ Présent mais incomplet | ❌ Absent |
|----------------|---------------------|---------------------------|-----------|
| **Organization** | Nom, URL, logo, address | Nom, URL seulement | Rien |
| **WebSite** | name, url, potentialAction (search) | name, url | Rien |
| **FAQPage** | 10+ questions bien structurées | 1-5 questions | Rien |
| **BreadcrumbList** | Présent (si site > 2 niveaux) | — | Absent |
| **Service / Product** | Description complète + prix | Description seule | Rien |

**Outil de validation:** Google Rich Results Test
**Minimum B2B SaaS:** Organization + FAQPage (au moins 10 questions)

---

## 2. CRITÈRES SÉMANTIQUES

### 2.1 Structure de contenu

| Critère | ✅ Optimal | ⚠️ Acceptable | ❌ Insuffisant |
|---------|-----------|---------------|----------------|
| **H1 unique par page** | Oui, descriptif (50-70 car) | Oui mais générique | Multiple H1 ou absent |
| **Hiérarchie H2-H3** | Logique, 3-5 H2 par page | Présente mais désordonnée | Absente |
| **Longueur homepage** | 800-1500 mots | 400-800 mots | < 400 mots |
| **Longueur page service** | 600-1200 mots | 300-600 mots | < 300 mots |
| **Meta description** | 140-155 car, unique | 100-140 car | Absente ou dupliquée |

**Note:** Pour B2B SaaS, la qualité > quantité (éviter remplissage)

---

### 2.2 FAQ (Foire Aux Questions)

| Métrique | ✅ Excellent | ⚠️ Minimum | ❌ Insuffisant |
|----------|--------------|------------|----------------|
| **Nombre de questions** | 15-25 | 8-14 | < 8 ou absent |
| **Markup FAQPage** | Présent et valide | Présent mais erreurs | Absent |
| **Qualité questions** | Naturelles, issues clients réels | Génériques mais utiles | Marketing fluff |
| **Longueur réponses** | 50-150 mots/réponse | 20-50 mots | < 20 mots |

**B2B SaaS minimum:** 10 FAQ avec markup FAQPage valide

---

### 2.3 Densité sémantique (mots-clés)

| Métrique | ✅ Optimal | ⚠️ Acceptable | ❌ Problème |
|----------|-----------|---------------|-------------|
| **Densité mot-clé principal** | 1.5-3% | 0.8-1.5% ou 3-5% | < 0.5% ou > 5% |
| **Variantes sémantiques** | 5-10 variantes utilisées | 2-4 variantes | 0-1 variante |
| **Formules répétitives (ancrage)** | 3-5 fois même formule clé | 1-2 fois | 0 fois |

**Exemple formule répétitive (customs):**
"Automatisation des déclarations douanières en 48h" → répété 3x dans page

**Outil:** Analyse manuelle ou tools comme Yoast (WordPress)

---

### 2.4 Fraîcheur du contenu

| Indicateur | ✅ Bon | ⚠️ Moyen | ❌ Obsolète |
|------------|--------|----------|-------------|
| **Date dernière mise à jour (homepage)** | < 3 mois | 3-12 mois | > 12 mois |
| **Date dernière mise à jour (blog)** | < 1 mois | 1-6 mois | > 6 mois ou pas de blog |
| **Présence "2024/2025" dans textes** | Oui | Mention "2023" | Mention "2022" ou antérieur |

**Action si obsolète:** Mettre à jour au moins homepage + ajouter date visible

---

## 3. CRITÈRES LLM VISIBILITY

### 3.1 Score de visibilité

| Score (sur 72)* | ✅ Très bon | ⚠️ Moyen | ❌ Faible |
|-----------------|------------|----------|-----------|
| **Mentions totales** | 41-72 | 15-40 | 0-14 |
| **Par LLM (sur 24)** | 15-24 | 6-14 | 0-5 |
| **Par type requête (sur 36)** | 15-36 | 6-14 | 0-5 |

*24 requêtes × 3 LLM = 72 tests max

**Interprétation:**
- < 10/72 = Invisibilité critique (priorité #1)
- 10-25/72 = Visibilité faible (action nécessaire)
- 26-40/72 = Visibilité moyenne (optimisation souhaitable)
- 41-60/72 = Bonne visibilité (maintien)
- 61-72/72 = Excellente visibilité (rare, benchmark à étudier)

---

### 3.2 Qualité des mentions

| Critère | ✅ Optimal | ⚠️ Acceptable | ❌ Problématique |
|---------|-----------|---------------|------------------|
| **Position dans réponse** | 1ère-2ème mention | 3ème-5ème mention | > 5ème ou absence |
| **Exactitude informations** | 100% correct | Majoritairement correct | Erreurs factuelles |
| **Contexte de citation** | Positif/neutre, pertinent | Neutre, contexte limité | Négatif ou hors-sujet |
| **Présence lien/source** | Oui, vers site officiel | Oui mais source tierce | Non |

**Red flag:** Si LLM invente infos fausses → vérifier cohérence NAP

---

### 3.3 Consistance inter-LLM

| Métrique | ✅ Bon | ⚠️ Variable | ❌ Incohérent |
|----------|--------|-------------|---------------|
| **Même info dans 3 LLM** | Oui (cohérence 100%) | Partiellement (50-90%) | Non (< 50%) |
| **Nom entreprise identique** | Oui | Variantes mineures | Noms différents |
| **Description produit similaire** | Oui | Partiellement | Contradictoire |

**Si incohérent:** Problème de données structurées ou NAP inconsistant

---

## 4. CRITÈRES CONCURRENTIELS

### 4.1 Position relative

| Position vs concurrents (top 5) | Interprétation |
|--------------------------------|----------------|
| **1er (score LLM le plus élevé)** | Leader de visibilité ✅ |
| **2ème-3ème** | Bonne position ✅ |
| **4ème-5ème** | Position faible ⚠️ |
| **Dernier ou absent** | Invisible ❌ |

---

### 4.2 Écart de maturité technique

| Critère | Vous | Meilleur concurrent | Gap | Priorité |
|---------|------|---------------------|-----|----------|
| Schema.org Organization | ❌ | ✅ | -1 | Haute |
| FAQPage (10+ Q) | ❌ | ✅ | -1 | Haute |
| Vitesse (LCP < 2.5s) | ⚠️ | ✅ | -0.5 | Moyenne |
| Présence Capterra/G2 | ❌ | ✅ | -1 | Moyenne |

**Calcul gap total:** Somme des -1, -0.5
**Gap > 3:** Action urgente requise

---

## 5. PRIORITISATION ACTIONS

### 5.1 Matrice Impact × Effort

| Impact | Effort | Score | Catégorie | Exemple |
|--------|--------|-------|-----------|---------|
| **Élevé (5)** | **Faible (1)** | 5.0 | Quick Win ✅ | Ajouter Schema.org |
| **Élevé (5)** | **Moyen (3)** | 1.7 | Moyen | Créer 15 FAQ |
| **Élevé (5)** | **Élevé (5)** | 1.0 | Long terme | Refonte complète |
| **Moyen (3)** | **Faible (1)** | 3.0 | Quick Win ✅ | Corriger robots.txt |
| **Faible (2)** | **Élevé (5)** | 0.4 | Éviter ❌ | Optimisation mineure complexe |

**Formule:** Score = Impact / Effort
**Seuil Quick Win:** Score > 2.0

---

### 5.2 Classification temporelle

| Timeframe | Effort | Budget | Exemples |
|-----------|--------|--------|----------|
| **Quick Wins (0-7j)** | < 2h | 0€ | Schema.org, robots.txt, NAP fix |
| **Moyen (2-4 sem)** | 2-10h | 0-500€ | FAQ complet, optimisation textes |
| **Long terme (3-6 mois)** | > 10h | 500€+ | Refonte, stratégie contenu |

---

## NOTES DE VERSION

**v0.1 (31 décembre 2025)**
- Seuils initiaux basés sur best practices SEO/GEO
- À ajuster après 10 premiers audits réels
- Benchmarks secteur à affiner (actuellement B2B SaaS générique)

**Prochaines versions:**
- Benchmarks par sous-secteur (customs vs logistics vs HR)
- Seuils géographiques (France vs Belgique vs Québec)
- Critères spécifiques e-commerce, services professionnels
