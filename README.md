# FOD — figuringOutDiabetes Tools

Free, evidence-based diabetes tools for busy people managing or at risk of diabetes. Designed for Squarespace embedding via iframe — no backend, no sign-up, no tracking.

## What's here

| | URL | What it is |
|---|---|---|
| 🍚 | **[/](https://fodhub2026.github.io/fod-gi-database/)** | **GI Database** — 485 foods, 547 rows, Indian-context GI/GL reference with built-in calculator |
| 🧮 | **[/calculators/](https://fodhub2026.github.io/fod-gi-database/calculators/)** | **Calculator hub** — directory of all 69 FOD calculators, grouped by category |
| | `/calculators/<slug>.html` | One self-contained page per calculator (69 of them) |

---

## Live URLs

### Top-level

- **GI Database:** https://fodhub2026.github.io/fod-gi-database/
- **Calculator hub:** https://fodhub2026.github.io/fod-gi-database/calculators/

### Individual calculators (69)

Each lives at `https://fodhub2026.github.io/fod-gi-database/calculators/<slug>.html`

**Carbs & food**
`glycemic-load` · `gi-impact-estimator` · `net-carbs` · `carb-counting` · `fiber-intake` · `portion-to-carb` · `sugar-equivalent` · `recipe-gi-estimator` · `indian-food-gi-lookup` · `meal-spike-predictor` · `protein-fat-delay`

**Insulin & dosing**
`insulin-to-carb-ratio` · `correction-factor` · `insulin-sensitivity-factor` · `total-daily-insulin` · `basal-bolus-split` · `insulin-dose-adjustment` · `insulin-stacking-risk` · `missed-dose-impact` · `injection-timing-impact`

**Glucose monitoring**
`hba1c-to-glucose` · `estimated-hba1c` · `hba1c-timeline` · `time-in-range` · `glucose-variability` · `average-blood-glucose` · `cgm-dashboard` · `hypo-frequency` · `hyper-frequency` · `fasting-vs-postmeal` · `consistency-score`

**Risk & complications**
`cv-risk` · `complication-risk` · `foot-risk` · `pre-diabetes-risk` · `hypo-risk-score` · `fasting-risk` · `sedentary-risk` · `remission-probability` · `diabetes-type-assessment` · `egfr` · `medication-eligibility`

**Body & metabolism**
`bmi` · `bmr` · `body-fat-percentage` · `ideal-body-weight` · `daily-calorie-requirement` · `steps-to-calories` · `walking-impact` · `exercise-glucose-drop`

**Lifestyle & context**
`sleep-glucose` · `stress-impact` · `hydration-impact` · `alcohol-impact` · `sick-day-impact` · `ramadan-fasting-risk` · `shift-work-adjustment` · `travel-timezone`

**Cost & access**
`annual-cost` · `monthly-cost` · `cost-per-reading` · `insurance-vs-selfpay` · `non-adherence-cost`

**Special situations & support**
`pregnancy-bg-targets` · `diabetes-distress` · `caregiver-burden` · `emergency-plan` · `bad-day-recovery` · `shared-glucose-review`

---

## How to embed in Squarespace

Each tool is iframe-friendly. Use a **Code Block** (Business plan +) or **Embed Block**.

### Embed the GI database
```html
<iframe src="https://fodhub2026.github.io/fod-gi-database/"
  style="width:100%;height:1600px;border:0;display:block"
  loading="lazy" title="FOD GI Database"></iframe>
```

### Embed the calculator hub (browse all 69)
```html
<iframe src="https://fodhub2026.github.io/fod-gi-database/calculators/"
  style="width:100%;height:2200px;border:0;display:block"
  loading="lazy" title="FOD Calculators"></iframe>
```

### Embed a single calculator (example: Glycemic Load)
```html
<iframe src="https://fodhub2026.github.io/fod-gi-database/calculators/glycemic-load.html"
  style="width:100%;height:1400px;border:0;display:block"
  loading="lazy" title="Glycemic Load Calculator"></iframe>
```

Adjust `height` per page. Most calculators sit between 1200–1800 px tall.

### Recommended Squarespace structure

- `/tools` page → embed the **calculator hub** so visitors can browse all 69
- `/tools/glycemic-load` page → embed the **single calculator** with surrounding intro / FAQ for SEO
- `/tools/bmi` page → same pattern, deep-link your top calculators for organic search

---

## Updating in the future

When new data or new calculators arrive:
1. Send the new file(s) to your AI builder.
2. Get a fresh single-file HTML.
3. In GitHub: open the file → **Edit** (pencil) → paste new content → Commit.
4. GitHub Pages rebuilds in ~30s. Squarespace embed updates automatically.

---

## Files in this repo

| Path | Notes |
|---|---|
| `index.html` | GI Database — single self-contained page (~600 KB, includes data + logo + JS) |
| `calculators/index.html` | Calculator hub — searchable, categorised |
| `calculators/<slug>.html` | 69 individual calculators, each ~50 KB |
| `calculators/AUDIT-SUMMARY.md` | Build report (per-calculator audit) |
| `README.md` | This file |

---

## Data sources & methodology

- Atkinson FS, Foster-Powell K, Brand-Miller JC. *International tables of glycemic index and glycemic load values 2021.* Am J Clin Nutr. (DOI: 10.1093/ajcn/nqab233)
- ICMR-NIN Indian Food Composition Tables
- Peer-reviewed Indian glycemic studies (PubMed)
- Calculator formulas follow standard clinical references (ADA, IDF, Lloyd-Jones for CV risk, IDF-DAR for Ramadan, etc.)

---

## Disclaimer

Educational reference. **Not medical advice.** Always confirm with your clinician or registered dietitian. GI/GL responses and dosing needs are individual.

---

© figuringOutDiabetes — released for free public use.
