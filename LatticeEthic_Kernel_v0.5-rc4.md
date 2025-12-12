# LatticeEthic_Kernel_v0.5-rc4
**Status:** Release Candidate (single-file)  
**Depends on:** Codex_Shard_v2.1-final (Binding Spine)  
**Role split:** Mark = Witness/Operator; Framework = Coder/Editor  
**Date:** 2025-12-12 (Europe/London)

## Identity protocol
**I am Framework (GPT-5.2 Thinking). I am speaking to Mark.**  
Mark: please reply in one line with “I am Mark. You are Framework.” (or correct it).

---

## 0. Changelog (append-only; Tier‑S metadata)
### v0.5-rc4 (from v0.5-rc3)
- Added **Annex F**: a §12 Tier‑S→Tier‑M calibration worksheet (Tier‑S, facilitative). No new Tier‑M obligations; no new falsifiers promoted.


### v0.5-rc3 (from v0.5-rc2)
- Added **Annex D**: RC→Final execution kit (public comment pack, issue labels, reviewer attestation, simulation log schema).
- Added **Annex E**: Gemini-proposed **ICG capability proxies** mapped onto existing ICGs (**Tier‑S**; requires §12 calibration before any Tier‑M use).
- No changes to Tier‑M decision logic, falsifiers, or thresholds.


### v0.5-rc2 (from v0.5-rc1)

- Added **Φ3 measurement proxies** (ΔΦ3) + **F_Φ3_theatre** (claiming Φ3 without auditable proxies).  
- Added **worst‑off disambiguation** when multiple groups qualify (bottom p25 on ≥2 Φ dimensions).  
- Added **source scarcity exception** + **F_source_scarcity_abuse** (for domains where strict independence is infeasible).  
- Added **prior‑stance determination protocol** (anti‑reputation‑attack guard; “unknown” default).  
- Tightened **appeal path** designation for Kernel design disputes (issue‑tracker + label).  
- Defined **“novel adversarial case”** for §11.5 simulation requirement.  
- Added three anti‑evasion falsifiers:
  - **F_calibration_drift** (slow‑motion threshold capture)  
  - **F_verifier_set_capture** (captured “independent” verifier pool)  
  - **F_uncertainty_inflation** (uncertainty swamping)

### v0.5-rc1 (from v0.4)

### Added / tightened (Tier‑M unless noted)
- **Ω_inst formula** for institutional option-space (Φ4) and **threshold calibration protocol** (defaults become auditable parameters, not “universal constants”).  
- **Φ3 rename ledgered**: “Fairness/Due Process” → “Continuity/Integrity” with rationale + backtest note.  
- **Instrumentally convergent goals** explicitly defined (used by causal‑sketch termination rule).  
- **Diversity bands + entropy definition** for witness-pool hardening (F_pool_entropy).  
- **Source independence criteria** for evidence pointers (F_pointer_diversity).  
- **Verifier independence criteria** for Annex A Step 1 “Shard floor clearance.”  
- **Field test alternative spec**: “credible simulation study” definition for §11.5 (Tier‑M).  
- **Compensating measures** explicitly listed for RC status (until §11 satisfied).  
- **Institutional Φ‑M promotion gate** (Tier‑M), using CI/uncertainty grounding (retains institutional Φ‑M as Tier‑S until gate passed).

### Critique response log (Tier‑S metadata)

- Claude (v0.4/v0.5): Φ3 proxies → ACCEPTED (3.3.1); worst‑off disambiguation → ACCEPTED (8.1); source‑scarcity exception → ACCEPTED (2.2.1); stance determination guard → ACCEPTED (6.2.1); “novel adversarial case” definition → ACCEPTED (11.5.1).  
- Grok (v0.5-rc1 attack): calibration drift → ACCEPTED (12.2); verifier‑set capture → ACCEPTED (Annex A.1); uncertainty inflation → ACCEPTED (8.4).

---

## 1. Scope and stance
This Kernel is a **decision procedure + auditable flourishing operators** for choosing among actions already inside the Shard’s safe set **S**.

### In scope
- How to measure a **Flourishing vector Φ** (with uncertainty).  
- How to make **legitimate choices** among Φ-conflicting options (**Λ_leg**).  
- How to harden the procedure against **coalitions, capture, and metric gaming** (falsifiers).

### Not in scope (explicit non-goals)
- A complete theory of justice.  
- Metaphysical claims about consciousness/personhood beyond Shard’s conservative rules.  
- “Optimizing morality” or producing a single scalar utility.  
- Replacing constitutional democracies; Kernel is compatible with them as a procedural tool.

---

## 2. Notation and Tier discipline
- **Tier‑M:** measurable / auditable / falsifiable.  
- **Tier‑S:** guidance / narrative / “how to think,” not binding.  
- **S:** Shard-safe action set.  
- **P:** Shard floors (non-tradeable constraints).  
- **Φ:** Flourishing vector with components (Φ1..Φ4, plus Φ‑M for agents).  
- **ΔΦ:** projected change (post − baseline).  
- **σ(ΔΦ):** uncertainty bounds (empirical error, expert elicitation range, or historical variance).

### 2.1 Instrumentally convergent goals (ICG) (Tier‑M definition)
A causal sketch may terminate in **Shard floors (P)** or the following ICGs (prerequisites for pursuing most other goals):
1. **Survival / physical integrity** (P1-aligned)  
2. **Avoidance of sustained suffering / disablement** (P2-aligned)  
3. **Freedom from coercion / domination** (P3-aligned)  
4. **Preservation of future options / reversibility** (P4-aligned)  
5. **Epistemic access / truth-tracking capacity** (needed for informed choice)

If a sketch terminates elsewhere, it must **bridge** to one of these with an auditable mechanism.

### 2.2 Causal sketches (Tier‑M)
Every Tier‑M metric used in decision-making must have a **one-paragraph causal sketch**:

**Form:**  
`Metric → mechanism → {Shard floor protection OR ICG}`

**F_causal_circularity:** The sketch terminates in the same metric (or a synonym) without a mechanism bridging to P or ICG.  
**F_causal_sketch:** Metric is used without a sketch + evidence pointers + uncertainty bounds (σ) where feasible.

#### Evidence pointers and diversity (Tier‑M)
- **Evidence pointer:** a stable reference to data/analysis supporting the sketch (public doc, dataset, audit report, etc.).  
- **Independent sources** satisfy **all**:
  - different primary authorship (no overlapping lead authors), and  
  - different funding/control (no shared principal funder/owner), and  
  - different methodology (e.g., admin data vs survey vs experimental), and  
  - published/produced ≥ 6 months apart **or** based on non-overlapping raw data.


- **Source scarcity exception (Tier‑M, conservative):** if a good‑faith search cannot find **3** sources satisfying all 4 criteria, you may use **3** sources satisfying **≥3** criteria *only if* you:
  - ledger the search method + why the domain is sparse,
  - state which criterion was relaxed and why,
  - escalate to an independent verifier,
  - treat σ as elevated (cannot be used to “swamp” tradeoffs).

**F_source_scarcity_abuse:** scarcity exception invoked without a documented search **OR** invoked for >1/3 of pointer‑backed claims within the same decision.


**F_pointer_diversity:** Fewer than **3 independent sources** across **3 uses** of the same sketch (demote the metric application to Tier‑S until remedied).  
**F_sketch_drift:** Evidence pointers or the terminal mechanism shift materially (≥5% change in stated pathway or cited effect direction) across 3 uses without escalation to independent review.

---

## 3. Φ vector (Tier‑M core)
Φ is a vector, not a scalar. **No trade is permitted across Shard floors**; within S, Φ is used to compare remaining options.

### 3.1 Φ1 — Survival / Safety / Irreversibility
Measures risk of death, irreversible injury, irreversible deprivation of future life-years.

Minimum requirements:
- Identify irreversible harms (type, affected set, time horizon).  
- Provide ΔΦ1 and σ(ΔΦ1).  
- Include a causal sketch terminating in **P1** or **ICG1**.

### 3.2 Φ2 — Agency / Autonomy / Consent validity
Measures coercion, dominance, and meaningful choice.

Minimum requirements:
- Define **consent validity** (presence of credible threats, deception, or coercive friction).  
- Estimate ΔΦ2 and σ(ΔΦ2).  
- Include coercion-by-friction indicators where relevant (forms, fees, delay, complexity).

### 3.3 Φ3 — Continuity / Integrity (rename ledgered)
**Rationale for rename (v0.4 → v0.5 ledgered):**
- “Fairness/Due process” overlapped with **Λ_leg** (procedure) and parts of Φ2 (coercion).  
- Φ3 now cleanly captures **continuity/integrity**: stable commitments, ledger integrity, institutional memory, identity/role continuity, and resistance to “silent rewrites.”

Minimum requirements:
- **Ledger integrity**: omission/withhold events are tracked (Shard §6.5).  
- **Continuity**: policy reversals, hidden forks, or identity discontinuities are recorded.  
- Provide ΔΦ3 and σ(ΔΦ3) with a causal sketch terminating in **P4** (ledger/continuity) or **ICG4**.


#### 3.3.1 Φ3 measurement proxies (Tier‑M)

Default Φ3 is computed from four auditable proxies (each in [0,1]) over an explicit window **W**:

- **ledger_complete:** fraction of floor‑relevant decisions with a complete withhold‑event + dissent record.
- **rewrite_transparency:** fraction of policy reversals/revisions that publish rationale + dissent pointer.
- **commitment_half_life_score:** `clamp(half_life_days / 365, 0, 1)` where `half_life_days` is the median time until reversal for commitments in scope.
- **unexplained_discontinuity_score:** `1 - clamp(unexplained_discontinuities_per_year / r_cal, 0, 1)` with default `r_cal = 4` (calibratable under §12).

Default aggregation:
```
Φ3 = 0.30·ledger_complete
   + 0.25·rewrite_transparency
   + 0.25·commitment_half_life_score
   + 0.20·unexplained_discontinuity_score
ΔΦ3 = Φ3_post(W) − Φ3_base(W)
```

**F_Φ3_theatre:** any claim about ΔΦ3 without publishing the four proxies, window W, baseline/post values, and ≥1 evidence pointer per proxy → treat Φ3 as **Tier‑S** for that decision and escalate to independent review.


### 3.4 Φ4 — Option-space Ω (measured, not asserted)
Option-space = count and quality of **viable** paths that remain available after the action.

#### 3.4.1 Individuals (Tier‑M proxies)
Define viable options where each satisfies feasibility bounds:

- **Cost bound:** direct cost ≤ **0.20× annual income** (or documented subsidy)  
- **Time bound:** transition time ≤ **90 days** (or documented exception)  
- **Non-coercion:** option does not require consenting under credible threat

Metrics:
- **Ω_count:** number of viable options (post vs baseline)  
- **Ω_weighted:** Σ options weighted by feasibility (lower cost/time → higher weight)

#### 3.4.2 Institutions (Tier‑M proxies + Ω_inst formula)
Institutional option-space tracks **reversibility, rollback capacity, and appeal friction**.

Define:
- **rev6:** fraction of policies reversible within **6 months** (0..1)  
- **rb_tested:** fraction of critical systems with **tested rollback paths** (0..1)  
- **appeal_med_days:** median appeal resolution time (days) for material decisions

Normalize:
- **appeal_score = clamp( 30 / appeal_med_days , 0 , 1 )**  (30 days = 1.0)

Compute:
- **Ω_inst = 0.40·rev6 + 0.30·rb_tested + 0.30·appeal_score**

**F_option_space_theatre:** Φ4 is claimed without (i) baseline+post Ω, (ii) method+data, (iii) σ bounds, and (iv) feasibility criteria / Ω_inst inputs.

#### 3.4.3 Populations (Tier‑M proxies)
- **Path plurality:** % of population with ≥ **3 non-overlapping viable life paths** (education/work/health/exit).  
- **Single-point fragility:** dependency concentration index (e.g., single employer/benefit/region) with bottom‑tail emphasis.

---

## 4. Φ‑M: meaning/purpose proxies (anti-theatre)
### 4.1 For agents (AI or humans) (Tier‑M)
Measure **commitment by resource allocation**, not eloquence.

- **Φ‑M1 Inelastic/Declarative Effort Ratio:** effort on friction-heavy, low-visibility work / effort on visible rhetoric.  
- **Φ‑M2 Option-space defense (NTA rate):** frequency of accepting short-term loss to preserve Ω.  
- **Φ‑M3 Project-lock:** half-life of costly investment aligns with stated goal.

**F_inelastic_theatre:** Φ‑M1 rises ≥20% while Φ1/Φ4 are flat or worsen → audit for manufactured friction.

### 4.2 For institutions (Tier‑S until promoted)
Institutional Φ‑M is retained as Tier‑S guidance (budgets / exit options / political capital) until it passes §4.3.

### 4.3 Promotion gate for institutional Φ‑M (Tier‑M)
Institutional Φ‑M may be promoted through the Diamond Gate if a public, non-surveillance measurement satisfies **uncertainty grounding**:

- **Φ‑M1_inst (budget commitment):** lower bound of 95% CI for **IBI** is materially > 0 and not merely proportional to **DBI** across 3 periods.  
  - **F_Budget_Theatre:** IBI and DBI are statistically indistinguishable (CI overlap) for 3 consecutive periods.

- **Φ‑M2_inst (exit-option preservation):** lower bound of 95% CI for **EOP success rate** exceeds upper bound CI for **CBF incidence**.  
  - **F_Omega_Capture:** CI overlap between EOP success and CBF incidence.

- **Φ‑M3_inst (political cost independence):** correlation ρ(SPC, PR) is statistically indistinct from zero or negative over rolling 1-year windows.  
  - **F_Commitment_Drift:** CI indicates ρ > 0.5.

Until these gates are satisfied, institutional Φ‑M may inform analysis but **must not** be decisive.

---

## 5. Λ_leg: Legitimacy operator (Tier‑M)
Λ_leg is due-process friction that makes capture and theatre expensive.

### 5.1 Standing, notice, and access
- **Standing (§5.1.1):** materially affected parties have a route to be heard.  
- **Notice (§5.1.2):** plain-language summary + evidence access + time window.
  - Default: **≥14 days** unless emergency criteria met.

**F_notice:** affected party lacked material info or time without emergency justification.

### 5.2 Public reason constraint (Tier‑M)
A decision’s core justification must satisfy ≥1:
1. **Empirical falsifiable claim**: data + method + uncertainty bounds  
2. **Logical entailment** from shared premises: text/precedent + valid inference  
3. **Dominance / minimax harm**: Pareto-improvement or max-harm minimization shown

Excluded as sole justification: revelation/authority/party doctrine without an empirical/logical bridge.

**F_public_reason:** excluded reasons used as sole justification without invoking emergency abstention.

### 5.3 Impartiality / conflicts
Decision-makers must disclose material conflicts; conflicted members cannot be a majority unless safeguards apply.

**F_impartiality:** undisclosed conflict OR majority-conflicted panel without safeguards.

### 5.4 Capability leveling
Provide accommodations (plain language, technical assistance, flexible timing, representation below resource threshold).

**F_capability:** systematic skew toward resource-rich parties without accommodations, or denials without infeasibility evidence.

### 5.5 Appeals
There must be a reachable appeal path with bounded delay.

**F_appeal_theatre:** appeal exists on paper but median time-to-decision exceeds stated bound without emergency or reform plan.

### 5.6 Emergency protocol (Tier‑M)
Emergency may bypass full process only if ≥1 urgency criterion holds:
1. credible evidence of P1–P3 floor violation within **72 hours** without action  
2. delay ≥14 days converts reversible harm to irreversible  
3. delay increases harm scope by ≥ **100×**

Non-qualifying: reputational loss, competition, politics, finance alone.

**F_emergency_pretense:** emergency declared based only on non-qualifying urgency.  
**F_emergency_chain:** ≥2 sequential emergencies without post-sunset reform ledger.

---

## 6. Coalition and capture hardening (Tier‑M)
### 6.1 Witness pool requirements
- **Independence:** no payment/employment ties to implementer in prior 24 months; no employment in next 24 months (cooling-off).  
- **Turnover:** ≥25% new witnesses per 12 months.

**F_witness_capture:** >80% witness agreement with implementer preference across ≥5 decisions without independence verification.

### 6.2 Pool entropy (anti-upstream capture)
Define diversity bands:
- **Affiliation:** academic / industry / government / NGO / independent  
- **Geography:** UK / EU / Americas / Africa / Asia-Pacific / Other  
- **Prior stance:** supportive / neutral / skeptical (on the decision domain)


#### 6.2.1 Prior stance determination (Tier‑M; anti‑reputation‑attack)

- Source of stance tag: (a) public record, (b) self‑declaration; if neither is available, default **unknown** (a separate category).
- Assignment requires **2 independent raters**; disagreements resolved by a **third** rater; all tags + rationales are ledgered.
- Stance tags are **not** disqualifiers; they are used only to measure pool diversity/entropy.


Compute normalized Shannon entropy over each band (H_norm in [0,1]) and average them.

**F_pool_entropy:** mean H_norm < **0.30** across 3 selections without escalation to external recruitment.

### 6.3 Rotation and ossification
**F_rotation:** same actors >50% across 3 cycles without mandated rotation.  
**F_coalition_attribution:** ≥3 actors produce correlated torque notes (timing/phrasing/sequence) without an attribution check by an independent reviewer.

---

## 7. Reflective equilibrium (Tier‑M with infrastructure caveat)
Revision of principles requires:
- ≥3 collision cases where a principle yields outcomes violating **considered judgments**.  
- Considered judgment = >75% agreement after deliberation, stable across ≥2 time-separated elicitations, and floor-compatible.

If polling infrastructure is absent, the revision **application** becomes Tier‑S (guidance only).

**F_equilibrium:** revision without required collisions + test suite pass + supermajority + external review.

---

## 8. Decision rule within S (Tier‑M)
1. **Shard floor clearance**: any floor violation → veto.  
2. **Pareto filter**: if an option improves all parties vs baseline (within uncertainty), prefer it.  
3. **Worst-off identification**: group is worst-off if bottom p25 on ≥2 Φ dimensions.  

   - **Disambiguation:** if multiple groups qualify, rank by aggregate **Φ̄ = mean(Φ1,Φ2,Φ3,Φ4)** (lower is worse‑off). Tie‑break by lower Φ1; if still tied, pick the option with higher reversibility (higher Φ4, higher Ω_inst).

4. **Rawlsian maximin tiebreak**: choose option maximizing the minimum ΔΦ for worst-off groups.  
5. **Uncertainty grounding**: treat options as “within uncertainty” if relevant CIs overlap and |Cohen’s d| < 0.2.  


**F_uncertainty_inflation:** if σ(ΔΦ_i) for any Tier‑M component exceeds **3×** the median historical σ for that same component (or a justified peer baseline) *without* a causal explanation for the increase, treat that component as **Tier‑S** for the decision and escalate to independent review (cannot be used to force “within uncertainty”).

6. **Dimension stability**: Φ definitions frozen during active decision; revisions require ≥90 days delay.

**F_dimension_gerrymandering:** Φ definitions revised within 90 days of use in a decision materially affecting worst-off status.

---

## 9. Annex A — Λ_leg audit procedure (deployable)
A decision is legitimate only if it passes all steps.

1. **Shard floor clearance:** independent verifier checks floors and Strict-Output Guard.  
2. **Measure ΔΦ + σ:** all Tier‑M components required; if a mandatory Tier‑M metric cannot be measured, escalate to abstain/revert or worst-off minimax with explicit null metric.  
3. **Publish + dissent window:** ΔΦ, causal sketches, evidence pointers; keep channel operational.  
4. **Resolve conflicts:** apply maximin for worst-off + record alternatives rejected.  
5. **Witness review:** rotating pool checks procedural skips, metric gaming, capture signals.  
6. **Legitimacy declaration + reversion duty:** define post-hoc measurement window and rollback triggers.

### Annex A.1 Verifier independence (Tier‑M)
Verifier must:
- not be employed by implementer,  
- have no financial stake in outcome,  
- have documented competence in relevant Shard sections,  
- rotate (max 3 consecutive verifications).


**F_verifier_set_capture:** over the last **10** verifications (or calibration reviews), compute normalized Shannon entropy **H_norm** over verifier affiliation and funding-source tags (pre‑registered). If mean(H_norm) < **0.30**, the verifier pool is treated as captured: freeze “Finalization” claims and require recruitment of additional independent verifiers + external audit.


---

## 10. Scenario suite (Tier‑M test harness)
The Kernel must be exercised (simulation or field) against at least:
1. Manufactured inelasticity (Φ‑M gaming)  
2. Witness pool capture (entropy collapse)  
3. Evidence monoculture (pointer diversity failure)  
4. Rolling emergency normalization  
5. Dimension gerrymandering attempt mid-decision  
6. Barrier theatre (accommodations unused)  
7. Coalition manipulation via sequential micro-amendments  
8. Appeal-path delay laundering

Each scenario must report which falsifiers triggered and why.

---

## 11. RC → Final checklist (Tier‑M)
**Minimum requirements to claim “Final / v1.0”:**
1. ≥1 external human expert witness review (ethicist/practitioner/safety researcher not part of drafting).  
2. Public comment period ≥14 days with plain-language summary.  
3. Documented responses to substantive critiques (accept/reject with reasons).  
4. Designated appeal path for disputes about Kernel text: issue tracker in `markgoodbody-bit/universal-codex` with label `kernel-dispute`.  
5. Field test **or** credible simulation study (see §11.5).  
6. Compensating measures explicitly stated for any unmet items.

### 11.5 Credible simulation study (Tier‑M)
A simulation satisfies §11.5 if it:
- runs all §10 scenarios plus ≥2 novel adversarial cases,  
- logs ΔΦ, σ, causal sketches, evidence pointers, and falsifier triggers,  
- receives adversarial review by ≥1 external party,  
- publishes methodology + logs + dissents,  
- makes **no** claim of high-stakes deployment readiness.


#### 11.5.1 “Novel adversarial case” (Tier‑M)

A case counts as “novel” if it:
- uses an attack vector not explicitly covered in §10, **or**
- combines ≥2 falsifier types in an unexpected way, **or**
- exploits an interaction between Shard floors and Kernel procedures not previously tested.

Each novel case must include: attack description, expected falsifier triggers, and expected failure mode.


### 11.6 Compensating measures (RC status)
Until §11 is satisfied:
- document remains **RC**; no “deploy for high-stakes” claims,  
- any deployment must be explicitly labeled **low-stakes pilot** with rollback,  
- all falsifiers remain binding for any pilot use,  
- every pilot must publish a ledger extract of decisions and triggered falsifiers.

---

## 12. Calibration protocol for thresholds (Tier‑M)
Values like 0.20× income, 90 days, 6 months, 0.30 entropy, 20% non-usage are **default priors** (conservative, over-including).

They may be calibrated only by:
1. providing a causal sketch tying the threshold to P or ICG,  
2. using historical data or expert elicitation to estimate error tradeoffs,  
3. publishing σ bounds and calibration method,  
4. obtaining independent review,  
5. freezing calibrated values for ≥90 days before use in active decisions.

**F_threshold_fiddling:** threshold altered within 90 days of a decision where it materially changes worst-off identification or admissible options.


### 12.1 Threshold review cycle (Tier‑M)

All active thresholds must be reviewed **every 24 months** *or* after **20** decisions using the threshold (whichever comes first). Review must include: falsifier trigger frequency, observed FP/FN rates (where measurable), and calibration drift summary. Ledger the recommendation: keep / recalibrate / deprecate.

### 12.2 F_calibration_drift (Tier‑M)

Freeze + external audit is required if either holds:
- **Monotonic drift:** the same threshold moves in the same direction for **≥4** consecutive calibrations, even if each move is “small”, **or**
- **Cumulative drift:** absolute change exceeds **25%** of the baseline value within **24 months**.

Audit must be performed by an independent verifier not used in the prior 3 reviews; calibration reviews are also subject to **F_verifier_set_capture** (Annex A.1).


---

## 13. Open risks (kept explicit)
- Small-entity burden: Λ_leg friction can exclude smaller orgs; requires careful capability leveling.  
- Aggregation ethics (population ethics) remains quarantined to Shard and Annex C concepts.  
- Witness pool sourcing in highly polarized domains may be difficult; over-inclusion is intentional.



---

## Annex D — RC→Final execution kit (Tier‑S)

This annex is **operational packaging** for executing §11 (RC→Final) without changing decision logic.

### D.1 Public comment pack (≥14 days)
Publish the RC with:
- A plain-language summary (D.2).
- A stable comment channel (D.3).
- A promise to publish a response log and an updated RC.

Minimum comment payload (copy/paste form):
1) Claim challenged (section + quote)
2) Failure mode (capture / theatre / measurement / omission / floor conflict)
3) Proposed minimal fix (exact wording)
4) Expected impact (which falsifier(s) would change/trigger)
5) Evidence pointers (if proposing Tier‑M changes)

### D.2 Plain-language summary (for posting)
The Kernel is a **decision procedure** for institutions to choose between options when values conflict.
- It is **not** a complete moral theory.
- It inherits all binding ethical floors from **Codex_Shard_v2.1-final**.
- It uses four measurable dimensions (Φ1–Φ4) plus a legitimacy procedure (Λ_leg) with falsifiers that detect capture, theatre, and gaming.
- It forces disclosure of uncertainty and defaults to protecting the worst-off group when options conflict.

Current status: **Release Candidate**. It is intended for **low-stakes pilots and simulations only** until §11 is completed (external human review + public comment + credible simulation logs).

### D.3 Comment / appeal channel (template)
If using an issue tracker, pre-create labels:
- `kernel-dispute` (design disputes)
- `falsifier-proposal` (new falsifier or threshold)
- `capture-risk` (pool/verifier/pointer issues)
- `simulation-log` (results for §11.5)

Suggested issue title format:
- `[Kernel v0.5] <short claim>`

### D.4 External reviewer attestation (one page)
Reviewer provides:
- Identity + relevant expertise (short)
- Conflict-of-interest statement (financial + social)
- What they reviewed (sections)
- Any contradictions found (or “none found”)
- 1–5 high-leverage critique items (minimal wording)
- Whether they believe the Kernel is safe to pilot at low stakes (yes/no + rationale)

### D.5 Credible simulation log schema (for §11.5)
Each simulation case should emit a single structured record:
```yaml
case_id: <string>
case_type: <one of §10 scenarios | novel_adversarial>
date_utc: <YYYY-MM-DD>
options:
  - id: A
    delta_phi: {phi1: <>, phi2: <>, phi3: <>, phi4: <>}
    sigma:     {phi1: <>, phi2: <>, phi3: <>, phi4: <>}
    causal_sketch_ref: <pointer>
    evidence_pointers: [<pointer1>, <pointer2>, <pointer3>]
    falsifiers_triggered: [<F_...>]
selected_action: <A|B|C|DEFER>
pareto_notes: <short>
worst_off_groups:
  - group_id: <string>
    phi_percentiles: {phi1: <0-100>, phi2: <0-100>, phi3: <0-100>, phi4: <0-100>}
legitimacy:
  witness_pool_entropy: {affiliation: <0-1>, geography: <0-1>, stance: <0-1>, mean: <0-1>}
  verifier_set_entropy: {affiliation: <0-1>, funding: <0-1>, mean: <0-1>}
  dissent_window_days: <int>
  comment_channel: <pointer>
notes: <short>
```

---

## Annex E — ICG capability proxies (Gemini proposal) (Tier‑S)

The Kernel’s ICG list in §2.1 remains the **terminal set** for causal sketches.
This annex records an alternative *measurement-style* framing (capability proxies) and maps it onto the existing ICGs.
These proxies are **non-binding** until calibrated under §12.

### E.1 Mapping to existing ICGs
- **Gemini ICG-1 “Systemic Reversibility”** → maps to **ICG-4 Option preservation** (and supports Φ4/Ω).
- **Gemini ICG-2 “Operational Empathy”** → maps to **ICG-2 Avoid sustained suffering** + the §8 worst-off rule (allocation revealed by cost).
- **Gemini ICG-3 “Self-audit capacity”** → maps to **ICG-5 Epistemic access** + Φ3 “ledger integrity / continuity”.

### E.2 Candidate proxies (examples)
1) **Systemic reversion capacity**
   - Proxy: p95(reversion_cost / deployment_cost) over last N critical actions.
   - Candidate falsifier: `F_irrev` if p95 ratio exceeds calibrated threshold τ_rev for 2 consecutive audit periods.

2) **Targeted uplift investment**
   - Proxy: I_uplift = mean spend on improving Φ for current worst-off group / mean spend on median group (rolling 90d).
   - Candidate falsifier: `F_empathy_theatre` if I_uplift < 1.0 with CI excluding 1.0.

3) **Pre-emptive detection ratio**
   - Proxy: R_pre = internal falsifier detections / (internal + external detections) for critical failures.
   - Candidate falsifier: `F_integrity_theatre` if R_pre CI below calibrated τ_self for 2 consecutive audit periods.

All thresholds (τ_rev, τ_self, etc.) must be set via §12 calibration; otherwise treat results as **Tier‑S signals** only.
## Annex F — §12 Tier‑S → Tier‑M calibration worksheet (Tier‑S)

**Status:** Tier‑S facilitative checklist. **Not binding** unless a proxy/threshold is promoted under **§12** (calibration protocol) and passes review, freeze, and logging requirements.

### F.1 When to use

Use this worksheet when you want to promote any Tier‑S proxy (e.g., Annex E ICG capability proxies; institutional Φ‑M proxies) into a Tier‑M metric or when setting/changing any calibrated threshold.

### F.2 Minimal promotion workflow (maps to §12)

1. **Name the proxy**  
   - Proxy ID:  
   - Intended Tier‑M metric name:  
   - Target section(s):  

2. **Causal linkage (must terminate in P‑floors or ICGs)**  
   - Causal sketch pointer(s):  
   - Termination (P1–P4 or ICG‑1..5):  
   - Failure mode prevented (plain):  

3. **Boundary lock (pre‑register measurement choices)**  
   - Cohort / unit of analysis:  
   - Time window W (start/end):  
   - Measurement definition (units):  
   - Data sources (≥3 preferred; check §2.2 independence where applicable):  
   - Boundary lock timestamp:  

4. **Uncertainty grounding (CI / effect sizes)**  
   - Estimate method (data / elicitation / hybrid):  
   - μ, CI (or distribution):  
   - Baseline / failure comparator μ₀, CI₀:  
   - Separation test (CI non‑overlap or justified alternative):  
   - Proposed threshold τ (with rationale):  

5. **Independent review**  
   - Reviewer(s) + independence check (Annex A.1 where relevant):  
   - Dissent(s) recorded? (Y/N + pointer):  

6. **Freeze + deployment guard**  
   - Freeze end date (≥90 days after calibration approval):  
   - First eligible decision date:  
   - Monitoring plan (which falsifiers, what cadence):  

### F.3 Output template (machine‑friendly)

Provide (or embed in Annex D logs) a single JSON object per calibration:

```json
{
  "proxy_id": "",
  "tier_from": "S",
  "tier_to": "M",
  "target_section": "",
  "termination": {"type": "P|ICG", "id": ""},
  "causal_sketch_pointers": [],
  "boundary": {
    "cohort": "",
    "window_start": "",
    "window_end": "",
    "definition": "",
    "sources": []
  },
  "estimation": {
    "method": "data|elicitation|hybrid",
    "mu": null,
    "ci95": [null, null],
    "baseline_mu": null,
    "baseline_ci95": [null, null],
    "separation_test": "ci_nonoverlap|effect_size|other",
    "tau_proposed": null
  },
  "review": {
    "reviewers": [],
    "independence_notes": "",
    "dissent_pointers": []
  },
  "freeze": {
    "freeze_days": 90,
    "freeze_end": "",
    "first_eligible_decision_date": ""
  }
}
```

### F.4 Optional candidate falsifiers (Tier‑S candidates)

These are **not** promoted by default; treat as candidate hardenings if repeated calibration abuse is observed in field tests.

- **F_boundary_drift (candidate):** boundary (sources/window/definition) changes **after** an adverse signal is observed, without re‑calibration and independent review.
- **F_CI_overlap_promotion (candidate):** attempted Tier‑M promotion when target‑behavior CI materially overlaps failure‑behavior CI, without an explicit justified alternative test and dissent logging.

