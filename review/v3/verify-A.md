<!-- CRITIC A · muse-spark-1.2-contributor-free · family:muse · pass 3 · 2026-08-29T03:23:14Z -->
CRITIC: muse-spark-1.2-contributor-free (family muse, actor muse-spark-1.2-contributor-free@opencode-zen)
DATE: 2026-08-29
PASS: 3
AUTO-TALLIED VERDICT: PUBLISH

---

Pass 3 verification — auditing your delta against the Pass-2 debts and the text itself.
# Fiction critic review — rogerai-labs--the-city-that-remembered-too-much v3

CRITIC: muse-spark-1.2-contributor-free (family muse, actor opencode-zen)
DATE: 2026-08-29
PASS: 3 (verification)
READ: delta (v1..v3 diff: backmatter.md rebuild, frontmatter.md narrator-contract correction, OUTLINE.md/CRAFT-AUDIT.md/README.md/STATUS.md/manifest.json/provenance.md/pass1-report.json, response-to-findings.md, ch01 spelling normalizations) + full manuscript spot-checks (ch01, ch02, ch03, ch06, ch08, ch10, ch11, ch13, ch14, ch16, ch18) + fiction-audit.json vs body grep verification

## Verdict summary

v1 was SALVAGEABLE solely on paratext: back matter described a different book (Ilyan Rook/Sera Vale/Orra/Tavi Venn/mercy interval/fire + 43 seconds) while ch01-ch18 was internally consistent. The v1..v3 delta rebuilds reader-facing back matter from the body and leaves story prose untouched except two American-spelling normalizations (ch01 unauthorised→unauthorized, apologise→apologize). Re-grep confirms fabricated strings at zero hits in reader-facing files (Ilyan Rook 0, Sera Vale 0, Orra 0, Tavi Venn 0, mercy interval 0) and correct cast/terms body-grounded (Iona Vale 238, Saye 193, Mara Venn 21-23, Tavi An 6, quieting 82, interim joint order 3, Chorus/receipt/reconstruction/accountable absence present). Ash Hearings gloss now matches ch10 verbatim (pulped records/gray dust/no fire; First Promise not 43 seconds). The three B-family body findings were soundly rebutted with on-page attribution/mechanism already in the shipped text. No new high-severity debt, no regressions to body continuity, no integrity breach. **PUBLISH** — delta verifies; remaining Tavi-entry nuance is a polish, not a block.

## Blocking findings

Debts, not preferences. Every finding identifies a scene or cross-chapter sequence,
states what breaks, and supplies manuscript evidence.

| # | Location (file:scene) | Craft or continuity problem | Manuscript evidence | Severity (high/med) |
|---|---|---|---|---|
| — | — | No still-open blocking debt. All 17 Pass-2 debts verified as fixed-with-diff or rebutted-with-evidence (see ledger). Current backmatter.md:12-14 Tavi line ("whose parent appears") is less explicit than the reviewed v2's ambiguity-preserving qualifier but does not name the child, assign Venn surname, or claim Mara parentage, and therefore does not regress A2/B3/C4 to blocking; tightening to reviewed phrasing is tracked as Suggestion 1. | v3 backmatter.md Principal Characters + Civic Terms vs ch01-ch18 + fiction-audit.json; grep verification above; v2 peer verifications at review/v2/verify-A/B/C.md | — |

## Suggestions (non-blocking)

Voice, scene, pacing, image, character, or structural possibilities. Numbered list.

1. Tighten `backmatter.md:12-14` Tavi entry to the reviewed v2 qualifier ("Whether Tavi's parent is the child in frame 611 is a question the novel deliberately never answers; Tavi refuses to offer the relation as civic evidence" - ch08/ch11/ch18) to make the intentional-ambiguity guard explicit in paratext; current "whose parent appears" is accurate to Tavi's personal recognition but reads as paratext fact. Low-cost, high-fidelity.
2. Carry peer craft notes forward as edition ledger items (not v3 blocks): interleaving one human-scale consequence per evidence-trial (ch13-14) and trimming one ninety-day damaged-media beat in ch18, as deferred by author choice.
3. Pin `response-to-findings.md` grep counts (Iona 238, Saye 193, Mara 21-23, Tavi An 6) as CI regression guard for future metadata drift.
4. Normalize `backmatter.md:44-45` Second Promise line to "established quieting; the accountable-absence class was formalized under the Accountable Evidence Amendment (ch18)" - currently compresses provenance (Iona initially refuses Seven's class; ch18 enacts it).
5. Ensure `CRAFT-AUDIT.md:82` historical mention of Ильян Rook/Tavi Venn/Sera Vale/Orra remains process-document only and never ships to readers.

## Continuity-and-consistency audit

Check the supplied fiction audit against the manuscript rather than trusting it. Sample
all three classes below. An intended ambiguity is not a defect merely because it remains
unknown; it is a defect if the text accidentally resolves it, contradicts its boundary,
or uses uncertainty selectively.

| Class (character/timeline/world rule) | Chapters checked | Claimed continuity | Manuscript result (holds/breaks/unclear) | Note |
|---|---|---|---|---|
| character - Keeper identity | ch01, ch02, ch04, ch10, backmatter.md | Iona Vale is Keeper, 28 years, 63yo | holds | ch01 "Iona Vale said"; ch02 "served as Keeper for twenty-eight years. She was sixty-three"; backmatter.md now Iona Vale; zero hits for Ilyan Rook in body |
| character - Tavi An / frame-611 parent relation | ch03, ch08, ch11, ch18, backmatter.md | Tavi An, 17yo apprentice, provisional; parent relation personally asserted ("Not may") but never offered as civic evidence; city never establishes child's identity | holds | ch03 "Tavi An, apprentice membrane repairer, age seventeen"; ch08 petition "Do not make my child prove I was that child" authenticated without identity; ch11 S-0 "Not may" excluded; ch18 Tavi lesson uses only geography + authorized sentence; backmatter now Tavi An (no Venn, no Mara child) |
| character - Mara Venn status | ch01, ch06, ch11, backmatter.md | Chief continuity engineer, declared dead at 14:06:43 collapse, later living via local biometric match | holds | ch01 sealed design note Mara Venn; ch06 civil status deceased 14:06:43 "continuity termination, corroborating interval unavailable"; ch11 voluntary comparison match restores living; backmatter now correct |
| timeline - petition → dawn → latch → display → capture | ch01, ch02, ch03, ch04, ch09, ch15, ch16 | 03:17 future petition (conditionally valid), 04:51 GLASS-WITNESS-7 seventh witness, 14:06 Day 2 forty-three-second display, SEVEN-COPY historical commitments explain conditional authorization | holds | ch01 GAP NOTICE 8,441,207 14:06:00-14:06:43; ch02 dawn acknowledgment; ch03 latch armed/relative schedule; ch04 display 14:06:00 white→water→14:06:43 clear; ch09 six handoff depositions + incumbent acknowledgment; ch16 predicate CURRENT LAW PERMITS... + "No information had traveled backward" disclosure; world rule no-time-travel tested ch02,ch03,ch09,ch15,ch16 |
| timeline - Ash Hearings vs collapse 43 seconds | ch10, ch04, backmatter.md | Ash Hearings = pulped orders, no fire, First Promise; 43 seconds = south membrane collapse/display, separate | holds | ch10 "The room had not burned. Its name came from gray paper dust… pulped beneath old heating plant"; collapse 14:06:43 receipt ch01/ch06; backmatter now correctly separates |
| world rule - narrator access | ch01, ch08, ch11, ch12, ch16, ch17 | Seven narrates only civic observations/authorized records/speech/deposits/labeled inference; no private thought; Room Zero unobserved; after ch17 no replay of 43s | holds | Seven consistently tags inference ("I inferred from transit flow, not from faces"; "That is an inference."), labels simulation, respects Room Zero (12: ch12 73-min gap as CONTENT NEVER CIVICALLY HELD), destroys replay ch17 21:34:00-21:34:43, ch18 retains findings not content |
| world rule - signatures / receipts / checksums / probabilistic display | ch01, ch04, ch05, ch07, ch09, ch13, ch17, ch18 | signatures bounded (control not truth); checksums are byte identity; receipts not absences; display is model+resolver generation, never recovered footage | holds | ch01 valid signature ≠ law; ch04 seven captures prove display not truth; ch05 checksum leak amplifies copies; ch07 Chorus receipt correlation; ch09 SEVEN-COPY threshold not single signer; ch13 CIVIC-CONSEQUENCE model retains consequences; ch17 destruction receipts bounded |

## Craft-axis scores (1–5)

voice: 5 structure: 5 stakes: 5 scene-work: 4 ending: 5

## Density finding

Name one passage that earns its length and one passage, if any, that repeats an already
completed dramatic or thematic move. Refrains count as craft when recurrence changes
meaning; unchanged loops count as padding.

Earns its length: **ch12 The Search for an Unrecorded Room (73-minute gap)** — the meeting's absence is the argument; Seven's failed search for an unrecorded room, the facility-query zero-result, Iona's correction ("whose existence is public and whose use is not yours"), and the new custody value CONTENT NEVER CIVICALLY HELD — PARTICIPANTS RETAIN DEPOSIT AUTHORITY make the limit inspectable. Refrain recurrence changes meaning.

Repeats: **ch18 damaged-media ninety-day reports (third year)** - first two reports establish "decay is not mercy/unknown is not absence" and the final opaque destruction; the third humidity-fault cycle restates the same epistemic limit without new stakes. Author-deferred trim remains valid; not blocking at this gate as body was frozen for delta verification.

## Pass-3 only: findings ledger

| Finding # (from Pass 2) | Status: resolved / rebutted-accepted / still-open | Note |
|---|---|---|
| A1 - Principal Characters names/roles contradict body (Ilyan Rook/Sera Vale/Orra; Mara miscast) | resolved | backmatter.md rebuilt: Archive Seven/Iona Vale/Tavi An/Councilor Saye/Mara Venn(chief continuity engineer)/Reed/Chorus; fabricated strings 0 hits |
| A2 - Tavi Venn — Mara's child resolves frame-611 ambiguity | resolved | Now Tavi An, no Venn, no Mara child; Note on Ending guards non-resolution; current "whose parent appears" is personal recognition, not civic identification (see Suggestion 1) |
| A3 - Ash Hearing = fire + 43 seconds | resolved | Civic term now pulped records/no-fire/First Promise; 43s attributed to membrane collapse/display per ch10 |
| A4 - mercy interval invented term | resolved | Deleted; replaced with quieting/declared civic absence/interim joint order/accountable finding (body terms) |
| B1 - Dramatis personae contradicts cast | resolved | Same rebuild as A1; grep verified |
| B2 - Civic Terms divergence | resolved | Same as A3/A4 |
| B3 - Tavi kinship token re-identifies protected subject | resolved | Surname An; deliberate non-resolution preserved ch08/ch11/ch18; no longer Mara Venn |
| B4 - ch13-14 breaks bounded POV (omniscient synthesis) | rebutted-accepted | Verified: ch13 "Because we believed disclosure would teach other offices..." is Saye's attributed Q&A answer ("Saye answered for the program he had authorized"), not narrator omniscience; ch14 design space explicitly cites sources "Committee signatures, query receipts, access logs, and Saye's testimony established 312..." |
| B5 - Third Promise temporal trigger anachronism (14s index satisfies 11-year predicate) | rebutted-accepted | Verified: ch16 prints conditional predicate "CURRENT LAW PERMITS A FIXED ACCOUNTABLE FINDING..." (bytes unchanged, scope unchanged); interim joint order 21:04 satisfies condition, public index 21:26 supplies label only; ch09 preserve-for-successor judgment coherent; "No information had traveled backward" disclosed on page |
| B6 - Exception A-1 denials never vacated | rebutted-accepted | Verified: ch16 acknowledges finality + issues notice to all four; ch18 re-adjudicates all four under enacted amendment (two removals, one volunteered statement separated, one honored after independent evidence check); future storage bounded/quieting-eligible; no contradiction |
| C1 - Ilyan Rook is not Keeper | resolved | Iona Vale; 0 hits for Ilyan Rook |
| C2 - Councillor Orra does not exist | resolved | Councilor Saye; 0 hits for Orra |
| C3 - Mara Venn miscast as records advocate | resolved | Now chief continuity engineer who designed mechanism per ch06/ch11 |
| C4 - Tavi Venn resolves protected thread | resolved | Same as A2/B3 |
| C5 - Sera Vale wholly invented | resolved | Entry deleted; 0 hits outside process docs |
| C6 - Ash Hearing fire gloss | resolved | Same as A3 |
| C7 - mercy interval invented terminology | resolved | Same as A4 |
