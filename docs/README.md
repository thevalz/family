# Newborn Glucose Tracking

A small, self-contained tool to understand the relationship between **IV dextrose**,
**formula feeds**, and **blood sugar** over time for a newborn being treated for
hypoglycemia in the NICU — and to watch the dextrose drip being weaned as he takes
over on his own.

This is **not** a "blood sugar below the danger line" chart. It's an intake ↔ response
picture: how much glucose is going in (IV + feeds), how hard the drip is working (GIR),
and how his sugar responds.

> Personal tracking aid — **not medical advice.** The NICU team's readings and orders
> are always the authority.

## Install it on your iPad (or phone) as an app

This folder is a **GitHub Pages** site and an installable **PWA**. Once Pages is enabled
(see below), open the published URL in Safari, then **Share → Add to Home Screen**. It
gets the blood-drop icon, opens full-screen with no browser chrome, and works offline.

**Enabling GitHub Pages (one-time, in the GitHub website):**
1. Repo **Settings → Pages**.
2. Under **Build and deployment → Source**, pick **Deploy from a branch**.
3. Branch: **`claude/family-empty-repo-prp7O`**, folder: **`/docs`** → **Save**.
4. Wait ~1 minute; the published URL will be **https://thevalz.github.io/family/**.

> Privacy note: on a public repo this URL (and the sugar data embedded in it) is publicly
> reachable by anyone who has the link. Keep the repo private + a paid GitHub plan, or accept
> that exposure, per your preference.

## Files

| File | What it is |
|---|---|
| [`index.html`](index.html) | The app. Open in any browser — no install needed; charts, a full data table, and a form to log readings. |
| [`readings.csv`](readings.csv) | Plain-text master log (open in Excel / Sheets): `date, time, dextrose, iv_rate_ml_per_hr, blood_sugar_mg_dl, formula_ml, fortification_kcal_oz, breast_milk_ml`. |
| `manifest.webmanifest`, `sw.js`, `icon-*.png` | PWA plumbing — app name, icon, and offline service worker. |
| `README.md` | This page. |

The app renders from an embedded `READINGS` array (a static page can't read a local CSV
directly), so `readings.csv` and that array are the same data kept in sync — edit the CSV
to confirm/correct values and the array is updated to match.

## The baby

- Born **July 2, 8:18 AM**.
- Birth weight **10 lb 2 oz = 4.59 kg** (large for gestational age).
- Fed **Enfamil Gentlease** (fortified to 20, then 24 kcal/oz), with **breast milk**
  being introduced, while on a continuous **D20** (20% dextrose) IV drip.

Weight and birth time are the two constants at the top of `index.html`. Weight drives
every GIR number; birth time drives the **hours-of-life** axis — toggle the timeline
between **Clock time** and **Hours of life**, and the clinically meaningful **48h** and
**72h** boundaries show as vertical marks. (48h is when the weaning thresholds step up
from >50/>60 to >65/>75 — the reference lines on the blood-sugar chart shift with it.)

## The measures (and where they come from)

**GIR — Glucose Infusion Rate** — the number the NICU titrates, in mg/kg/min:

```
GIR = (%dextrose × IV rate mL/hr) / (6 × weight kg)
```

At 4.59 kg: **D20 @ 13 mL/hr = 9.4**, **D20 @ 12 mL/hr = 8.7 mg/kg/min**.
Source: Brigham & Women's / CWN "WNH G.1" neonatal glucose pathway (referencing
Chowning & Adamkin, *J Perinatol* 2015).

**Weaning the drip** — the pathway weans *in GIR units*, gated by blood sugar
(first 48h): wean GIR by **0.5 if BG > 50**, by **1.0 if BG > 60**. A GIR above
**~8** is considered high support. He's above it — which is the quantitative way of
seeing that he genuinely needs the drip right now, and why weaning is gradual.

**The fluid budget** — total intake (IV + feeds) is capped near **100 mL/kg/day**
(~459 mL/day for him). This is *why* the drip must come down as feeds go up: every mL
of formula he tolerates buys back a mL of IV dextrose — as long as his sugar holds.
Source: Giouleka et al., *Children* 2023 (guideline comparison).

**Formula's contribution** — feed volume × the formula's carbohydrate per 100 mL gives
the glucose from feeds. Fat and protein feed the gluconeogenesis machinery that steadies
his sugar between feeds. The formula profile is a single editable block in `index.html`
— swap in the real product's label numbers to make the nutrition view exact.

## How to read the charts

- **How it all moves together** — one shared time axis; read straight down a moment to
  see BG, GIR, and the feed at that time. **Good looks like:** sugars holding steady
  while the GIR step-line drops and the feed bars climb.
- **Total glucose delivered** — cumulative grams from the IV vs from feeds. Watch the
  formula band steepen as he takes over.
- **Formula nutrition** — each feed broken into carbohydrate / fat / protein.
- **Fluid budget** — daily IV + feed volume against the ~100 mL/kg/day cap.

## Logging new readings

Two ways, use whichever is easier in the moment:

1. **In the page (fastest at the bedside).** Fill the *Add a reading* form — date, time,
   blood sugar, formula mL, dextrose %, IV rate. It saves to that device instantly and
   redraws every chart. Your phone remembers entries between visits.
2. **In the file (permanent, kept in git).** Add one line to the `READINGS` list near the
   top of `index.html`:
   ```js
   { d:"2026-07-06", t:"05:30", dex:20, iv:12, bg:58, ml:25, fort:24, bm:10 },
   ```
   `bg:null` when a sugar wasn't measured; `fort` is fortification (kcal/oz) and `bm` is
   breast milk (mL). The **Export rows** button copies your device-entered readings in
   exactly this format to paste in.

## Sources

Provided by the family:
- Brigham & Women's Hospital / CWN **"WNH G.1" Neonatal Glucose** clinical pathway (GIR formula, weaning rule).
- Giouleka S. et al. *Diagnosis and Management of Neonatal Hypoglycemia: A Comprehensive Review of Guidelines.* **Children** 2023;10:1220.
- Rozance P.J., Hay W.W. *New approaches to management of neonatal hypoglycemia.* **Matern Health Neonatol Perinatol** 2016;2:3.
