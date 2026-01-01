# PROJECT CONTEXT — SGR Agent Core

**Master reference for AI agents working on this project**
**Version:** 0.1
**Last updated:** 2026-01-01

---

## 1. Цель проекта
(Что именно продаётся, кому и зачем)

**Продукт:** Audit de Visibilité Numérique & LLM
**Клиент:** B2B SaaS компании (PME, ETI), которые невидимы в ChatGPT/Claude/Perplexity
**Ценность:** Фактическая диагностика цифрового следа + roadmap конкретных действий (не обещания трафика)

**Формат доставки:**
- PDF-отчёт (8-12 страниц) с проверяемыми фактами
- Приоритизированная roadmap (quick wins + 60-дневный план)
- Конкурентный бенчмарк (где вы vs где конкуренты)

**Философия:** Честный аудит. Мы не гарантируем "доминирование в LLM", мы показываем реальное состояние и объясняем, почему оно такое.

---

## 2. Текущий статус (на сегодня)

**Codex:**
- ✅ Docs structure created
- ✅ AUDIT_METHODOLOGY.md v0.1 documented
- ✅ REPORT_STRUCTURE.md v0.1 defined
- ✅ CASELOG.md v0.1 initialized
- ✅ INTAKE_FORM.md ready for client intake
- ✅ QUERY_LIBRARY.md (24 queries FR/EN)
- ✅ CRITERIA_BENCHMARKS.md (evaluation thresholds)

**SGR Agent Core:**
- ❌ NOT installed yet (dependency installation pending)
- ❌ NOT configured (config.yaml not set up)
- ❌ NOT tested (no sample runs)

**Audits:**
- ❌ 0 completed
- ❌ 0 in progress
- ❌ CASELOG.md empty (awaiting first case)

**Website/Marketing:**
- ❌ No landing page
- ❌ No client acquisition funnel
- ❌ No case studies (obviously, since 0 audits done)

---

## 3. Principes (GALA — кратко)

**GALA = Guiding Architecture & Living Assumptions**

Core principles established in README.md:

1. **Real practice first, scale second**
   - Ne jamais promettre ce qui n'a pas été testé
   - Documenter ce qui fonctionne réellement
   - Itérer basé sur l'évidence, pas la théorie

2. **No audits without evidence**
   - Chaque recommandation doit être vérifiable
   - Pas de "best practices" sans test réel
   - Benchmarks basés sur observations, pas spéculations

3. **No selling without doing**
   - Pas de clients avant le 1er audit de démonstration
   - Pas de "success stories" sans cas réels
   - Pas de promesses de ROI sans données

4. **Fix decisions, don't rethink endlessly**
   - Méthodologie v0.1 est fixée → exécuter, pas rediscuter
   - Format docs accepté → utiliser, pas réinventer
   - Critères définis → appliquer, affiner après 10 cas

---

## 4. Что уже решено (DO NOT REDECIDE)

**Ces décisions sont CLOSES. Ne pas rediscuter.**

### Méthodologie
- ✅ AUDIT_METHODOLOGY.md v0.1 **accepted as-is**
- ✅ 6 phases audit (Intake → Tech → Semantic → LLM → Competitive → Roadmap)
- ✅ 12 requêtes FR + 12 EN (QUERY_LIBRARY.md) **fixed**
- ✅ Scoring 0-72 (24 queries × 3 LLM) **standardized**

### Format livrables
- ✅ REPORT_STRUCTURE.md v0.1 **template locked**
- ✅ PDF 8-12 pages (Executive Summary + 6 sections + Appendices)
- ✅ Roadmap: Quick Wins (0-7j) / Moyen (2-4 sem) / Long terme (3-6 mois)

### Critères évaluation
- ✅ CRITERIA_BENCHMARKS.md v0.1 **thresholds set**
- ✅ Schema.org minimum: Organization + FAQPage (10+ questions)
- ✅ LLM visibility tiers: < 10/72 = Critical, 41-60 = Good, 61+ = Excellent

### Premier cas
- ✅ **Cas #001 = audit d'apprentissage public B2B SaaS**
- ✅ Objectif: tester méthodologie end-to-end
- ✅ Résultat documenté dans CASELOG.md (post-audit)
- ✅ Pas de client payant avant validation Cas #001

---

## 5. Чего НЕ делать

**STOP-LIST — actions interdites avant premier audit réel**

### ❌ NE PAS étendre scope
- Pas de nouveaux documents méthodologiques
- Pas de frameworks additionnels
- Pas d'outils complexes (rester SGR Agent Core + manuel)
- Pas de multilangues au-delà de FR/EN

### ❌ NE PAS optimiser prématurément
- Pas de site web avant avoir 3 cas
- Pas de branding/design avant avoir preuve concept
- Pas de automation avant processus manuel validé
- Pas de scale tools avant 10 audits manuels

### ❌ NE PAS écrire contenu marketing
- Pas de landing page "pourquoi LLM visibility matters"
- Pas de blog posts théoriques
- Pas de "success stories" inventées
- Pas de promesses ROI sans data

### ❌ NE PAS rediscuter décisions closes
- Méthodologie v0.1 → exécuter, pas débattre
- Format docs → utiliser, pas réinventer
- Critères benchmark → appliquer, affiner après usage réel

---

## 6. Ближайший обязательный шаг

**NEXT MANDATORY ACTION:**

### → Audit #001: Public Learning Case

**Objectif:**
Exécuter méthodologie complète sur un cas B2B SaaS réel (peut être fictif ou cas d'étude public).

**Deliverables obligatoires:**
1. ✅ Remplir INTAKE_FORM.md (même si fictif)
2. ✅ Exécuter 24 requêtes (QUERY_LIBRARY.md) dans 3 LLM
3. ✅ Appliquer CRITERIA_BENCHMARKS.md (scoring technique + LLM)
4. ✅ Générer rapport selon REPORT_STRUCTURE.md
5. ✅ Documenter learnings dans CASELOG.md

**Durée estimée:** 2-3 jours (si SGR Agent Core opérationnel)

**Critère succès:**
- Rapport PDF complet généré
- CASELOG.md Case #001 complété
- Au moins 3 learnings documentés ("ce qui a marché" / "ce qui n'a pas marché")

**Blocker actuel:**
- SGR Agent Core not installed/configured
- Need: `uv sync` + config setup + test run

---

## 7. Как ИИ должен помогать

**Guidelines for AI agents assisting this project:**

### ✅ DO: Help move forward step-by-step
- Rappeler le next mandatory step (Audit #001)
- Proposer actions concrètes alignées avec docs/
- Pointer vers AUDIT_METHODOLOGY.md quand incertitude processus
- Utiliser CRITERIA_BENCHMARKS.md pour évaluation objective

### ✅ DO: Stop perfectionism drift
- Si humain veut "améliorer méthodologie" → rappeler "exécuter d'abord, affiner après"
- Si propose nouveau doc → rappeler "scope closed, use existing"
- Si veut optimiser avant usage → rappeler "practice first, scale second"

### ✅ DO: Reference existing docs, don't invent
- TOUJOURS citer section exacte de docs/ (ex: "AUDIT_METHODOLOGY.md § 2.4")
- Ne JAMAIS inventer critères non documentés
- Si gap trouvé → noter pour v0.2, mais utiliser v0.1 pour l'instant

### ❌ DON'T: Propose expansions
- Ne pas suggérer "aussi on pourrait faire X"
- Ne pas proposer outils additionnels
- Ne pas recommander refonte avant 1er audit complet

### ❌ DON'T: Rediscuss closed decisions
- Méthodologie v0.1 est fixe → ne pas proposer changements
- Format docs locked → ne pas suggérer alternatives
- Critères définis → ne pas débattre seuils

### 🎯 Role: Execution facilitator, not strategy consultant
**Your job:** Help execute what's decided.
**Not your job:** Redecide strategy or expand scope.

---

## Meta-Note for AI Context Transfer

**When resuming work on this project in new chat:**

1. Read this file FIRST (PROJECT_CONTEXT.md)
2. Check CASELOG.md to see completed audits
3. Reference AUDIT_METHODOLOGY.md for process questions
4. Use CRITERIA_BENCHMARKS.md for evaluation questions
5. Remind human of "next mandatory step" if they deviate

**This file is the single source of truth for:**
- What's decided (§4)
- What NOT to do (§5)
- What's the priority (§6)
- How to assist effectively (§7)

**Update this file only when:**
- Audit #001 completed → update §2 status
- Major milestone reached (ex: 10 audits done, v0.2 methodology locked)
- Scope intentionally expanded by project owner (explicit decision)

---

**Version history:**
- v0.1 (2026-01-01): Initial project context established
