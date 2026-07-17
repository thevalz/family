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
  to see the range. (That the immature brain has genuine **windows of vulnerability** is not in
  dispute — it's well described for hypoxic-ischemic and excitotoxic injury (Johnston 1995,
  among the papers you shared)[^johnston]; being preterm is exactly why his exposure is worth
  quantifying carefully rather than dismissing. What that literature does *not* establish is an
  aluminum-specific injury mechanism at these doses.)

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

### How much injected aluminum is "too much"? Two frameworks

Under the hood of the whole vaccine-aluminum debate is a single unsettled question: **what
number should a vaccine dose be compared against?** There are two camps, and the papers you've
gathered are mostly the second one. It's worth seeing both clearly.

**Framework A — modeled body burden (mainstream / regulatory).** Aluminum injected into muscle
is released *slowly* and cleared continuously, so the right thing to track is the **whole-body
burden over time**, not the size of a single dose. FDA's pharmacokinetic model (Mitkus 2011)
does exactly that and finds the burden across the entire schedule stays **below** the safety
level derived from the ATSDR minimal-risk level.[^mitkus] A 2018 *Vaccine* review by **Principi
& Esposito** — mainstream pediatric-infectious-disease authors — reaches the same bottom line:
**"no apparent reason exists to support the elimination of Al from vaccines for fear of
neurotoxicity"** (they flag only the separate, adult, macrophagic-myofasciitis / chronic-fatigue
question as unsettled).[^principi] On this view, comparing a per-dose µg/kg to a *daily* limit is
simply the wrong comparison.

**Framework B — weight-scaled dose limit (the minority / "Pediatric Dose Limit" school).** A
group centered on IPAK (Lyons-Weiler) and the Exley/CHD circle argues the opposite: take a
**safe level and scale it to a baby's body weight**, and the schedule looks alarming.
- **Lyons-Weiler & Ricketson (2018)** derive a weight-corrected **"Pediatric Dose Limit"** and
  show that an 850 µg vaccine dose is ~**150 µg/kg at 2 months** — far above the FDA 4–5 µg/kg/day
  IV figure and above their own derived pediatric limit (~10 µg/kg at birth rising to ~37 µg/kg
  at 2 years).[^lwr] The tool's schedule section can now overlay this line so you can see it.
- **McFarland, Thomas & Lyons-Weiler (2020)** run a retention model over three schedules —
  standard CDC, a low-/no-aluminum CDC, and **Dr. Paul Thomas's "Vaccine Friendly Plan," which is
  essentially the spaced plan you're considering** — and report a **"% of days over limit":**
  roughly **24% of days (birth–2 yr) for CDC vs. ~2–5% for the spaced plan.**[^mcfarland] Taken at
  face value, that is the strongest quantitative argument *for* spacing.

**Why they reach opposite conclusions.** Two real methodological forks:
1. **Which safe level?** Framework B scales a limit that was itself derived from **oral/dietary**
   aluminum in **adult animals** (the ATSDR/JECFA MRL) and applies it to **injected** aluminum.
   Oral and injected aluminum differ ~1000-fold in absorption, so mainstream toxicology considers
   this cross-route scaling invalid — it's the same category error as reading a vaccine's µg/kg
   against the IV drip limit.
2. **Dose vs. burden.** Framework B compares each **dose** to a **daily** limit (a bolus-vs-rate
   mismatch); Framework A models the **slow-release burden** the body actually carries.

**Provenance matters here, and cuts both ways.** Framework B's papers cluster in a few journals
and authors (IPAK; the Exley group; and, in McFarland 2020, **Paul Thomas himself — the author of
the very "Vaccine Friendly Plan" being evaluated**, whose Oregon medical license was suspended in
2020 over his vaccine practices); McFarland 2020 also carries a **published 2021 correction.**
That doesn't make their concern illegitimate — under-study of injected-aluminum kinetics in
infants is a fair point — but it does mean these are advocacy-adjacent analyses built on a
contested limit, not independent confirmation.

**The tie-breaker is outcomes, not models.** You don't have to adjudicate the dose math to get an
answer, because the hypothesis has been tested at the level that matters — **actual children,
actual diagnoses.** The Danish cohort of **1.2 million** (Andersson 2025) linked each child's
cumulative vaccine aluminum to 50 chronic conditions and found **no increased risk**, including
neurodevelopmental (§5).[^andersson] Framework B's own community published a **critique** of that
study — Crépeaux et al. 2026, *"a call for science,"* co-authored by Shaw, Tomljenovic, Exley,
Shoenfeld, Lyons-Weiler and Children's Health Defense figures — raising objections about exposure
classification, confounding, and conflicts of interest.[^callforscience] Some of those points are
worth engaging; none, in the mainstream reading, overturns a null result across a million
children. **So: if the spacing question is about aluminum specifically, Framework B says spacing
helps against a limit most toxicologists reject, and the best outcome data finds nothing to
prevent in the first place.** Which is why this stays a values-and-logistics conversation for you
and your pediatrician — the disease-timing trade-off is the concrete part.

## 7. The aluminum–autism question — reading the literature you shared

You've gathered a real cross-section of the aluminum-and-autism literature, and it deserves a
straight, rigorous read rather than a wave-off. The single most useful lens is the **hierarchy
of evidence** — not all studies answer the causal question equally well:

> **Strongest → weakest for "does X cause Y":** randomized trials → large **individual-level**
> cohort studies (each child's own exposure linked to their own outcome) → **ecological**
> correlations (population averages, no individual data) → uncontrolled tissue/case series →
> mechanistic and animal plausibility.

The papers you shared sit mostly in the **lower** tiers; the study that sits highest — the
Danish cohort (§5) — points the other way. Here is each, on its merits.

- **Tomljenovic & Shaw (2011), "Do aluminum vaccine adjuvants contribute to the rising
  prevalence of autism?"** (*J. Inorg. Biochem.*).[^tomshaw] This is the most-cited paper for the
  vaccine-aluminum→autism claim. What it did: took **population-level** autism-prevalence numbers
  (US Dept. of Education, 1991–2008) and correlated them with the cumulative aluminum in the CDC
  vaccine schedule, plus cross-country comparisons, reporting a strong correlation (r ≈ 0.92) and
  applying "Hill's criteria" to argue causation. Why it can't carry that weight: it is an
  **ecological correlation** — it never links any individual child's aluminum to that child's
  outcome, so it is wide open to the **ecological fallacy.** Over 1991–2008 essentially everything
  that rose with time correlates with autism *diagnoses* at r ≈ 0.9 (household internet, organic
  food sales, bottled water) — the classic illustration of why time-trend correlation isn't cause.
  And autism **diagnosis** rose largely because the diagnostic criteria broadened (DSM-III-R →
  DSM-IV) and ascertainment improved, not necessarily because the underlying condition became more
  common. The authors are also not neutral: Shaw and Tomljenovic's aluminum-adjuvant program has
  been funded by foundations that campaign against vaccines, and **several of their subsequent
  aluminum-adjuvant animal papers were retracted or corrected** over data-integrity concerns. Most
  decisively, the hypothesis this paper raises was **testable at the individual level and has since
  been tested** — the Danish cohort of 1.2 million children (§5) found **no association**.
  Individual-level data beats an ecological correlation every time.
- **Sealey, Bagasra et al. (2016), "Environmental factors in the development of autism spectrum
  disorders"** (*Environ. Int.*).[^sealey] A **review** that catalogs many candidate environmental
  contributors to ASD — pesticides, phthalates, PCBs, solvents, air pollutants, fragrances,
  glyphosate, heavy metals — with aluminum-in-vaccines as **one item on a long, speculative list.**
  As a narrative review it *surveys hypotheses*; it does not test them or establish causation for
  any of them, aluminum included. Useful as a map of what's been proposed; not evidence that any
  particular factor (or aluminum) is causal.
- **Mold, Umar, King & Exley (2018), "Aluminium in brain tissue in autism"** (*J. Trace Elem.
  Med. Biol.*).[^mold] *(You uploaded this one twice — it's a single paper.)* It measured aluminum
  in brain tissue from **5 deceased donors** with autism (imaging in 10) and reported high values.
  Its limitations are serious and widely noted: **n = 5**, **no matched control group** in the
  quantitative arm (so "high compared to whom?" is unanswered), brain-aluminum measurement is
  contamination-prone, and — fundamentally — **finding a substance in tissue cannot show it caused
  the condition**, nor does it establish where the aluminum came from (diet, air, and vaccines all
  contribute over a lifetime). A hypothesis-generating case series; the major review bodies (AAP,
  CDC) do not treat it as evidence of causation.[^aap]
- **Johnston (1995), "Neurotransmitters and vulnerability of the developing brain"** (*Brain &
  Dev.*).[^johnston] This one is different in kind — a **legitimate, mainstream** developmental-
  neuroscience review, and it isn't about aluminum. Its point is that the immature brain passes
  through **windows of selective vulnerability** (the germinal matrix to hemorrhage in the
  preterm infant, developing white matter to injury, NMDA/glutamate receptors to excitotoxicity
  during hypoxia-ischemia). It's a sound argument for taking the *developing/preterm brain*
  seriously — which is exactly why this note flags his **36-week status** rather than waving it
  away (see §4). But it speaks to *susceptibility in general* (chiefly hypoxic-ischemic and
  excitotoxic injury); it offers **no aluminum-specific mechanism** and shouldn't be read as one.
- **AAP 2026 Immunization Schedule** — used above as the source for the standard schedule.
- **Delgado-León et al. (2018), apoptosis in pancreatic β-cells from arsenic + atorvastatin in
  diabetic rats** — reviewed, but it concerns **arsenic and a cholesterol drug in a diabetes
  model**, not aluminum and not neurodevelopment. It doesn't bear on this question.

**The honest synthesis.** The case *for* a vaccine-aluminum→autism link rests on ecological
correlations (Tomljenovic & Shaw; the vaccine strand of Sealey/Bagasra), an uncontrolled tissue
series (Mold/Exley), and mechanistic/animal plausibility. The case is weakened by the fact that
when the hypothesis was finally tested with **individual-level** data on **1.2 million children**,
the association **wasn't there** (§5). That doesn't make aluminum harmless in every context — the
FDA's parenteral warning is real, and the preterm brain is genuinely a vulnerable system (Johnston)
— but it does mean the specific claim that aluminum-adjuvanted vaccines cause autism is **not
supported by the best available evidence.** Read the papers; weigh them by what kind of question
each can actually answer.

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

[^callforscience]: Crépeaux G., Hammond J.R., Handley J.B., Hooker B., Jablonowski K., Luján L.,
Lyons-Weiler J., Nosten-Bertrand M., Shaw C.A., Shoenfeld Y., Tomljenovic L., Exley C.
*Aluminium adjuvants and childhood health: a call for science.* **J. Trace Elem. Med. Biol.**
2026;93:127810 (the paper you shared). A **critique of the Andersson 2025 Danish cohort**,
objecting on aluminum toxicology, cohort design/statistics, and conflicts of interest.
*Positioning:* a position paper by the aluminum-skeptic author network (incl. Children's Health
Defense affiliates). Some methodological points merit engagement; does not, in the mainstream
reading, overturn a null result across 1.2M children. *(Confidence: high on what it argues; low
that it refutes the cohort.)*

[^lwr]: Lyons-Weiler J., Ricketson R. *Reconsideration of the immunotherapeutic pediatric safe
dose levels of aluminum.* **J. Trace Elem. Med. Biol.** 2018;48:67–73 (the paper you shared).
Derives a weight-corrected **Pediatric Dose Limit** and argues the schedule's per-dose µg/kg
(e.g., ~150 µg/kg @2mo) exceeds it. *Positioning:* the limit is scaled from **oral/dietary**
adult-animal MRLs and applied to **injected** aluminum — a cross-route extrapolation mainstream
toxicology rejects; not adopted by regulators; IPAK-authored. *(Confidence: high on what it
claims; the injected-from-oral scaling is its central contested step.)*

[^mcfarland]: McFarland G., La Joie E., Thomas P., Lyons-Weiler J. *Acute exposure and chronic
retention of aluminum in three vaccine schedules and effects of genetic and environmental
variation.* **J. Trace Elem. Med. Biol.** 2020;58:126444 (the paper you shared; **corrected
2021, vol. 65**). Models CDC vs. low-/no-Al CDC vs. Paul Thomas's **"Vaccine Friendly Plan"**
(≈ your spaced plan) with a Priest-based retention model and a **"% days over limit"** metric
(~24% CDC vs. ~2–5% spaced, birth–2yr). *Positioning:* co-authored by the VFP's creator
(Paul Thomas, license suspended 2020) + IPAK; builds on the contested PDL and a modified Priest
model with retention-amplifying assumptions. *(Confidence: high on what it reports; its "over
limit" claim inherits the PDL's contested basis.)*

[^principi]: Principi N., Esposito S. *Aluminum in vaccines: Does it create a safety problem?*
**Vaccine** 2018;36(39):5825–31 (the paper you shared). Mainstream pediatric-ID review:
**"no apparent reason exists to support the elimination of Al from vaccines for fear of
neurotoxicity"**; flags only the Al-oxyhydroxide → macrophagic-myofasciitis / ME-CFS question
as unsettled. *(Confidence: high; establishment counter-review to Framework B.)*

[^aap]: Committee on Infectious Diseases, American Academy of Pediatrics. *The Role and Safety of
Aluminum Adjuvants in Childhood Vaccines.* **Pediatrics** 2025;157(3):e2025074874. Reviews the
evidence and affirms the safety of aluminum adjuvants; notes alternative/spaced schedules lack
demonstrated benefit and prolong susceptibility. *(Confidence: high; professional-society
consensus.)*

[^mold]: Mold M., Umar D., King A., Exley C. *Aluminium in brain tissue in autism.* **J. Trace
Elem. Med. Biol.** 2018;46:76–82 (the paper you shared, twice). Case series, n = 5 (imaging in
10), no matched controls in the quantitative arm; hypothesis-generating, cannot establish
causation, and the producing lab has drawn substantial methodological criticism. *(Confidence:
high on the description of its limits.)*

[^tomshaw]: Tomljenovic L., Shaw C.A. *Do aluminum vaccine adjuvants contribute to the rising
prevalence of autism?* **J. Inorg. Biochem.** 2011;105(11):1489–99 (the paper you shared).
**Ecological correlation** of population ASD prevalence vs. schedule aluminum (US 1991–2008,
r ≈ 0.92; cross-country), interpreted via Hill's criteria. *Positioning:* population-level
correlation cannot establish individual causation (ecological fallacy); confounded by
diagnostic-criteria broadening and secular trends; authors have anti-vaccine-foundation funding,
and later aluminum-adjuvant animal papers from this group were retracted/corrected. Contradicted
by individual-level cohort data (Andersson 2025). *(Confidence: high that its design cannot
support a causal claim.)*

[^sealey]: Sealey L.A., Hughes B.W., … Bagasra O. *Environmental factors in the development of
autism spectrum disorders.* **Environ. Int.** 2016;88:288–98 (the paper you shared). Narrative
**review** cataloging many hypothesized environmental ASD contributors (pesticides, phthalates,
PCBs, solvents, air pollutants, fragrances, glyphosate, heavy metals incl. aluminum adjuvants).
*Positioning:* surveys hypotheses; does not test causation for aluminum or any single factor.
*(Confidence: high that it is hypothesis-level, not causal evidence.)*

[^johnston]: Johnston M.V. *Neurotransmitters and vulnerability of the developing brain.* **Brain
Dev.** 1995;17(5):301–6 (the paper you shared). Mainstream review of developmental
selective-vulnerability windows (germinal-matrix hemorrhage, periventricular leukomalacia,
NMDA/glutamate excitotoxicity in hypoxia-ischemia). *Positioning:* supports taking the
preterm/immature brain seriously in general; **not** about aluminum and offers no
aluminum-specific mechanism. *(Confidence: high; a well-regarded neuroscience review.)*
