# Portfolio Dashboard

Generated: 2026-07-01 12:55 UTC

This public dashboard is a sanitized portfolio summary. Raw ledgers, source
archives, private schemas, and active prediction internals are not included.

## Engines

| Engine | Family | Status | Week |
|---|---|---|---|
| IDN_NI | ResourceCountry | active | 2026-W18 |
| FOMC | CentralBank | active | 2026-W25 |
| ODAC | RegulatoryCommittee | monitoring | 2026-W18 |
| AI_CAP | SemiconductorCompute | active | 2026-W27 |

## Engine Notes

### IDN_NI: IDN-NI Resource Policy Engine

Indonesia nickel policy, RKAB execution, substitution flow, and market transmission engine.

- Family: `ResourceCountry`
- Status: `active`
- Packet generated at: `2026-04-28`

**Notable Updates**
- Initial Metis manifest connected IDN_NI as the ResourceCountry family seed engine.
- Current engine state exposes open RKAB predictions and active belief ledger to the portfolio dashboard.

**Open Questions**
- Which open B6/RKAB predictions are closest to resolution and should be reviewed first?

**Needs Human Review**
- Review whether IDN_NI remains active weekly or should move to event-triggered active monitoring after current RKAB windows close.

**Cross-Engine Candidates**
- [ODAC] IDN_NI's institution-path error attribution may map to ODAC vote-to-decision bridge errors.

### FOMC: FOMC Voter Thesis Engine

FOMC voter, statement, dot plot, dissent, and framework-level consensus gap engine.

- Family: `CentralBank`
- Status: `active`
- Packet generated at: `2026-06-18`

**Notable Updates**
- June 17 statement-week added three pre-meeting baseline rows plus official resolution evidence, culminating in [private-id] for the unanimous 12-0 hold.
- The June live-prep cycle created two watch candidates: zero dovish dissent and unanimous-versus-topology, and both were resolved true at statement time without forcing formal prediction registration.
- The June statement strengthened the voter-profile dissent-threshold lesson and updated the April topology lesson with a unanimous counterexample, reinforcing topology separation rather than recurrence.
- A statement-day postmortem now records June 17 as a unanimous-hold reset under Warsh's shorter, more declarative communications style.

**Open Questions**
- When the June 2026 minutes are released, do they show genuine internal unanimity or only a unanimous final vote with compressed statement packaging?
- Does Warsh's shorter statement style persist into the next meeting, or was June a one-meeting debut effect?
- Should the June unanimous-hold reset eventually promote [private-id] from draft, or do we still need another comparable sample?

**Needs Human Review**
- Review the June minutes through the vote-topology lens before adding any new topology or communications lessons.
- Decide whether the June watch objects should remain watch-only examples or be harvested into a reusable pre-registration discipline note.
- Keep [private-id] in draft until another minutes cycle tests the quantifier thesis against a fresh meeting.

**Cross-Engine Candidates**
- [Metis Core] FOMC's June statement cycle is a good example of how watch objects can improve judgment and lessons without creating low-quality calibration samples.
- [ODAC] The distinction between narrow count objects and broader topology objects may transfer to other engines that model unanimous outcomes versus latent internal splits.

### ODAC: ODAC Minimal Thesis Engine

FDA ODAC case replay and live-ready advisory committee concern/vote/decision bridge engine.

- Family: `RegulatoryCommittee`
- Status: `monitoring`
- Packet generated at: `2026-04-28`

**Notable Updates**
- Initial Metis manifest connected ODAC as the RegulatoryCommittee family seed engine.
- ODAC currently appears replay-rich: resolved predictions, concern registry, and active lessons are visible to dashboard.

**Open Questions**
- Which replay lesson should be promoted upward to a RegulatoryCommittee family rule candidate?

**Needs Human Review**
- Decide whether ODAC should stay monitoring or receive a next live/replay case trigger.

**Cross-Engine Candidates**
- [FOMC] ODAC concern activation can inform FOMC dissent-threshold modeling as a structured salience problem.

### AI_CAP: AI CAP Thesis Engine

Advanced process, CoWoS, HBM, hyperscaler capex, and AI infrastructure scarcity thesis engine.

- Family: `SemiconductorCompute`
- Status: `active`
- Packet generated at: `2026-06-29`

**Notable Updates**
- [private-id] was formally updated from [private-probability] to [private-probability] after the CoWoS proxy baseline and approval checks were completed.
- [private-id] was upgraded to official_and_proxy_supply_baseline with confidence [private-probability], improving the HBM research baseline without overruling the missing price-consensus gate.
- AI_CAP adopted the new history-compression review pattern with a local variant: golden cases and monthly compression are now tracked explicitly, while `reviews/` remains the current lesson-registry surrogate.
- [private-id] remains in research-only proxy review, while [private-id] remains applied at [private-probability] with no new independent probability evidence this cycle.

**Open Questions**
- Can [private-id] secure a recurring HBM contract-price proxy or sell-side price baseline, rather than only supply-commitment evidence?
- Does [private-id] need any further probability review before the next material CoWoS datapoint, now that it has been updated to [private-probability]?
- Will the next NVDA earnings cycle provide enough direct data-center consensus to move [private-id] beyond its current open / research-only proxy path?
- Which AI_CAP local patches are stable enough to promote to a SemiconductorCompute family pattern without compressing away domain-specific distinctions?

**Needs Human Review**
- Find or archive an HBM contract-price proxy or sell-side price baseline for [private-id] before considering any probability move.
- Keep [private-id] in research_only proxy mode until direct consensus or a separately approved scope change appears.
- Review whether any alternative-demand or faster-supply hypotheses deserve strengthening after the latest [private-id] update.
- Use `private artifact` before simplifying any baseline or proxy gate that might affect future regression safety.

**Cross-Engine Candidates**
- [Metis Core] The AI_CAP baseline progression pattern now has two examples: CoWoS moved through baseline-to-approval-to-apply, while HBM moved through baseline-to-still-blocked. This should inform a reusable baseline maturity ladder.
- [SemiconductorCompute family] Monthly compression plus golden-case regression is now adopted in AI_CAP with a local lesson-registry variant.
