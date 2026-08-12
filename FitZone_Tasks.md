# FitZone Gym — Task Notes

## The Project

FitZone is a single gym in Gurugram: 1,200 members joined over 18 months (Jan 2025 – Jun 2026) on three plans — Monthly (₹1,500/mo), Quarterly (₹1,200/mo), Annual (₹1,000/mo). The owner, Kavita, says:

> "People join with full josh and vanish in two months. I spend on Instagram ads, they come, they go. Who stays? Who leaves? And can I predict who is about to quit — early enough to save them?"

**Goal:** find who leaves, why — and build an early-warning signal.

Reference list for `FitZone.ipynb`. Each task below matches a section in the notebook.

**T1 — Clean.** Fix duplicate check-ins, mixed-format `join_date`/`cancel_date`, and impossible cancel-before-join rows. Handle at the field level, don't drop whole members.

**T2 — Overall churn.** Compute the headline churn rate. On its own it's nearly meaningless — the value is in the splits that follow.

**T3 — Churn by plan.** Compare churn across Monthly / Quarterly / Annual plans.

**T4 — Churn by signup source.** Compare churn across Instagram / Google / Walk-in / Referral.

**T5 — The January effect.** Do members who join in January churn more than everyone else?

**T6 — The habit finding.** Count each member's visits in their first 30 days, bucket them, and compare churn. Include zero-visit members (fillna(0)) — don't let them silently vanish.

**T7 — The memo to Kavita.** Turn the findings into numbered, actionable recommendations, each backed by its number.
