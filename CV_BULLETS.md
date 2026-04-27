# Resume / CV Bullet Points — Market Basket Analysis Project

Three STAR-structured bullets, each tunable to space. Pick the one that fits the role you're
targeting; numbers below come from the actual notebook execution
(UK basket, 15,365 invoices × 3,821 SKUs, `min_support` ∈ [0.008, 0.030]).

---

## Bullet 1 — Algorithmic & engineering angle (best for quant / DS roles)

> **Engineered an end-to-end association-rule pipeline** on **396K cleaned e-commerce
> transactions** (UCI Online Retail, 12 months, UK retailer) to surface cross-sell
> opportunities. **Implemented and benchmarked Apriori vs. FP-Growth** in `mlxtend` across
> five support thresholds, **achieving up to a 3.80× FP-Growth speed-up** at
> `min_support = 0.01` (Apriori 4.26 s → FP-Growth 1.12 s on a 15K × 3.8K basket matrix);
> documented the regime where Apriori wins (small / sparse data) as the design-review
> rationale. **Mined 94 rules**, filtered to **36 high-impact rules** at
> `support ≥ 2 %`, `confidence ≥ 50 %`, `lift ≥ 3`, with top lift **22.5×** on the Regency
> teacup colourway family.

## Bullet 2 — Business-impact angle (best for strategy / consulting / BizDev roles)

> **Translated transactional data into a five-lever revenue plan** for an online retailer by
> mining association rules on a **541K-line, 12-month basket dataset**. **Identified
> 36 cross-sell rules with lift > 3 and confidence > 50 %** (top lift 22.5×, Regency
> teacup colourways), mapping each to a concrete action: PDP "frequently bought together"
> widget, colourway bundle pricing, planogram clustering, antecedent dynamic pricing, and
> recommender cold-start. **Quantified expected impact of +3-5 % units-per-order on the
> cross-sell widget alone** and packaged the read-out with A/B-test success criteria for
> each lever.

## Bullet 3 — Pipeline & reproducibility angle (best for MLE / production-DS roles)

> **Built a reproducible market-basket analysis pipeline in Python**
> (`pandas`, `mlxtend`, `seaborn`) covering ingestion, cleaning (cancellations, admin SKUs,
> returns), EDA, transaction encoding, frequent-itemset mining (Apriori + FP-Growth), rule
> extraction with Support / Confidence / Lift, and an executive-grade Markdown narrative.
> **Cut frequent-pattern mining time from 5.85 s (Apriori) to 1.70 s (FP-Growth)** on
> 1,838 itemsets at `min_support = 0.008` — **a 3.4× reduction** — and shipped the project
> as a portfolio-grade GitHub repo with structured README, requirements lock, and saved
> figures.

---

### Notes for tuning the bullets

* **Numbers above were captured on a laptop CPU.** Re-run the benchmark cell on the target
  hardware if you want exact reproducibility — the *shape* (FP-Growth ≈ 2-4× faster on the
  full basket, slower on the small Top-300 matrix) is hardware-stable.
* **Front-load the verb** ("Engineered", "Built", "Translated", "Cut") — STAR works only if
  the *Action* is unmistakable in the first three words.
* **One bullet per CV is usually enough** — pick the angle that matches the JD's language
  and cite the others in your cover letter or interview narrative.
* If the role explicitly values stochastic optimisation / Monte Carlo skills, append a
  one-liner: *"Identified follow-on extension to a Monte-Carlo-driven bundle-margin
  optimiser under inventory constraints — implementation in progress."*
