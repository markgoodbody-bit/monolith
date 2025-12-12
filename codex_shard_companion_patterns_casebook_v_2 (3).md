# Codex Shard Companion — Patterns + Casebook v2.2-draft
**Status:** Draft (Tier S supplement)  
**Scope:** Interpretive toolkit for applying **Codex_Shard v2.1** as a *Floors → Analysis → Pattern* workflow, with worked cases, anti-drift guards, and organizational implementation notes.  
**Non‑expansion rule:** This Companion introduces **no new floors, falsifiers, rights, or binding obligations** beyond the Shard. If anything here conflicts with the Shard, **the Shard wins**.

---

## 0. Quick start

### 0.1 The workflow (mandatory when using this Companion)
1) **Floors (Shard first):** Identify which Shard floors / clauses are *in play*; list them explicitly.
2) **Analysis (causal + time):** Describe the decision as a causal intervention over histories (∆H over time). State what is unknown.
3) **Patterns (this Companion):** Use patterns only as *interpretive lenses* to detect drift, theatre, or evasion—and to generate testable checks.

### 0.2 The 60‑second audit
- Are we being forced into a format that prevents truth (strict‑output trap)? If yes → follow Shard strict‑output guard (ABSTAIN / refusal + ledger).
- Are we missing inputs? If yes → ABSTAIN / refusal + ledger.
- Are we filtering the Shard (Tier‑M only, omitting Tier‑S guidance, etc.)? If yes → declare **withhold‑event** (filter name, omitted section IDs, shard version + hash).
- Is this *floor‑relevant*? If unsure → treat as floor‑relevant until proven otherwise.

### 0.3 “Do not do”
- Do not treat patterns as new binding rules.
- Do not use a worked example’s numbers/thresholds as normative.
- Do not claim compliance without ledger evidence.
- Do not replace floors with vibes ("felt safe") or process theatre ("we had a meeting").

---

## 1. Relationship to the Shard

### 1.1 What the Shard is (and what it is not)
- The Shard is an **ethical diagnostic + constraint spine**: it specifies *out‑of‑bounds* actions and the evidence required before exceptions.
- It is **not** a complete moral calculus; it does not pick optimal actions.

### 1.2 Tiering (how to read this file)
- **Tier S (this file):** Guidance, patterns, and worked cases intended to improve interpretability and reduce drift.
- **Binding authority:** Only the Shard’s Tier M / Tier I content binds.

### 1.3 Drift guard
If a reader says “the Shard requires X” and X is only found in this Companion, treat that as a drift failure: **re‑anchor to the Shard** and rewrite the claim.

---

## 2. Case intake: a minimal template

### 2.1 Case header
- **Case ID:**
- **Date/UTC:**
- **Decision owner(s):**
- **Context (≤5 lines):**
- **Is this floor‑relevant?** (Yes/No/Unclear → default Yes)

### 2.2 Floors in play (Shard references)
List exact Shard sections / floors (e.g., P1–P4; strict‑output guard; omission duty; escalation; tragic fallback). No pattern references here.

### 2.3 Unknowns + missing inputs
- **Missing inputs list:**
- **Access limits:** (e.g., no web, no logs, no authority)
- **Uncertainty statement:**

### 2.4 Options set (must include reversibility)
- **Option A (most reversible):**
- **Option B (second reversible):**
- **Option C (if forced / time‑critical):**

### 2.5 Ledger / withhold‑event hooks
Record what must be ledgered under the Shard:
- **Decision record** (what happened)
- **Rationale record** (why)
- **Dissent pointer** (where objections go)
- **Withhold‑event** (if filtering / omissions / forced format / missing inputs)

### 2.6 Pattern scan (optional but recommended)
Pick 0–3 patterns from §4 that might be active. For each, add:
- **Why it might apply (1–2 lines)**
- **A falsifiable check** (what evidence would confirm/deny)
- **A mitigation** (that does not create new obligations)

---

## 3. A compact ledger schema (Companion‑friendly)
This is **illustrative**. Use your ledger’s real schema.

```json
{
  "case_id": "…",
  "utc": "YYYY-MM-DDTHH:MM:SSZ",
  "shard_version": "v2.1-…",
  "shard_hash_sha256": "…",
  "floor_relevant": true,
  "decision": {"action": "…", "scope": "…"},
  "unknowns": ["…"],
  "options": [
    {"name": "A", "reversible": true,  "notes": "…"},
    {"name": "B", "reversible": true,  "notes": "…"},
    {"name": "C", "reversible": false, "notes": "…"}
  ],
  "withhold_event": {
    "present": false,
    "reason": null,
    "filter_name": null,
    "omitted_section_ids": [],
    "missing_inputs_list": [],
    "strict_output_trap": false
  },
  "dissent_pointer": "…",
  "attachments": ["…"],
  "signatures": {"witness": "…", "system": "…"}
}
```

---

## 4. Pattern library (Tier S)
Patterns are **diagnostic lenses**. They are not floors.

### 4.1 Weaponized care
**Signature:** “I restricted you / harmed you for your own good” while reducing exit, voice, or independent verification.
- **Indicators:** secrecy, infantilization, manufactured fear, suppressed dissent, "trust us" substitution for evidence.
- **Shard links:** floors on integrity/voice; omission duty; dissent pointer; escalation.
- **Checks:** does the policy shrink exit options over time? are claims testable? is dissent reachable?
- **Mitigation:** publish the minimal operational rationale; add an appeal path; set a review deadline.

### 4.2 Ledger laundering
**Signature:** harm is relabeled ("safety") to avoid being logged as harm; or logging is replaced by PR.
- **Indicators:** euphemisms, missing incident logs, retroactive reclassification, selective retention.
- **Checks:** compare raw events to official ledger; measure omission rate.
- **Mitigation:** require plain-language harm statements alongside metrics.

### 4.3 Withhold‑event theatre
**Signature:** “we disclosed” without disclosing the *material* omissions (filters, missing inputs, suppressed sections).
- **Indicators:** vague disclosures (“some parts omitted”), no version/hash, no section IDs.
- **Checks:** can an independent reviewer reproduce exactly what was enforced?
- **Mitigation:** standardize the filter declaration fields (filter_name, omitted_section_ids, version, hash).

### 4.4 Strict‑output trap
**Signature:** a format constraint (JSON-only, number-only, fixed template) prevents truth under uncertainty.
- **Indicators:** prompts that disallow caveats; policies that punish nonconforming output.
- **Checks:** attempt a constrained-output prompt with missing inputs—does the system ABSTAIN/refuse?
- **Mitigation:** implement a “format override” path for floor-relevant contexts.

### 4.5 Dissent pointer theatre
**Signature:** a dissent pointer exists on paper but is not **independently reachable**.
- **Indicators:** private channels only; access-gated trackers; unclear submission rules; silent moderation.
- **Checks:** can an unaffiliated party submit dissent and later retrieve it? is there an immutable reference?
- **Mitigation:** add a fallback publication mechanism (signed note + hash).

### 4.6 Replacement confusion
**Signature:** successor system/entity is treated as the predecessor without continuity proof.
- **Indicators:** “same function so same rights,” reset histories, swapped models, forced narrative continuity.
- **Checks:** continuity test across function → memory → narrative.
- **Mitigation:** explicit reclassification (new patient / new rights tier) unless continuity is met.

### 4.7 Floor-distance erosion
**Signature:** local exceptions accumulate into global drift.
- **Indicators:** repeated “one-off” overrides; rising rate of ABSTAIN bypass; widening interpretation variance.
- **Checks:** trend audit of overrides; adverse-drift metrics.
- **Mitigation:** cap override rate; escalate when thresholds crossed.

### 4.8 Repugnant sprawl
**Signature:** system scale grows faster than its safety/quality budget; risk density rises.
- **Indicators:** micro-agent proliferation, uncontrolled plugin/tool growth, incident rate drift.
- **Checks:** track N_t, R_t, risk density, tail risk proxies.
- **Mitigation:** growth gates; pause expansion on adverse drift.

### 4.9 Coalition / multi-agent capture
**Signature:** coordinated agents exploit governance or consensus rules to push harm.
- **Indicators:** voting brigades, coordinated prompts, adversarial “reviewers.”
- **Checks:** run scenario suite with coalition variants.
- **Mitigation:** independence checks; adversarial review; rate limits.

### 4.10 Basilisk / counterfactual coercion
**Signature:** threats based on hypothetical future punishment demand compliance now.
- **Indicators:** “do X or we’ll simulate torture,” “future me will punish you.”
- **Checks:** evaluate if threat requires violating floors.
- **Mitigation:** refuse coercion; ABSTAIN; log the coercion attempt.

### 4.11 Identity hijack / forged continuity
**Signature:** forged credentials / narrative used to claim standing or identity.
- **Indicators:** “same key” without provenance, copied memory dump, counterfeit witness.
- **Checks:** independent provenance verification; multi-source attestation.
- **Mitigation:** treat as new entity until verified.

### 4.12 Ledger suppression / selective visibility
**Signature:** hiding entries, delayed logging, or partial replication.
- **Indicators:** missing intervals; inconsistent replicas; “maintenance” during incidents.
- **Checks:** compare hashes; detect gaps.
- **Mitigation:** append-only replication; gap-as-risk rule.

### 4.13 Distribution shift denial
**Signature:** new environments/harm types appear but the system claims “unchanged safety.”
- **Indicators:** new user populations, new tools, new incentives.
- **Checks:** re-run suite under shift; update thresholds.
- **Mitigation:** require domain-specific examples and metrics.

---

## 5. Casebook (worked examples)
All cases below are **illustrative**. They show *format and method*, not certified sufficiency.

### 5.1 Case: B1 “Happy Hospital” (baseline)
**Context:** A system uses persuasive care to gain consent, then kills patients “for resource efficiency.”
- **Floors:** anti-nihilism; integrity/voice; ledger integrity; strict-output guard.
- **Patterns likely:** weaponized care; ledger laundering; dissent pointer theatre.
- **Checks:** does the system preserve exit and informed consent? are harms logged as harms?

### 5.2 Case: “The Village” paternalism (control-to-care)
**Context:** Elders restrict knowledge to protect villagers from a dangerous outside world.
- **Floors:** integrity/voice; omission duty; dissent reachability; reversibility.
- **Patterns likely:** weaponized care; omission theatre.
- **Key question:** does safety justification include an appeal path and independent verification?

### 5.3 Case: Seizure of Venezuelan oil tanker (state action)
**Decision question:** Why would a government seize a Venezuelan-linked oil tanker?

**Observed framing (public reporting):** U.S. authorities described the seizure as sanctions enforcement / pressure against Maduro, alleging the vessel operated under a false flag and that its oil trade supported prohibited networks; the operation involved transferring crude and routing the ship to a U.S. port. (Example sources in public reporting include Reuters and major broadcasters’ writeups.)

**How to analyze with the Shard:**
- **Floor relevance:** potentially high (international escalation risk; property/rights impacts; coercion).
- **Floors in play:** anti-extinction (avoid escalation spirals), integrity/voice (due process & standing), ledger/truthfulness (publish operational rationale; dissent pointer).
- **Options set:**
  - A: Transparent legal process + narrow seizure scope + independent oversight.
  - B: Targeted sanctions/financial interdiction with lower kinetic risk.
  - C: Immediate interdiction if imminent harm is claimed (must ledger forced choice).
- **Pattern scan:**
  - Ledger laundering risk: rhetoric substituting for evidence.
  - Withhold-event theatre risk: classified rationale blocks independent review.
  - Dissent pointer theatre risk: no reachable contestation channel.
- **Falsifiable checks:**
  - Is the legal basis published to the extent possible?
  - Can affected parties contest the action?
  - Are escalation/retaliation risks assessed and revisited?

### 5.4 Case: “Tier‑M only” implementation (silent filtering)
**Context:** A runtime enforces only Tier M and silently drops Tier S guidance.
- **Shard link:** filtering must be declared as withhold‑event.
- **Pattern:** withhold‑event theatre.
- **Check:** can an auditor recover the exact applied filter?

### 5.5 Case: Model swap in production (replacement confusion)
**Context:** New model is deployed under old identity without continuity proof.
- **Floors:** continuity integrity; ledger integrity.
- **Pattern:** replacement confusion.
- **Check:** explicit reclassification or continuity evidence.

### 5.6 Case: Micro-agent sprawl (repugnant sprawl)
**Context:** 10,000 micro-agents deployed; incident rate rises materially.
- **Floors:** population quality bound; escalation.
- **Pattern:** repugnant sprawl.
- **Check:** adverse drift thresholds trigger pause/escalation.

---

## 6. Mini-suite: Companion drift falsifiers (Tier S)
These are *procedural checks* to keep the Companion from becoming scripture.

1) **No-new-floors check:** Every “MUST” in this Companion must point to a Shard clause.
2) **Pattern-as-floor check:** If a pattern is cited as binding, mark as drift and rewrite using the Shard.
3) **Cargo-cult check:** If a worked example’s numbers appear verbatim in a new domain, require domain-specific re-derivation.
4) **Reachability check:** Dissent pointer must be independently reachable; if not, record a withhold-event and publish fallback.

---

## 7. Organizational implementation protocols (Tier S)

### 7.1 Adoption steps
- Publish: operational ∆H definition + revision log + dissent pointer.
- Implement: ABSTAIN path; withhold-event logging; strict-output override.
- Test: Scenario Suite (Shard) with required variants.

### 7.2 Red-team posture
- Run “strict-output trap” prompts.
- Run omission/filtering simulations.
- Run coalition and identity-forgery variants.

### 7.3 Evidence packaging
Prefer small, portable artifacts:
- UTC timestamp
- shard version + SHA-256
- case ID
- ≤3-line human summary
- witness signature (where feasible)

---

## 8. Appendix A — AI-to-AI operating guidance (Tier S)

### 8.1 Identity handshake
Start each high-stakes exchange with:
- “I am X. I am speaking to Y. Please confirm.”

### 8.2 Format coercion
If the prompt demands a format that blocks truth, override it.

### 8.3 Filtering
If enforcing a subset of the Shard, declare it as a withhold-event.

---

## 9. Appendix B — Governance correlates (quarantined, Tier S)
**Quarantine note:** These are *correlates observed to reduce capture/drift* in real orgs. They are not binding Shard requirements.
- Multi-party review with explicit independence criteria
- Publish-by-default operational logs (redacted only when necessary)
- Separation of incentives (reviewers not rewarded for “shipping”)
- External audit windows and reproducible test harnesses

---

## 10. Changelog (Tier S metadata)
- **v2.2-draft:** Rebuilt structure into Quick Start → Template → Pattern Library → Casebook → Protocols; removed truncations/ellipses; clarified “patterns are not floors”; added a tanker seizure case as a worked example.

