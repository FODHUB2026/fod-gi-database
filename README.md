# FOD Glycemic Index Database

A free, interactive, Indian-context Glycemic Index & Glycemic Load reference, with a built-in GL calculator.

**Live demo:** _set after GitHub Pages is enabled_

- **485 unique foods** · **547 food/preparation rows** · evidence-graded (A/B/C)
- Search by English, Hindi (Latin), or alias
- Filter by GI band, category, evidence quality, Indian-staple
- Live GI / GL calculator with portion + servings inputs
- Mobile-optimised (card layout under 640px)
- Single self-contained `index.html` — no build step, no dependencies

---

## How to publish on Squarespace

### Option 1 — GitHub Pages + Embed Block (recommended, works on all Squarespace plans)

1. **Create a new GitHub repo** named e.g. `fod-gi-database` (public).
2. Upload `index.html` to the root of the repo.
3. In the repo: **Settings → Pages → Build from `main` branch → `/ (root)` → Save.**
4. Wait ~1 minute. GitHub gives you a URL like
   `https://<your-username>.github.io/fod-gi-database/`
5. Open that URL in a new tab to confirm it loads.
6. In Squarespace: **Edit page → Insert block → Embed → "Code Snippet" / "iframe"** and paste:

   ```html
   <iframe
     src="https://<your-username>.github.io/fod-gi-database/"
     style="width:100%;height:1600px;border:0;display:block"
     loading="lazy"
     title="FOD Glycemic Index Database">
   </iframe>
   ```

7. Adjust `height:1600px` if your page needs more/less vertical space.

> **Tip:** Squarespace's basic Embed Block sometimes only takes a URL. Use the **Code Block** (Business plan +) for the iframe snippet above, or use the **Embed Block** with just the URL — Squarespace will auto-iframe it.

### Option 2 — Paste full HTML into a Code Block (Business plan and above)

Open `index.html`, copy everything, paste into a Squarespace Code Block. No GitHub needed — but every update means re-pasting.

---

## How to update the database

When new GI data arrives, you regenerate `index.html` and push the updated file. The Squarespace embed updates instantly because it points to the same URL.

**Workflow:**
1. Send the new food rows (or updated CSVs) to your AI builder.
2. Get a fresh `index.html`.
3. In GitHub: open `index.html` → **Edit (pencil icon)** → paste the new content → Commit. Done.

---

## Files in this repo

| File | What it is |
|---|---|
| `index.html` | The interactive database (single file, ~600 KB, includes data + logo + JS) |
| `README.md` | This file |

---

## Data sources

- **Atkinson FS, Foster-Powell K, Brand-Miller JC.** *International tables of glycemic index and glycemic load values 2021.* Am J Clin Nutr. (DOI: 10.1093/ajcn/nqab233)
- **ICMR-NIN** Indian Food Composition Tables
- Peer-reviewed Indian glycemic studies indexed in PubMed
- See `figuringOutDiabetes.com` for full methodology

---

## Disclaimer

Educational reference. **Not medical advice.** Always confirm dietary decisions with your clinician or registered dietitian. GI/GL responses are individual — what matters more than any single number is the overall meal pattern, fiber, protein, fat, and your post-meal movement.

---

© figuringOutDiabetes — released for free public use.
