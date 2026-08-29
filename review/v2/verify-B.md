<!-- CRITIC B · muse-spark-1.2 · family:muse · pass 3 · 2026-08-29T02:16:52Z -->
CRITIC: muse-spark-1.2 (family muse, actor muse-spark-1.2@opencode-zen)
DATE: 2026-08-29
PASS: 3
AUTO-TALLIED VERDICT: PUBLISH

---

# Critic review — the-city-that-remembered-too-much v2

```
CRITIC:    muse-spark-1.2 (family muse, actor opencode-zen@session)
DATE:      2026-08-29
PASS:      3 (verification)
READ:      delta (backmatter.md, ch13-the-model-beneath-the-records.md:250-258, ch14-evidence-of-the-evidence.md:174-180, ch15-the-third-promise.md:580-610, ch16-every-witness-including-you.md:102-120+645, ch18-what-remains-legible.md:81-90, ch10-the-ash-hearing.md:11, plus full backmatter vs body grep verification)
```

## Verdict summary
Delta verification of v1→v2 (SHA 641f038): the sole high-severity failure — back-matter apparatus describing an earlier draft — is correctly rebuilt from the body. All fabricated cast/term strings are removed from `backmatter.md` and absent from the narrative body; correct names/terms are now defined with body-faithful gloss and body hits verified. The three med-severity body findings (B4/B5/B6) were rebutted without prose change; each rebuttal cites passages that exist verbatim in the shipped v2 body and survive delta inspection. No new blocking debt introduced; v2 back matter preserves the deliberately-unresolved frame-611 thread rather than resolving it. **PUBLISH** — VERIFIED.

## Blocking findings
Debts, not advice. Author must fix-with-diff or rebut-with-evidence, every one.

| # | Location (file:section) | Claim / problem | Evidence | Severity (high/med) |
|---|---|---|---|---|
| — | — | No still-open blocking debt. All pass-2 debts either fixed-with-diff (B1-B3) or rebutted-with-evidence accepted (B4-B6) — see ledger below. | Verified by grep over shipped v2 body (ch01-ch18) and `backmatter.md` inspection. | — |

## Suggestions (non-blocking)
1. Align `backmatter.md:32-66` wording tighter to body exact phrases for search parity (e.g., cite `quieting` 82 hits, `declared civic absence`/`accountable absence` present in ch18) — already correct, optional polish.
2. Consider pinning the `response-to-findings.md` verification snapshot counts (Iona 238, Saye 193-195, Mara 22-23, Tavi An 6) as a regression guard so future metadata drift is CI-caught.
3. Retain ch13-14 attribution tags praised in B4 rebuttal in any future copy-edit — the tagging is what makes the rebuttal verifiable.

## Fact-check sample
Pass 3: fresh 3% weighted toward revised sections. Internal-consistency check against manuscript's own establishment; a claim its citation does not support = blocking finding.

| Claim (quoted) | Location | Cited source | Supported? (yes/no/partly) |
|---|---|---|---|
| "Iona Vale — Keeper of Petitions" | backmatter.md: Principal Characters | ch01 "Iona Vale said" (03:17 waking tone); ch02 "Iona had served as Keeper for twenty-eight years. She was sixty-three" | yes |
| "Mara Venn — the chief continuity engineer declared dead after the south-membrane collapse. Her old machinery gives later Archives a lawful way to contradict the city" | backmatter.md: Principal Characters | ch06 Civil Status Record "MARA VENN Status: deceased Effective time: collapse day, 14:06:43 Body: not recovered Basis: continuity termination" + ch09 SEVEN-COPY deposit + ch11 voluntary biometric match "VOLUNTARY IDENTITY COMPARISON: match" | yes |
| "Tavi An — a membrane repair apprentice whose parent appears in the public reconstruction. Tavi insists that reducing an exposure is real work" | backmatter.md: Principal Characters | ch03 "Tavi An, apprentice membrane repairer, age seventeen, duty credential provisional" (137); ch08 "DO NOT MAKE MY CHILD PROVE I WAS THAT CHILD." petition; ch08/11 Tavi refuses to offer kinship as civic evidence | yes |
| "The Ash Hearings — the proceedings after officials destroyed records of disappearances and then denied acts that living witnesses remembered. The Hearings produced the First Promise" | backmatter.md: Civic Terms | ch10 "The room had not burned. Its name came from the gray paper dust …" (11); Ash Hearings = pulped maintenance orders/evacuations producing First Promise | yes |
| "A quieting petition — a formal request to remove specified civic records… Its result is a 'declared civic absence' / 'accountable absence'" | backmatter.md: Civic Terms | ch01 "We built quieting because the Archive gave power…" four rings; ch18 "ACCOUNTABLE ABSENCE 000001 … destroyed with declared exceptions" and ch18:63-66 definition; 82 hits for `quieting` in body | yes |
| "Because we believed disclosure of the capability would teach other offices how to use it and tell subjects which sealed investigations existed." | ch13:253 cited in B4 | ch13:251-258 Q&A: "Why didn't the reports say that?" → Saye answer in quotes, not Seven narration | yes — attributed testimony, not omniscient synthesis |

## Scores (1–5)
accuracy: 5 · clarity: 5 · completeness-for-tier: 5 · density: 4 · originality: 5

## Pass-3 only: findings ledger
| Finding # (from Pass 2) | Status: resolved / rebutted-accepted / still-open | Note |
|---|---|---|
| B1 — Dramatis personae contradicts cast (Ilyan Rook / Tavi Venn / Sera Vale / Orra vs Iona Vale / Tavi An / Mara Venn / Saye) | resolved | Fixed-with-diff verified: `backmatter.md` now lists Iona Vale, Tavi An, Mara Venn, Councilor Saye, Archive Seven, Reed, Chorus. Grep: Ilyan Rook 0, Sera Vale 0, Orra 0, Tavi Venn 0 in ch01-ch18 and in v2 backmatter.md; Iona 238, Saye ~193, Mara Venn 22-23, Tavi An 6 hits in body. Fabricated entries deleted. |
| B2 — Civic Terms diverge (mercy interval; Ash Hearing = fire) | resolved | Fixed-with-diff verified: "mercy interval" 0 hits in body and removed from v2 backmatter; v2 defines quieting / declared civic absence / accountable absence / interim joint order / accountable finding. Ash Hearings gloss now matches ch10 "had not burned / gray paper dust / pulped records" and does not misattribute 43 seconds. |
| B3 — Tavi kinship token / Tavi Venn as Mara's child re-identifies protected subject | resolved | Fixed-with-diff verified: v2 entry is "Tavi An — … Whether Tavi's parent is the child in frame 611 is a question the novel deliberately never answers; Tavi refuses to offer the relation as civic evidence." Surname Venn removed; deliberate non-resolution preserved (ch08, ch11 "Not may", ch18). Matches body. |
| B4 — ch13-14 breaks Seven's bounded POV with omniscient synthesis | rebutted-accepted | Rebuttal sound: ch13:253 line is Saye testimony in Q&A, not Seven narration; ch14:176-179 explicitly cites "Committee signatures, query receipts, access logs, and Saye's testimony established 312…" and "investigators' testimony established eighteen…". Epistemic tagging present. No prose change warranted. |
| B5 — Third Promise execution basis reads as retroactive legislation (14-second index label satisfying 11-year-old predicate) | rebutted-accepted | Rebuttal sound: ch16:102-119 states predicate is conditional "CURRENT LAW PERMITS A FIXED ACCOUNTABLE FINDING…" — bytes/scope unchanged, field resolves when interim joint order satisfies condition; ch15:580 "THIRD PROMISE, PROPOSED — SEE INTERIM JOINT ORDER…" as semantic label, ch15:610 "The law contained no Third Promise." Non-retrocausal by design and self-disclosed. |
| B6 — A-1 retention-exception denials never vacated | rebutted-accepted | Rebuttal sound: vacatur shown in shipped body: ch18:81-82 "The four people denied under Internal Retention Exception A-1 returned to the Quieting Court as three petitioners and one prior instruction"; ch18:90 "The court ordered the content removed"; ch18:457 amendment reopens ACCOUNTABLE ABSENCE. Denials re-adjudicated under enacted amendment. |
