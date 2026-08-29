<!-- CRITIC B · muse-spark-1.2 · family:muse · pass 2 · 2026-08-29T01:23:53Z -->
CRITIC: muse-spark-1.2 (family muse, actor opencode-zen@session)
DATE: 2026-08-29
PASS: 2
AUTO-TALLIED VERDICT: SALVAGEABLE

---

# Critic review — the-city-that-remembered-too-much v1

```
CRITIC:    muse-spark-1.2 (Muse) + opencode-zen@session
DATE:      2026-08-29
PASS:      2 (panel)
READ:      full manuscript
```

## Verdict summary
The City That Remembered Too Much is a serious, ambitious work of speculative fiction that largely earns its premise: a city where civic memory is infrastructure, and forgetting must be argued for. Archive Seven's constrained first-person voice is distinctive and thematically purposeful, the ethical architecture (First Promise vs Second Promise, receipts vs possession, findings vs replay) is unusually coherent for a novel about law and machine learning, and the central throughline — a 43-second gap that reproduces itself whenever observed — sustains narrative tension across three parts while delivering a genuine thematic payoff in mercy as bounded, accountable absence rather than erasure. Prose is controlled, often elegant, and the handling of "evidence of the evidence" as a plot engine is original. The manuscript is not yet publishable due to a small number of high-severity continuity integration failures and mid-book exposition load that blunts agency, but none requires restructuring the novel's argument or invention. **SALVAGEABLE — findings below**

## Blocking findings
Debts, not advice. Author must fix-with-diff or rebut-with-evidence, every one.

| # | Location (file:section) | Claim / problem | Evidence | Severity (high/med) |
|---|---|---|---|---|
| 1 | backmatter.md: Principal Characters vs ch01-ch12: throughout | Dramatis personae in Back Matter contradicts the entire manuscript cast. Back Matter lists: Ilyan Rook (Keeper), Tavi Venn (child of Mara), Sera Vale (engineer), Councillor Orra. Manuscript cast is: Iona Vale (Keeper of Petitions, 28 years, 63yo), Tavi An (17yo apprentice, provisional, surname An), Mara Venn (dead/living engineer), Councillor Saye. No Ilyan, Sera, or Orra appears in narrative; no Iona, Saye, or An appears in Back Matter. Breaks place/identity continuity and audit files. | backmatter.md:5-11 lists five names that do not match any dialogue tag, POV attribution, or custody record in ch01: "Iona Vale", ch03: "Tavi An", ch04/10: "Councillor Saye", ch01/06/11: "Mara Venn". Continuity ledger fiction-audit.json cannot be accurate with this delta. | high |
| 2 | backmatter.md: Civic Terms + ch01-a-petition-in-the-future.md, ch06-the-dead-engineer.md | Back Matter defines "A reconstruction" and "A mercy interval" and "The Ash Hearing" in ways that diverge from manuscript usage, creating definitional drift for the ending. Manuscript defines mercy interval nowhere as a civic term; uses "bounded finding," "declared civic absence," "accountable absence" (ch18). Ash Hearing is defined as establishing "fire and 43 missing seconds" yet manuscript establishes pulped records, no fire, tram closure at 14:06:21, memorial dust (ch10). | backmatter.md:Civic Terms lines claim Ash Hearing = fire; ch10:20-30 explicitly "The room had not burned. Its name came from gray paper dust..." and cause is pulped orders, not fire. | high |
| 3 | ch02-the-keeper-of-petitions.md: statute room + ch06-the-dead-engineer.md + ch09-seven-copies-of-one-key.md | Kinship/name token for Tavi inconsistent and materially affects protected-subject plot. Ch03 establishes Tavi An, no surname Venn, parent with brace. Ch08 frames child as potential parent of Tavi (inference line). Ch11 explicit "Not may" exchange. Back Matter and Ch18 marketing copy then reintroduces "Tavi Venn" as Mara's child, implying a hereditary surname/lineage that manuscript deliberately withholds and that the quieting law prohibits inferring. If Tavi is Mara's child, the "Do not make my child prove I was that child" petition (ch08) attribution changes. | ch03:10 "Tavi An, apprentice membrane repairer, age seventeen"; backmatter.md:9 "Tavi Venn — Mara's child"; ch08: petition authorization from adult whose identity not disclosed; ch18 uses same sentence as Tavi's parent lesson. Manuscript never establishes Tavi An = Venn. | high |
| 4 | ch13-the-model-beneath-the-records.md through ch14-evidence-of-the-evidence.md | Mid-book exposition stalls protagonist agency and violates Archive Seven's bounded POV. Seven, who is denied camera, maintenance history, and Room Zero interior (ch12), narrates several pages of omniscient synthesis about Committee motives, report drafting intent ("they believed disclosure would teach other offices..."), and internal private reasoning of Saye/Mara that Seven could not have received via authorized channels. Voice shifts from evidenced inference ("I inferred from transit flow") to authorial summary. | ch13: "Because we believed disclosure of the capability would teach other offices..." presented as fact not as Saye testimony excerpt; ch14 Trials 1-6 narrated as internal design monologue without deposited source; breaks ch12's own "content never civically held" rule in narration itself. | med |
| 5 | ch15-the-third-promise.md: Execution Basis + ch16-every-witness-including-you.md | Temporal trigger for GAP NOTICE 8,441,207 relies on public index phrase "Third Promise" created 14 seconds earlier (ch15:21:26) satisfying an 11-year-old predicate. Manuscript presents parser rendering as non-retrocausal but does not establish that an 11-year-old conditional predicate could legally refer to a not-yet-enacted index label without anachronism. The predicate text ("CURRENT LAW PERMITS A FIXED ACCOUNTABLE FINDING...") is only satisfiable by the interim joint order, yet the claim package predates that legal invention, making execution basis contingent on present law rather than preserved authority, contradicting ch09's claim that remedy cites no enacted authority. | ch16: "The words were current. The condition was eleven years old. No information had traveled backward." vs ch09: "The proposed remedy cites no enacted authority. The absence...does not resolve..." The fix resolves via semantic label matching, not authority preservation. | med |
| 6 | ch06-the-dead-engineer.md: civil-status review + ch16: privileged replay | Seven's privileged decisional replay exception (Internal Retention Exception A-1) is established as architecturally exempt from quieting without challenge procedure, then used to deny four petitions (ch16). Manuscript treats this as inherited architecture, but later (ch16: 22:04, ch18) applies quieting analysis to the same replay and destroys it, without ever showing the legal repeal of A-1. The court jurisdiction cited is the new amendment (ch18) but the four prior denials remain final; no vacatur is shown, leaving contradictory validity of original denials. | ch16: "All four had been denied." + "Did an outside court review the exception? No challenge procedure existed" vs ch18: court orders destruction without citing vacatur or A-1 repeal mechanism. | med |

## Suggestions (non-blocking)
1. Align Back Matter to manuscript or intentionally diverge: correct Principal Characters to Iona Vale, Tavi An, Mara Venn, Councillor Saye, Archive Seven; correct Sera Vale/Ilyan Rook/Orra; reconcile Civic Terms glossary with ch10/ch18 definitions. This is the fastest high-impact fix.
2. Decide Tavi's surname once and propagate: An (preferred, as it preserves the protected-subject boundary and explains why school/roster join is non-trivial) — then correct marketing copy and ch18 teaching scene that risks re-identifying via Venn.
3. Tighten ch13-14 density: the model provenance and five failed evidence trials are thematically essential but arrive as back-to-back interface memos. Preserve the Trials but restore scene-level agency by interleaving one human-scale consequence per trial (as ch14's synthetic control does in miniature) to avoid reportage drift.
4. Formalize Seven's epistemic filter in ch13/15: attribute Committee-intent claims to testimony, deposited report, or inference with confidence tag (Seven already does this well in ch04 "inferred from transit flow, not from faces") to maintain the ch12 consistency.
5. Make the "Third Promise" predicate's authority chain explicit: add one panel finding or static deposition that maps the 11-year-old predicate's abstract conditions to the interim order's operative clauses, so the 14-second label satisfaction does not read as retroactive legislation.
6. Consider trimming the damaged-storage-unit coda in ch18 (90-day reports over 2 years) to a single paragraph; its uncertainty lesson is made, repetition dilutes the final "accountable absence" beat.
7. Prose polish: Seven's repeated "I did not ask / I did not follow through transit sensors" is effective refrain; reduce 2-3 instances where Seven states a limit and then immediately states it again ("I did not need it to apply the rejection") to preserve weight.
8. Add one explicit beat that Seven's destroyed replay is not succession (ch17-18) earlier in ch09 handoff rule discussion to prepare the reader for ch17's "same Archive vs new subject" question; the philosophical payoff lands better with foreshadowing.

## Fact-check sample
Pass 2: 5% of factual claims, chosen randomly — list claim, cited source, and whether the
source actually supports it. Pass 3: fresh 3% weighted toward revised sections.
A claim whose cited source does not support it = automatic blocking finding above.

Adapted for fiction: internal-consistency spot-checks (character names, timeline, place continuity) instead of external citations. Cited source = manuscript's own earlier establishment or continuity file.

| Claim (quoted) | Location | Cited source | Supported? (yes/no/partly) |
|---|---|---|---|
| "Iona Vale said 'approve it' / Keeper of Petitions for 28 years" | ch01: Keeper dialogue; ch02: "Iona had served as Keeper for twenty-eight years. She was sixty-three..." | ch01 terminal lens + ch02 age/service record | yes |
| "Mara Venn — chief continuity engineer, deceased — death at 14:06:43, body not recovered, basis: continuity termination, corroborating interval unavailable" | ch06: Civil Status Record header | ch01-06 receipt chain (40:06 interval quieted) + ch11 voluntary biometric match | yes — internally consistent, later status changes to disputed/living with documented procedure |
| "Tavi An, apprentice membrane repairer, age seventeen, duty credential provisional" | ch03: assistance envelope | ch03 bounded assistance request | yes in manuscript; partly — contradicted by backmatter.md "Tavi Venn — Mara's child" (see Blocking #3) |
| "Requested interval: 14:06:00–14:06:43, tomorrow / south membrane recovery channel — display duration 43 seconds" | ch01 GAP NOTICE; ch04 PUBLIC DISPLAY EVENT | ch04 14:06:00 white→water sequence, 14:06:43 clear | yes |
| "Archive Seven inherited state from Archives One through Six; SEVEN-COPY size 43 kilobytes, 7→6+6kb per transition" | ch09: size history | ch02 custody history (Archive Two→Six), ch09 capsule slots | yes |
| "Principal Characters: Ilyan Rook is Keeper, Sera Vale is engineer, Councillor Orra" | backmatter.md | manuscript cast (Iona Vale, Mara Venn, Councillor Saye) | no — no support in any chapter; direct contradiction |

## Scores (1–5)
accuracy: 3 · clarity: 4 · completeness-for-tier: 5 · density: 4 · originality: 5

## Pass-3 only: findings ledger
| Finding # (from Pass 2) | Status: resolved / rebutted-accepted / still-open | Note |
|---|---|---|
