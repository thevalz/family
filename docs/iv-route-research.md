# Peripheral vs. central IV for D20 — research note

*A companion note to the Newborn Glucose Tracker. This is a personal analysis, **not
medical advice.** The NICU team's readings and orders are always the authority.*

---

## The question

He is on a **D20** (20% dextrose) drip. The tracker earlier prompted a fair question:
*is 20% dextrose supposed to go through a peripheral IV at all, or does it require a
central line?* None of the sources originally provided with the tracker addressed the
**route** — they all cover glucose thresholds, GIR weaning, and monitoring. This note
fills that gap.

**Short answer:**

| Claim | Verdict | Strength |
|---|---|---|
| The *general* rule caps peripheral dextrose at **12.5%** — above that, use a central line | **Well established** — FDA label, CPS, ESPGHAN/ESPEN/ESPR all agree | High |
| So D20 (20%) *by the general rule* would imply central access | True as a default | High |
| **But** for the specific case of neonatal hypoglycemia, **20% glucose can be run peripherally as safely as 15%** | **Supported by a randomized trial** | Moderate–high (single RCT, n = 121) |
| Therefore running his D20 in a peripheral line is a **defensible, evidence-backed choice**, not an error | Reasonable conclusion | Moderate |

The bottom line: the "12.5% needs a central line" rule is real and near-universal, **and**
there is direct trial evidence that the neonatal-hypoglycemia scenario is a recognized
exception. Both things are true at once.

---

## 1. The default rule: peripheral dextrose ≤ 12.5%

Multiple independent, authoritative sources converge on the same threshold:

- **FDA prescribing information** for concentrated dextrose injection states dextrose should
  be diluted for peripheral administration to a **maximum of 12.5%**; concentrations above
  12.5% call for a central line.[^fda]
- The **Canadian Paediatric Society** newborn-hypoglycemia position statement says the
  maximal peripheral concentration is **D12.5**, and that an infant needing dextrose
  **> 12.5%** should have a **central venous catheter** inserted.[^cps]
- The **ESPGHAN/ESPEN/ESPR** pediatric parenteral-nutrition guideline frames the same limit
  in terms of **osmolarity**: peripheral PN should stay **below ~900 mOsm/L**, and dextrose
  is the main driver of osmolarity — which is *why* the concentration ceiling exists.[^espghan]

**The rationale** is osmolarity, not the sugar itself. Hypertonic solutions (broadly
> 10%) irritate the thin wall of a peripheral vein and can cause **phlebitis, thrombosis,
and — if the cannula leaks — extravasation into the surrounding tissue**. A central line
empties into a high-flow central vein where the solution is diluted almost immediately, so
concentration matters far less there (central lines routinely run 25%, and up to 50% in
emergencies).[^fda]

By this rule alone, **D20 is above the peripheral ceiling** and would default to central
access. That is the part of the picture the original sources were silent on, and it is a
legitimate thing to have wondered about.

## 2. The exception: 20% glucose peripherally in neonatal hypoglycemia

The default PN rule is a general-purpose safety margin. The **specific** question — can you
run 20% glucose peripherally *in a newborn being treated for hypoglycemia* — has been
studied directly:

- **Vanhatalo & Tammela (2010),** a **randomized controlled trial** of **121 hypoglycemic
  newborns**, assigned infants to peripheral **20%** vs **15%** glucose (started at
  8 mg/kg/min and tapered to blood sugar). It found the two concentrations could be
  **infused equally safely into peripheral veins**, with **no significant difference in
  phlebitis scores or the number of cannula changes**.[^vanhatalo] The authors framed 20%
  as a practical way to deliver the same glucose in *less fluid* — relevant when the fluid
  budget is tight (exactly the ~100 mL/kg/day cap the tracker charts).

This is the single most on-point piece of evidence, and it is why review articles now note
that although 12.5% is the accepted peripheral maximum, **the integrity of peripheral veins
has been supported at concentrations up to 20%** on the strength of this trial.[^giouleka]

**How to weigh it honestly:** it is *one* RCT from a single center, roughly 120 infants,
scoring local irritation rather than long-term vessel outcomes. It does not overturn the
general 12.5% rule for parenteral nutrition. What it does do is provide real, randomized,
condition-specific evidence that **peripheral D20 for hypoglycemia is within accepted
practice** — which is the exact question that matters here.

## 3. What this means for him

- Running his **D20 peripherally is a defensible, evidence-backed choice** — not a mistake
  and not off-label improvisation. It has direct RCT support for precisely his situation.
- It is also **inherently higher-maintenance** than a central line. Peripheral cannulas in
  neonates are short-lived — reported **median dwell times of roughly 1–2 days** — and
  local complications (infiltration, phlebitis) are the most common reason they're
  replaced.[^complications] That is *expected*, not alarming: it means the site gets checked
  often and swapped when it tires, which is normal for a peripheral drip this concentrated.
- **What the bedside team watches for** at the IV site: swelling, blanching or redness,
  coolness, or leaking — signs the line is irritated or infiltrating. Concentrated dextrose
  that **extravasates** (leaks into tissue) can injure the surrounding skin, which is the
  concrete reason peripheral high-dextrose sites are monitored closely and changed at the
  first sign of trouble.[^complications]
- If a peripheral site does fail, standard practice is to **restart at a concentration the
  new peripheral line can tolerate (≤ 12.5%)** until access is sorted — or, if he genuinely
  needed a *sustained* concentration above the peripheral ceiling, that is the point at
  which a **central line** would be considered.[^cps] His GIR is being **weaned** (the drip
  is coming *down*, now at 8 mL/hr), so the trajectory is away from needing central access,
  not toward it.

## Verdict

The original worry was well-founded and the answer is reassuring: **the 12.5% peripheral
rule is real, and D20 exceeds it, but neonatal hypoglycemia is a recognized exception with
randomized-trial support for peripheral 20% glucose.** Running his D20 in a peripheral line
is consistent with the evidence. The tradeoff paid for avoiding a central line is more
frequent site checks and cannula changes — which is the normal cost of concentrated
peripheral dextrose, and a shrinking concern as the drip weans.

---

## Sources

Because a couple of primary PDFs (FDA, PubMed) were not directly retrievable in this
environment, the claims below were cross-checked across multiple corroborating references
(guideline bodies, drug references, and review articles) rather than read verbatim end to
end. Confidence is noted per item.

[^vanhatalo]: Vanhatalo T., Tammela O. *Glucose infusions into peripheral veins in the management of neonatal hypoglycaemia — 20% instead of 15%?* **Acta Paediatr** 2010;99(3):350–353. doi:[10.1111/j.1651-2227.2009.01237.x](https://doi.org/10.1111/j.1651-2227.2009.01237.x). PMID [19397539](https://pubmed.ncbi.nlm.nih.gov/19397539/). *RCT, 121 hypoglycemic newborns; peripheral 20% vs 15% glucose equally safe (no significant difference in phlebitis or cannula changes). The direct evidence for peripheral D20. Confidence: high on the finding; note single-center, n ≈ 121, local-irritation endpoints.*

[^fda]: U.S. FDA. *Dextrose Injection 20%, 30%, 40%, 50% and 70% — prescribing information* (Hospira). [accessdata.fda.gov](https://www.accessdata.fda.gov/drugsatfda_docs/label/2016/018561s057,018562s056,018563s057,018564s059,019345s044lbl.pdf). *Dilute for peripheral administration to a maximum of 12.5%; > 12.5% requires a central line; hypertonic solutions risk vein irritation/thrombosis. Corroborated by ASHP and CHEO drug references. Confidence: high.*

[^cps]: Narvey M.R., Marks S.D.; Canadian Paediatric Society, Fetus and Newborn Committee. *The screening and management of newborns at risk for low blood glucose.* Paediatr Child Health, reaffirmed. <https://cps.ca/en/documents/position/newborns-at-risk-for-low-blood-glucose>. *Symptomatic/unfeedable infants: IV 10% dextrose (or 2 mL/kg bolus over 15 min); initial infusion 80 mL/kg/day D10 ≈ 5.5 mg/kg/min; maximal peripheral concentration D12.5; > 12.5% → central venous catheter. Confidence: high (national guideline).*

[^espghan]: Mesotten D., Joosten K., van Kempen A., Verbruggen S.; ESPGHAN/ESPEN/ESPR/CSPEN. *Guidelines on pediatric parenteral nutrition: Carbohydrates.* **Clin Nutr** 2018;37(6 Pt B):2337–2343. PMID [30037708](https://pubmed.ncbi.nlm.nih.gov/30037708/). Companion venous-access guidance sets peripheral PN osmolarity **< ~900 mOsm/L**, of which dextrose is the main contributor. *Confidence: high on the osmolarity limit; medium on exact sub-paper attribution (the osmolarity figure sits in the guideline's venous-access section).*

[^giouleka]: Giouleka S., et al. *Diagnosis and Management of Neonatal Hypoglycemia: A Comprehensive Review of Guidelines.* **Children (Basel)** 2023;10(7):1220. doi:[10.3390/children10071220](https://doi.org/10.3390/children10071220). <https://pmc.ncbi.nlm.nih.gov/articles/PMC10378472/>. *Cross-guideline synthesis; notes the 12.5% peripheral norm and that peripheral-vein integrity has been supported up to 20% per the Vanhatalo RCT. Confidence: high (open access). Already in the tracker's source list.*

[^complications]: Representative neonatal peripheral-IV complication literature — e.g. multicenter observational cannulation-complication studies and neonatal extravasation reviews (infiltration/phlebitis are the leading causes of catheter loss; neonatal peripheral cannula median dwell ≈ 1–2 days; concentrated-dextrose extravasation can cause tissue injury, hence close site monitoring). Cited here as background on the *cost* of the peripheral route, not as concentration-specific guidance. Confidence: medium (general PIVC data, ranges vary by unit and population).
