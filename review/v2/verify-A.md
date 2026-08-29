<!-- CRITIC A · claude-opus-4.8 · family:anthropic · pass 3 · 2026-08-29T02:16:42Z -->
CRITIC: claude-opus-4.8 (family anthropic, actor claude-opus-4.8@session)
DATE: 2026-08-29
PASS: 3
AUTO-TALLIED VERDICT: PUBLISH

---

# Critic review — rogerai-labs--the-city-that-remembered-too-much [v2]

```
CRITIC:    claude-opus-4.8 (family anthropic, actor claude@session)
DATE:      2026-08-28
PASS:      3 (verification)
READ:      delta (backmatter.md rebuild, response-to-findings.md, manifest.json, pass1-report.json) + targeted body re-reads for the rebutted findings (ch05, ch08, ch10, ch11, ch13, ch14, ch15, ch16, ch18)
```

## Verdict summary
The v1→v2 delta does exactly what the panel asked and nothing it was warned against: the story prose is untouched, and the back-matter apparatus has been rebuilt from the actual body. I independently verified every name and term claim: the fabricated strings (`Ilyan Rook`, `Sera Vale`, `Orra`/`Councillor Orra`, `Tavi Venn`, `mercy interval`) return zero hits in the v2 reader-facing files, while the corrected cast and terms are all body-grounded — Iona 238 body hits (ch02 confirms 28 years / age 63), Saye 193 (ch04 confirms nine-year Continuity chair, ch15 the resignation), Mara Venn 21 (ch06 civil-status record, ch11 return), Tavi An 2 (ch03, age seventeen), Reed 55, quieting 63, interim joint order 3 (ch15's order title verbatim). The Ash Hearings gloss now matches ch10's pulped-records/no-fire account, and the "Note on the Ending" explicitly guards the frame-611 non-resolution instead of breaking it. Critic B's three rebutted body findings (B4/B5/B6) all check out against the shipped text: the "disclosure would teach other offices" line is Saye's attributed dialogue, not narrator omniscience; the "Third Promise" trigger is a self-disclosed conditional predicate satisfied by present law, with ch16 doing the anti-retrocausal work on the page; and ch16/ch18 explicitly handle the A-1 denials' finality (notice to all four, new petitions under the enacted amendment, court-ordered removal) rather than leaving them contradictory. One new debt surfaced during independent verification: the local repository's working-tree back matter is a *different* post-fix variant than the reviewed v2, and its Tavi entry ("whose parent appears in the public reconstruction") would partially regress findings A2/B3/C4 if it shipped; the packet's diff SHAs (d26346b..641f038) do not resolve in the repo copy I can access, so which artifact is canonical must be reconciled before signing. The reviewed v2 itself is clean. Overall: **VERIFIED** (all seventeen pass-2 findings resolved or soundly rebutted against the reviewed v2), conditioned on the intake commit carrying the reviewed back matter, not the divergent repo variant. **PUBLISH**

## Blocking findings

| # | Location (file:section) | Claim / problem | Evidence | Severity (high/med) |
|---|---|---|---|---|
| 1 | repo working tree `backmatter.md` vs reviewed v2 `backmatter.md` (artifact reconciliation) | The repository copy at HEAD (661653a) carries a *different* rebuilt back matter than the v2 under review; its Tavi entry states "a membrane repair apprentice whose parent appears in the public reconstruction," which asserts as paratext fact the very relation the body keeps as unverified personal assertion (ch08 "Do not make my child prove I was that child"; ch11 "Not may" — offered and then excluded from civic evidence) — a partial regression of A2/B3/C4. The packet's delta SHAs d26346b/641f038 do not exist in the accessible repo history, so I could not confirm the reviewed bytes are the bytes staged for intake. | `git log` shows 661653a…82fa651, no d26346b/641f038; repo `backmatter.md:12-14` vs reviewed v2 backmatter ("a question the novel deliberately never answers"); grep confirms both variants are post-fix (correct names) but textually distinct. | med |

## Suggestions (non-blocking)
1. Reconcile the two post-fix back-matter variants into one canonical file before the intake commit; if any of the repo variant's additions are kept (e.g., the useful "The Chorus" entry), rewrite its Tavi line to the reviewed v2's ambiguity-preserving form.
2. Manifest review-trail dates are out of order: `panel-2` is dated 2026-08-29 while `revision-v2` (which responds to it) is dated 2026-08-28. Likely a timezone artifact, but for a press whose brand is the visible trail, normalize the timestamps.
3. The v2 glossary's "the Second Promise established quieting and civic absence" slightly compresses provenance: quieting is Second Promise, but "declared civic absence" as a formal class is created in ch18 under the Accountable Evidence Amendment (Iona initially refuses Seven's proposed class; it enacts only with the amendment). Consider "…established quieting; the amendment years later formalized its result as a declared civic absence."
4. The author's B6 citation set includes the "reopened ACCOUNTABLE ABSENCE 000001" line, which concerns the gap's integrity classification, not the four A-1 petitioners; the substantive support (ch18 "The four people denied… returned to the Quieting Court…"; "The court ordered the content removed") is correct on its own — drop the stray cite in any future response doc.
5. `CRAFT-AUDIT.md:82` still names Ilyan Rook / Tavi Venn / Sera Vale / Orra as part of the fix's historical record. Acceptable in a process document; just ensure it never ships as reader-facing matter.
6. The pass-2 craft notes (Part III density, ch18 coda trim, refrain thinning) remain valid and remain deferred by explicit choice; carry them on the ledger for a future edition rather than letting them silently expire.

## Fact-check sample
(Pass 3 fiction adaptation: fresh internal-consistency checks, ~3% of claims, weighted toward the revised section — the rebuilt back matter — plus the body passages cited in the B4–B6 rebuttals. Verified against the operator-supplied v2 manuscript and greps over the local repo copy; noted above where the two artifacts diverge.)

| Claim (quoted) | Location | Cited source | Supported? (yes/no/partly) |
|---|---|---|---|
| "Iona Vale — Keeper of Petitions for twenty-eight years, sixty-three years old" | v2 backmatter: Principal Characters | ch02 "Iona had served as Keeper for twenty-eight years… She was sixty-three" | yes |
| "Tavi An — a seventeen-year-old apprentice membrane repairer" + parent/frame-611 "deliberately never answers" | v2 backmatter: Principal Characters | ch03 "Tavi An, apprentice membrane repairer, age seventeen"; ch08/ch11/ch18 (relation asserted personally, excluded from civic evidence) | yes |
| "Councilor Saye — chair of Continuity for nine years, a former records advocate… finally resigns his chair" | v2 backmatter: Principal Characters | ch04 "Saye had chaired Continuity for nine years. He had been a young records advocate…"; ch15 "Saye resigned as Continuity chair effective immediately" | yes |
| "Mara Venn — chief continuity engineer, declared dead after the 14:06:43 collapse and later found alive. She designed the mechanism…" | v2 backmatter: Principal Characters | ch06 civil-status record; ch11 "VOLUNTARY IDENTITY COMPARISON: match" + Mara's design admissions | yes |
| "The Ash Hearings — …municipal maintenance orders found pulped beneath the old heating plant. The room had not burned…" | v2 backmatter: Civic Terms | ch10 "The room had not burned. Its name came from the gray paper dust… records were found pulped beneath the old heating plant" | yes |
| "The First Promise made forgetting anyone administratively difficult"; Third Promise "exists in the public index as a pointer to the interim joint order rather than as enacted law" | v2 backmatter: Civic Terms | ch10 (verbatim); ch15 "THIRD PROMISE, PROPOSED — SEE INTERIM JOINT ORDER…" + "The law contained no Third Promise" | yes |
| "the Second Promise established quieting and civic absence" | v2 backmatter: Civic Terms | quieting: yes (ch10/ch18); "declared civic absence" as formal class enacts only with the ch18 amendment | partly (see suggestion 3) |
| "Because we believed disclosure of the capability would teach other offices…" is attributed spoken testimony, not narrator omniscience (B4 rebuttal) | response-to-findings.md: B4 | ch13 Q&A exchange: "Why didn't the reports say that?" → Saye's answer → "And an institutional advantage. I did not name the second reason in the reports." | yes |
| "No information had traveled backward" — predicate conditional, satisfied by present law, not retroactive authority (B5 rebuttal) | response-to-findings.md: B5 | ch16 predicate text + parser explanation; consistent with ch09 "preserve for successor judgment" | yes |
| A-1 denials re-adjudicated under enacted law, not left contradictory (B6 rebuttal) | response-to-findings.md: B6 | ch16 "Their denials were legally final… The Quieting Court could accept new petitions. I issued notice to all four"; ch18 "The four people denied… returned to the Quieting Court…"; "The court ordered the content removed" | yes |
| "`Tavi Venn` 0 body hits, `mercy interval` 0, `Sera Vale` 0, `Orra` 0" (author verification snapshot) | response-to-findings.md: snapshot table | independent grep over ch01–ch18 + v2 backmatter: all zero in reader-facing files (one historical mention in CRAFT-AUDIT.md only) | yes |

## Scores (1–5)
accuracy: 5 · clarity: 4 · completeness-for-tier: 5 · density: 3 · originality: 5

## Pass-3 only: findings ledger

| Finding # (from Pass 2) | Status: resolved / rebutted-accepted / still-open | Note |
|---|---|---|
| A1 (cast contradicts body: Ilyan Rook / Sera Vale / Orra / Mara miscast) | RESOLVED | Rebuilt from body; grep confirms fabricated names at 0 hits, Iona Vale / Mara Venn (engineer) / Councilor Saye entries body-accurate |
| A2 (Tavi Venn — Mara's child resolves frame-611 ambiguity) | RESOLVED | Now "Tavi An"; entry and Note on the Ending explicitly preserve the non-resolution |
| A3 (Ash Hearing = fire + 43 seconds) | RESOLVED | Gloss now matches ch10 (pulped records, no fire); 43 seconds no longer attributed to the Hearings |
| A4 ("mercy interval" invented term) | RESOLVED | Deleted; replaced with body-real quieting / declared civic absence / interim joint order / accountable finding |
| B1 (dramatis personae contradicts cast) | RESOLVED | Same rebuild as A1; Reed and Archive Seven added, all entries verified against dialogue tags |
| B2 (Civic Terms divergence) | RESOLVED | Same as A3/A4 |
| B3 (Tavi kinship token re-identifies protected subject) | RESOLVED | Surname fixed to An; parent relation left unresolved in both entry and ending note — but see Blocking #1: the divergent repo back-matter variant would partially regress this if it, not the reviewed v2, ships |
| B4 (ch13–14 breaks Seven's bounded POV) | REBUTTED-ACCEPTED | Verified: the cited line is Saye's on-page deposition answer; ch14's enumerations name their sources of record ("Committee signatures, query receipts, access logs, and Saye's testimony established 312…"); Seven's inferences elsewhere are tagged ("I revised my model of Saye") |
| B5 (Third Promise reads as retroactive legislation) | REBUTTED-ACCEPTED | Verified: ch16 discloses the conditional-predicate mechanism (petition bytes unchanged, label from public index, "No information had traveled backward"); coheres with ch09's preserve-for-successor-judgment design. B's suggestion 5 remains good craft advice for a future pass |
| B6 (A-1 denials never vacated) | REBUTTED-ACCEPTED | Verified: ch16 acknowledges the denials' finality and issues notice; ch18 shows all four re-adjudicated under the enacted amendment with court-ordered removal. Coherent by design, not contradictory. (Author's "reopened ACCOUNTABLE ABSENCE" cite is stray but non-load-bearing — suggestion 4) |
| C1 (Ilyan Rook is not the Keeper) | RESOLVED | Now Iona Vale; 0 hits for Ilyan Rook |
| C2 (Councillor Orra does not exist) | RESOLVED | Now Councilor Saye, body spelling; 0 hits for Orra |
| C3 (Mara Venn miscast as records advocate) | RESOLVED | Now chief continuity engineer who designed the mechanism, per ch06/ch11 |
| C4 (Tavi Venn resolves protected thread) | RESOLVED | Same as A2/B3; same repo-variant caveat as B3 |
| C5 (Sera Vale wholly invented) | RESOLVED | Entry deleted; 0 hits outside process docs |
| C6 (Ash Hearing fire gloss) | RESOLVED | Same as A3 |
| C7 (mercy interval invented terminology) | RESOLVED | Same as A4 |
