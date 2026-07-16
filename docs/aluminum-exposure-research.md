# Aluminum exposure from the D20 IV — research note

*A companion note to the Newborn Glucose Tracker and the interactive
[**aluminum exposure tool**](aluminum.html). This is a personal analysis, **not medical
advice.** Your NICU team, pediatrician, and pharmacist have his real records and are the
authority. The goal here is to answer, as honestly and quantitatively as possible, a fair
question: **how much aluminum went into him intravenously, how does his body handle it, and
how does that compare to the toxic threshold — and to vaccines?***

---

## The questions

1. **How much aluminum was put into him through the IV?**
2. **The FDA's 4–5 mcg/kg/day limit — is that an oral number or an intravenous one?**
3. **How does the amount administered compare to the rate his body can expel it, and to the
   toxic level?**
4. **How does the IV aluminum compare to what vaccines would add — and can we evaluate a
   specific spaced-out schedule?**

**Short answers:**

| Question | Answer | Confidence |
|---|---|---|
| Total IV aluminum from the D20 | **~25 mcg (0.025 mg)** over the whole course, at the label's *worst-case* concentration; likely less | High (given the data + labeled ceiling) |
| Is the 4–5 mcg/kg/day limit oral or IV? | **Intravenous (parenteral).** The label says so explicitly | Very high (verbatim in the label) |
| Peak daily rate vs. the toxic threshold | **~1.65 mcg/kg/day at the busiest day — below the 4–5 mcg/kg/day line**, even at the labeled max | High for dextrose alone; see additive caveat |
| Does his body clear it? | Yes — the majority is excreted renally; a fraction is retained. He is late-preterm, so clearance is less complete than term but far better than a very-preterm infant | Moderate (population estimates, not his labs) |
| IV vs. vaccine aluminum | The first-6-month vaccine schedule is **~4.4 mg intramuscular** — ~175× the *mass* of his IV course, but a different route with a long safety record | High on the mass; see kinetic nuance |

---

## 1. How much went in — the arithmetic

The tracker logs the IV rate (mL/hr) at each check. Holding each rate until the next reading
(the same integration the glucose tracker uses for cumulative dextrose) gives the total
volume of D20 infused:

- **Total D20 infused ≈ 992 mL** (forward-fill) to **~1,110 mL** (trapezoidal), over the
  active drip window of ~4.3 days (Jul 3 06:00 → Jul 7 14:30, then off).

The FDA label states Dextrose Injection **"contains no more than 25 mcg/L of aluminum"**
(§5.6 and §11).[^fda] That is a **labeled maximum at expiry** — a regulatory ceiling, not a
measurement of the specific lots he received, which are typically lower. Using the ceiling as
a worst case:

| Aluminum in the D20 | Total aluminum | Cumulative per kg | Average daily | Peak day (Jul 4) |
|---|---|---|---|---|
| **25 mcg/L** (labeled max) | **~25 mcg (0.025 mg)** | ~5.4 mcg/kg | ~1.2–1.4 mcg/kg/day | **~1.65 mcg/kg/day** |
| 15 mcg/L (mid estimate) | ~15 mcg | ~3.2 mcg/kg | ~0.7–0.8 mcg/kg/day | ~1.0 |
| 5 mcg/L (low estimate) | ~5 mcg | ~1.1 mcg/kg | ~0.25 mcg/kg/day | ~0.3 |

Per-day rate at the labeled max: Jul 3 ≈ 1.45, **Jul 4 ≈ 1.65**, Jul 5 ≈ 1.37, Jul 6 ≈ 0.78,
Jul 7 ≈ 0.15 mcg/kg/day. **Even at the labeled maximum, his highest single day sits below the
FDA's 4–5 mcg/kg/day threshold**, and the true concentration is almost certainly lower than
25 mcg/L.

> **The one big caveat on "how much."** This counts the **dextrose only**. In *full*
> parenteral nutrition, the dextrose is usually a **minor** aluminum source; the large
> contributors are the additives — **calcium gluconate, cysteine, sodium/potassium phosphate**
> — historically the dominant aluminum in neonatal PN.[^oliveira] If he received any of those,
> they are **not** in this calculation. The single most useful thing you can do is ask the NICU
> pharmacist whether he got anything IV besides dextrose, and if so, the aluminum content.

## 2. Oral or IV? The threshold is **intravenous**

This is the crux of your question, and the label is unambiguous. FDA §5.6, *Aluminum
Toxicity*:

> *"Patients with renal impairment, including preterm infants, who receive **parenteral**
> levels of aluminum at greater than 4 to 5 mcg/kg/day, accumulate aluminum at levels
> associated with central nervous system and bone toxicity."*[^fda]

"Parenteral" means into the bloodstream — IV (or the aluminum in IV nutrition). It is **not**
an oral limit, and the distinction is enormous, because **how much aluminum actually reaches
the blood depends almost entirely on the route:**

| Route | Fraction that reaches the bloodstream | Why |
|---|---|---|
| **Oral** (feeds, formula, breast milk, water, food) | **~0.1–0.3%** | The gut is a barrier; nearly all ingested aluminum passes straight through and is excreted in stool[^atsdr] |
| **Intravenous** (his D20 drip) | **~100%** | Injected directly into blood — the gut barrier is bypassed entirely[^atsdr][^toxrev] |
| **Intramuscular** (vaccines) | High over time, but **released slowly** from the muscle over weeks[^mitkus] | A depot in the muscle dissolves gradually while the kidneys clear it |

This is why an IV product warns about single-digit mcg/kg/day while the same amount eaten
would be trivial: an oral aluminum limit is roughly **1,000× higher** than the parenteral one
because so little is absorbed.[^atsdr] It is also why the FDA regulates aluminum in *IV*
products specifically.

## 3. The route he actually got — central line

He received the D20 through a **central venous catheter (central line)**, not a peripheral
IV. That is the *standard* route for D20: at 20%, dextrose is too concentrated (and too
hypertonic, >900 mOsm/L) for a peripheral vein, so the label requires central access above
~12.5%.[^fda] (An earlier note in this project explored whether D20 *could* run peripherally;
that scenario did not apply to him.)

For the aluminum question, **central vs. peripheral makes no difference**: both are
intravenous, both deliver ~100% of the aluminum to the blood, and both are cleared the same
way. What matters is that it was **intravenous rather than oral** — which is exactly the route
the FDA threshold is about.

## 4. Administered vs. expelled vs. toxic

Aluminum that reaches the blood is handled two ways: **excreted by the kidneys** (the
majority, in urine) and **retained** in tissue — mostly bone, with a small amount elsewhere —
where it has a **very long half-life (years)**.[^toxrev][^atsdr] The balance between intake
and clearance is the whole story, and it is exactly why the FDA limit is a **daily rate**, not
a lifetime total: toxicity is about **administering faster than the body can clear**.

- In **healthy adults**, roughly **40%** of parenteral aluminum is retained short-term and the
  rest is excreted, most within days.[^toxrev]
- In **preterm infants**, retention is higher — studies of parenterally-fed preterm infants
  report **>75%** retained, because immature kidneys excrete aluminum incompletely and it
  deposits in bone.[^fewtrell] This is the vulnerability the FDA warning names.
- He is **late preterm (36 weeks)** with a **high birth weight**. That places him in the
  flagged "preterm" category — his kidneys are less mature than a term baby's — **but** far
  from the extremely-preterm, very-low-birth-weight infants (often <32 weeks, ~1 kg) who
  dominate the toxicity literature. His renal clearance is much closer to a term infant's than
  to a 28-weeker's. The honest read is *"a real reason for care, not a reason for alarm"* — and
  the tool lets you move the retention assumption between term (~40%) and very-preterm (~75%)
  to see the range.

**Putting the three together for his case:** the daily *administration* rate peaked at
~1.65 mcg/kg/day (labeled max) — below the 4–5 mcg/kg/day line — for a **short ~4.3-day
course**, after which intake stopped and his kidneys have been clearing the load since. The
retained fraction is small in absolute terms (a few mcg to ~15 mcg depending on the scenario).
Contrast that with the classic toxicity setting: *weeks* of parenteral nutrition in a *very*
preterm infant at higher daily rates. He differs on all three axes — rate, duration, and degree
of prematurity.

### Calibrating context, stated fairly

Of the three drivers behind the FDA's aluminum warning:

- **Prematurity** — *partially present.* He is late preterm (36 wk), at the mild end.
- **Prolonged administration** — *absent.* ~4.3 days, versus the weeks of PN in the toxicity
  studies.
- **Renal impairment** — *no known impairment.*

None of this is a clinical clearance — only his team can give that — but it is the accurate
frame for reading the number.

## 5. IV aluminum vs. vaccines

Your underlying decision is about vaccination, so here is the honest comparison.

**By mass and route:**

| Source | Amount | Route | How much reaches blood |
|---|---|---|---|
| His entire D20 IV course | ~0.025 mg (25 mcg) | Intravenous | ~100%, over ~4 days |
| Diet, first 6 months (formula) | ~19 mg ingested | Oral | only ~0.04 mg absorbed (~0.2%)[^chop] |
| Vaccine schedule, first 6 months | up to ~4.4 mg | Intramuscular | high, but released over **weeks**[^chop][^mitkus] |

So by **raw mass**, the vaccine schedule is far larger than his IV course (~175×) — and even
the *absorbed* dietary aluminum over six months rivals the whole IV course. Mass alone is
misleading; **route and rate are what matter.**

**Why you cannot read a vaccine's mcg/kg against the 4–5 IV line.** This is the single most
important — and most misused — point. The 4–5 mcg/kg/day limit was derived for **intravenous**
products delivering aluminum straight to the blood, daily, in infants who can't clear it.
Vaccine aluminum is **intramuscular**: it forms a depot that dissolves slowly, so the *peak
amount in the blood on any day* is a small fraction of the injected dose, and the kidneys are
clearing it the whole time. FDA's own pharmacokinetic modeling (**Mitkus et al., 2011**) found
that the **body burden** of aluminum from the entire vaccine schedule stays **well below** the
regulatory safe body burden — precisely because of this slow-release, continuously-cleared
kinetics.[^mitkus] Taking the injected mcg/kg and comparing it to the IV per-day limit (the
basis of the widely circulated *"vaccines exceed the safe limit 50×"* claim) compares two
things that are not the same kind of exposure.

**What the outcome evidence says.** The question that actually matters isn't the microgram
count — it's whether children who get aluminum-adjuvanted vaccines have worse
neurodevelopmental outcomes. The largest study to date, a **nationwide Danish cohort of ~1.2
million children (Andersson et al., *Annals of Internal Medicine*, 2025)**, linked each child's
*cumulative* vaccine aluminum in the first two years to later diagnoses across 50 chronic
conditions — autoimmune, allergic, and **neurodevelopmental** — and found **no increased risk**;
for neurodevelopmental disorders the hazard ratio was slightly **below** 1 (0.93, 95% CI
0.90–0.97).[^andersson] This is consistent with the **American Academy of Pediatrics'** 2025
review of aluminum adjuvant safety.[^aap] (The Danish study has been criticized by
aluminum-skeptic researchers[^callforscience]; the criticisms are mostly about design choices
and do not, in the mainstream reading, overturn a null result of that size. You should weigh it,
but it remains by far the strongest evidence available.)

## 6. Evaluating your proposed spaced schedule

You asked to check a specific **spaced-out plan** against the standard schedule. The interactive
tool does this live; the numbers below use typical package-insert aluminum values and a median
weight-for-age. **Aluminum content is brand-dependent** — the biggest lever is the **Hib brand**.

**Your spaced plan** (roughly one aluminum-containing vaccine per visit, live vaccines given
alone, HepB deferred):

| Visit | Vaccines | Aluminum |
|---|---|---|
| 2 mo | Hib + DTaP | ~555 mcg (225 + 330) |
| 3 mo | Prevnar (PCV) | ~125 mcg |
| 4 mo | Hib + DTaP | ~555 mcg |
| 5 mo | Prevnar | ~125 mcg |
| 6 mo | Hib + DTaP | ~555 mcg |
| 7–9 mo | Prevnar | ~125 mcg |
| 1 yr | Hib + Prevnar | ~350 mcg |
| 18 mo | DTaP | ~330 mcg |
| 3 yr | MMR (alone) | 0 (live vaccine) |
| 4–6 yr | DTaP | ~330 mcg |

- **Peak single visit ≈ 555 mcg** (vs. ~930 mcg at the standard 2-month visit).
- **Total over this window ≈ 3.0 mg** (vs. ~4.0 mg standard) — similar totals, spread thinner.

**Two honest observations:**

1. **The Hib brand is the real lever.** **PedvaxHIB** (PRP-OMP) carries ~225 mcg of aluminum;
   **ActHIB / Hiberix** (PRP-T) carry **none**. Choosing a PRP-T Hib removes Hib's aluminum from
   *every* Hib visit — a larger effect than the spacing itself. This is worth discussing with the
   pediatrician regardless of schedule.
2. **What spacing does and doesn't buy.** Spacing lowers the *per-visit* aluminum but not
   dramatically the *total*, and — per the kinetics above — the per-visit peak was never the
   thing crossing a real toxic line to begin with. The mainstream view is that alternative
   spaced schedules have **no demonstrated neurodevelopmental benefit** and **lengthen the window
   in which he is unprotected** against the target diseases (pertussis, Hib, pneumococcus — all
   most dangerous in the youngest infants).[^aap] That is the genuine trade-off to weigh with your
   pediatrician: a modest reduction in per-visit aluminum (of uncertain benefit) against extra
   months of susceptibility (of well-established risk). The schedule is yours to choose; this note
   is only meant to make the aluminum side of the ledger accurate.

## 7. The papers you shared

You attached several sources; here is a straight read of each.

- **Mold, Umar, King & Exley (2018), "Aluminium in brain tissue in autism"** (*J. Trace Elem.
  Med. Biol.*).[^mold] This is the paper most often cited for an aluminum–autism link. What it
  actually did: measured aluminum in brain tissue from **5 deceased donors** with autism (plus
  fluorescence imaging in 10), and reported high values. Its real limitations are serious and
  widely noted: **n = 5**, **no matched control group** in the quantitative measurements (so
  "high compared to what?" is unanswered), aluminum measurement in brain tissue is prone to
  contamination, and — most fundamentally — **finding a substance in tissue cannot show it caused
  the condition.** The paper's own introduction leans on a correlation between rising vaccine use
  and rising autism diagnoses, which is an ecological correlation, not evidence of causation
  (autism *diagnosis* has risen for many well-documented reasons). The lab that produced it has
  been repeatedly criticized on methodology. It is a hypothesis-generating case series, and the
  major review bodies (AAP, CDC) do not treat it as evidence that aluminum causes autism.[^aap]
  It deserves to be read — and read critically.
- **AAP 2026 Immunization Schedule** — used above as the source for the standard schedule.
- **Delgado-León et al. (2018), apoptosis in pancreatic β-cells from arsenic + atorvastatin in
  diabetic rats** — reviewed, but it concerns **arsenic and a cholesterol drug in a diabetes
  model**, not aluminum and not neurodevelopment. It doesn't bear on this question.

## 8. What to ask your care team

- **NICU pharmacist:** Did he receive anything IV besides the D20 dextrose (amino acids, lipids,
  calcium, phosphate, IV meds)? If so, what was the aluminum content? *(This is the biggest
  unknown in the "total aluminum" figure.)*
- **Pediatrician:** Given he was late-preterm on a short dextrose course with no known kidney
  problem, is there any reason to check a **serum aluminum** level? *(For most such babies the
  answer is no — but it's the one test that measures him directly rather than by model.)*
- **Pediatrician, on vaccines:** Can we use **PRP-T Hib (ActHIB/Hiberix)** to cut aluminum with
  no downside? And what are the concrete disease risks of the spacing I'm considering?

---

## Sources

*Where a primary PDF wasn't fully machine-readable in this environment, figures were
cross-checked against authoritative secondary sources; confidence is noted per item.*

[^fda]: U.S. FDA / Hospira. *Dextrose Injection 20%, 30%, 40%, 50% and 70% — Prescribing
Information* (Rev. 2/2016). §5.6 Aluminum Toxicity: "contains no more than 25 mcg/L of
aluminum"; parenteral aluminum >4–5 mcg/kg/day in renal-impaired patients and preterm infants
accumulates to CNS/bone-toxic levels. §2.1/5.5: >12.5% dextrose / ≥900 mOsm/L requires central
access. *(The label you attached; read verbatim. Confidence: very high.)*

[^atsdr]: Agency for Toxic Substances and Disease Registry (ATSDR). *Toxicological Profile for
Aluminum*, Ch. 2–3 (toxicokinetics). Oral bioavailability ~0.1–0.3%; the majority of *absorbed*
aluminum is excreted in urine; oral vs. injected absorption differs ~1,000×. *(Confidence: high;
the 0.1% figure underlies ATSDR's route adjustment.)*

[^toxrev]: Willhite C.C. et al., and related aluminum toxicokinetics reviews (e.g., human ²⁶Al
tracer studies, Priest). Intravenous aluminum is ~100% bioavailable; ~40% short-term retention
in healthy adults; retained fraction has a multi-year half-life (bone). *(Confidence:
moderate–high; retention/half-life vary by study and renal status.)*

[^fewtrell]: Fewtrell M.S. et al. *Aluminium exposure from parenteral nutrition in preterm
infants and later health outcomes.* Proc. Nutr. Soc. 2011;70:299–304 (and the underlying
Bishop N.J. et al., *Aluminum neurotoxicity in preterm infants receiving intravenous-feeding
solutions,* **N. Engl. J. Med.** 1997;336:1557–61). Parenterally-fed preterm infants retain
>75% of infused aluminum; the RCT found lower Bayley motor scores in preterm infants on
standard (aluminum-containing) vs. aluminum-depleted IV feeding. *(Confidence: high; note the
population is preterm infants on prolonged PN — more exposed than this baby.)*

[^oliveira]: Oliveira S.R. et al. *Aluminum content in intravenous solutions for administration
to neonates.* JPEN 2010; and related neonatal-PN aluminum literature. In neonatal PN, calcium
and phosphate additives (and cysteine) are the dominant aluminum contributors; dextrose is
comparatively minor. *(Confidence: high on the qualitative ranking.)*

[^chop]: Children's Hospital of Philadelphia, Vaccine Education Center — *Aluminum in Vaccines.*
Cumulative vaccine aluminum up to ~4.4 mg in the first 6 months (~3.7 mg over the first year on
the 2025 schedule); dietary aluminum over the same period far exceeds it (breast milk ~5 mg,
milk formula ~19 mg, soy formula ~117 mg, ingested); IM route, slow elimination. *(Confidence:
high; a pediatric authority summarizing package-insert and dietary data.)*

[^mitkus]: Mitkus R.J., King D.B., Hess M.A., Forshee R.A., Walderhaug M.O. *Updated aluminum
pharmacokinetics following infant exposures through diet and vaccination.* **Vaccine**
2011;29:9538–43. PK modeling shows the body burden of aluminum from the vaccine schedule stays
below the ATSDR minimal-risk body burden across infancy. *(Confidence: high; the standard
reference for vaccine-aluminum kinetics.)*

[^andersson]: Andersson N.W. et al. *Aluminum-Adsorbed Vaccines and Chronic Diseases in
Childhood: A Nationwide Cohort Study.* **Ann. Intern. Med.** 2025;178(10) (ANNALS-25-00997);
PMID 40658954. ~1.2 million Danish children; cumulative vaccine aluminum in the first 2 years vs.
50 chronic disorders; no increased risk, neurodevelopmental HR 0.93 (0.90–0.97). *(Confidence:
high; largest cohort to date. Debated by aluminum-skeptic authors — see next.)*

[^callforscience]: Critique of the Danish cohort (aluminum-skeptic commentary, *J. Trace Elem.
Med. Biol.* 2025, "Aluminium adjuvants and childhood health: a call for science"). Raises
design/analysis objections. *(Included for balance; does not, in the mainstream reading,
overturn the cohort's null result.)*

[^aap]: Committee on Infectious Diseases, American Academy of Pediatrics. *The Role and Safety of
Aluminum Adjuvants in Childhood Vaccines.* **Pediatrics** 2025;157(3):e2025074874. Reviews the
evidence and affirms the safety of aluminum adjuvants; notes alternative/spaced schedules lack
demonstrated benefit and prolong susceptibility. *(Confidence: high; professional-society
consensus.)*

[^mold]: Mold M., Umar D., King A., Exley C. *Aluminium in brain tissue in autism.* **J. Trace
Elem. Med. Biol.** 2018;46:76–82 (the paper you shared). Case series, n = 5 (imaging in 10), no
matched controls in the quantitative arm; hypothesis-generating, cannot establish causation, and
the producing lab has drawn substantial methodological criticism. *(Confidence: high on the
description of its limits.)*
