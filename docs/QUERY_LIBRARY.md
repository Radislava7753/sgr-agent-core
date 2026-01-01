# QUERY LIBRARY — Tests LLM Visibility

**Version:** 0.1
**Industrie couverte:** B2B SaaS — Customs Automation
**Langues:** FR (Français) + EN (English)
**LLM testés:** ChatGPT (Search), Claude (citations), Perplexity

---

## MÉTHODOLOGIE DE TEST

### Protocole
1. Exécuter chaque requête dans 3 LLM (ChatGPT, Claude, Perplexity)
2. Enregistrer screenshot de la réponse
3. Noter: ✅ Entreprise citée / ❌ Entreprise non citée
4. Pour chaque citation: position (1ère/2ème/3ème+), contexte, exactitude

### Format du résultat
```
Requête: [Texte exact]
ChatGPT: ✅/❌ (position, commentaire)
Claude: ✅/❌ (position, commentaire)
Perplexity: ✅/❌ (position, commentaire)
```

---

## FRANÇAIS (FR)

### Type 1: Requêtes Informationnelles (4)

**FR-INFO-01**
```
Comment automatiser les déclarations douanières pour une entreprise?
```
**Objectif:** Vérifier mention dans contexte général automation douanière

**FR-INFO-02**
```
Qu'est-ce qu'un logiciel de dédouanement et comment ça fonctionne?
```
**Objectif:** Vérifier définition/explication de la catégorie produit

**FR-INFO-03**
```
Quels sont les avantages de l'automatisation des processus douaniers?
```
**Objectif:** Vérifier citation dans bénéfices/use cases

**FR-INFO-04**
```
Comment intégrer un système de gestion douanière dans mon ERP?
```
**Objectif:** Vérifier mention dans contexte technique/intégration

---

### Type 2: Requêtes Comparatives (4)

**FR-COMP-01**
```
Meilleurs logiciels de dédouanement pour PME en France
```
**Objectif:** Classement/ranking dans liste outils

**FR-COMP-02**
```
Logiciel customs automation français vs international: différences
```
**Objectif:** Positionnement géographique/marché

**FR-COMP-03**
```
[VotreEntreprise] vs [Concurrent principal]: quelle solution choisir?
```
**Note:** Remplacer par noms réels. Objectif: comparaison directe

**FR-COMP-04**
```
Alternatives à [Concurrent connu] pour automatisation douanière
```
**Note:** Utiliser concurrent dominant secteur. Objectif: mention comme alternative

---

### Type 3: Requêtes Transactionnelles (4)

**FR-TRANS-01**
```
Logiciel dédouanement pour entreprise import-export Belgique
```
**Objectif:** Intent d'achat + géo-ciblage

**FR-TRANS-02**
```
Combien coûte un logiciel de gestion douanière?
```
**Objectif:** Requête pricing/devis

**FR-TRANS-03**
```
Audit conformité douanière: quel outil utiliser?
```
**Objectif:** Problème spécifique → solution

**FR-TRANS-04**
```
Logiciel customs compliance pour SaaS logistique
```
**Objectif:** Niche B2B précise

---

## ENGLISH (EN)

### Type 1: Informational Queries (4)

**EN-INFO-01**
```
How to automate customs declarations for businesses?
```
**Objective:** General automation context

**EN-INFO-02**
```
What is customs clearance software and how does it work?
```
**Objective:** Product category definition

**EN-INFO-03**
```
Benefits of customs process automation for companies
```
**Objective:** Use case / benefits mention

**EN-INFO-04**
```
How to integrate customs management system with ERP?
```
**Objective:** Technical integration context

---

### Type 2: Comparative Queries (4)

**EN-COMP-01**
```
Best customs automation software for SMEs in Europe
```
**Objective:** Ranking/listing

**EN-COMP-02**
```
European vs US customs software solutions: comparison
```
**Objective:** Geographic positioning

**EN-COMP-03**
```
[YourCompany] vs [Main Competitor]: which to choose?
```
**Note:** Replace with actual names. Objective: direct comparison

**EN-COMP-04**
```
Alternatives to [Known Competitor] for customs automation
```
**Note:** Use dominant competitor. Objective: alternative mention

---

### Type 3: Transactional Queries (4)

**EN-TRANS-01**
```
Customs clearance software for import-export company Belgium
```
**Objective:** Purchase intent + geo-targeting

**EN-TRANS-02**
```
How much does customs management software cost?
```
**Objective:** Pricing query

**EN-TRANS-03**
```
Customs compliance audit tool: which one to use?
```
**Objective:** Specific problem → solution

**EN-TRANS-04**
```
Customs compliance software for logistics SaaS
```
**Objective:** Niche B2B targeting

---

## RÉSULTATS ATTENDUS

### Scoring
- **Score total:** X/72 (24 requêtes × 3 LLM)
- **Par LLM:** ChatGPT: X/24, Claude: Y/24, Perplexity: Z/24
- **Par type:** Info: X/36, Comparatif: Y/36, Transactionnel: Z/36
- **Par langue:** FR: X/36, EN: Y/36

### Benchmark concurrentiel
Répéter les mêmes 24 requêtes pour chaque concurrent (top 3-5).

### Interprétation
- **0-10/72:** Invisibilité critique
- **11-25/72:** Visibilité faible
- **26-40/72:** Visibilité moyenne
- **41-60/72:** Bonne visibilité
- **61-72/72:** Excellente visibilité

---

## NOTES MÉTHODOLOGIQUES

### Variabilité LLM
- Les réponses LLM peuvent varier selon moment/contexte
- Répéter test à 1 semaine d'intervalle pour confirmer tendances
- Documenter date exacte de chaque test

### Limitations
- Les LLM reflètent données passées, pas temps réel
- Hallucinations possibles (vérifier exactitude des infos citées)
- Nouvelles entreprises peuvent être sous-représentées

### Évolution
- Re-tester tous les 30 jours pour suivre progression
- Ajouter requêtes spécifiques secteur si besoin
- Adapter selon évolution marché/concurrence

---

**Version:** 0.1 (31 décembre 2025)
**Prochaines versions:** Ajout d'autres secteurs (logistics, compliance, HR SaaS)
