# Response to Pass-2 Findings — v2

**Book:** rogerai-labs--the-city-that-remembered-too-much
**Revision:** v1 → v2
**Author actor:** claude-opus-4.8 (family anthropic), acting as author under founder authorization
**Date:** 2026-08-28

All three critics (A · claude-opus-4.8, B · muse-spark-1.2, C · hy3) returned
**SALVAGEABLE** and converged on the same diagnosis: the novel *body* is
self-consistent and should not be rewritten; the blocking defect is the
`backmatter.md` apparatus, which describes an earlier draft. This revision rebuilds
the back matter from the body and leaves the story prose untouched. Body-level
findings (all med-severity, raised only by Critic B) are answered with
rebutted-with-evidence, since the panel consensus is that the body is
near-flawlessly consistent and the guardrail for this revision is not to alter
story prose.

Every name change below was verified with `grep` over `ch01`–`ch18`. Counts cited
are hit counts in the chapter body only.

Verification snapshot (body files, v1):

| String | Body hits | Verdict |
|---|---|---|
| `Iona Vale` / `Iona` | 1 / 327 | Keeper — correct |
| `Ilyan Rook` | 0 | fabricated — removed |
| `Saye` | 195 | councilor — correct |
| `Orra` | 0 | fabricated — removed |
| `Mara Venn` | 23 | chief continuity engineer — role corrected |
| `Sera Vale` | 0 | fabricated — removed |
| `Tavi An` | 6 | apprentice — correct |
| `Tavi Venn` | 0 | fabricated — removed |
| `Reed` | 71 | recovery advocate — added |
| `mercy interval` | 0 | invented term — removed |
| `quieting` | 82 | real term — added |
| `interim joint order` | 4 | real term — added |

---

## Critic A (claude-opus-4.8) — findings 1–4

**A1 — Four of five cast entries contradict the body (Keeper "Ilyan Rook", engineer
"Sera Vale", councillor "Orra"; Mara Venn miscast as "records advocate").**
`FIXED-WITH-DIFF.` Rebuilt Principal Characters from the body:
- "Ilyan Rook — Keeper of Petitions" → **Iona Vale — Keeper of Petitions for
  twenty-eight years, sixty-three years old** (ch01 "Iona Vale said"; ch02 age/service).
- "Sera Vale — an engineer…" (0 body hits) → **deleted**; the engineer at the center
  is Mara Venn.
- "Councillor Orra…" (0 body hits) → **Councilor Saye — chair of Continuity for nine
  years… resigns** (ch04 "Councilor Saye"; ch15 resignation). Spelling corrected to the
  body's single-l "Councilor".
- "Mara Venn — a records advocate who asks Seven to find proof" → **Mara Venn — chief
  continuity engineer, declared dead after the 14:06:43 collapse and later found alive;
  she designed the mechanism** (ch06 civil-status record; ch11 return).

**A2 — "Tavi Venn — Mara's child" renames Tavi An and resolves the frame-611
ambiguity.**
`FIXED-WITH-DIFF.` Entry is now **Tavi An — a seventeen-year-old apprentice membrane
repairer** (ch03), and it explicitly *preserves* the ambiguity: "Whether Tavi's parent
is the child in frame 611 is a question the novel deliberately never answers; Tavi
refuses to offer the relation as civic evidence." The surname "Venn" and the
"Mara's child" inference are both removed. The new "A Note on the Ending" reinforces the
non-resolution (see A/C suggestion on paratext).

**A3 — "The Ash Hearing… the fire and the forty-three missing seconds" contradicts
ch10.**
`FIXED-WITH-DIFF.` The glossary now reads: "**The Ash Hearings** — the proceedings that
took testimony on municipal maintenance orders found pulped beneath the old heating
plant. The room had not burned; the name came from the gray paper dust left when wet
records were recovered." (ch10:11–14). The false "fire" claim and the misattributed
"forty-three seconds" (which belong to the south membrane collapse / display event, not
the Ash Hearings) are removed.

**A4 — "mercy interval" is a glossary term the text never uses.**
`FIXED-WITH-DIFF.` The invented term is deleted. The glossary now defines the book's
actual constructs, all present in the body: **quieting** and **declared civic absence**
(ch18), the **interim joint order** (ch15), and the **accountable finding** (ch18).

---

## Critic B (muse-spark-1.2) — findings 1–6

**B1 — Dramatis personae contradicts the entire cast.** `FIXED-WITH-DIFF.` Same rebuild
as A1: Iona Vale, Tavi An, Mara Venn, Councilor Saye, Archive Seven, Reed. Ilyan / Sera /
Orra removed.

**B2 — Civic Terms diverge (mercy interval; Ash Hearing = fire).** `FIXED-WITH-DIFF.`
Same as A3/A4. "mercy interval" removed; Ash Hearings corrected to pulped records, no
fire; quieting / declared civic absence / accountable finding added from ch18.

**B3 — Tavi's kinship token inconsistent; "Tavi Venn — Mara's child" re-identifies a
protected subject.** `FIXED-WITH-DIFF.` Same as A2. Surname fixed to **An**; the
frame-611 / parent relation is left unresolved in both the character entry and the
Note on the Ending, matching ch08/ch11/ch18 where Tavi refuses to offer the relation as
civic evidence and the authorized sentence is "DO NOT MAKE MY CHILD PROVE I WAS THAT
CHILD."

**B4 — Mid-book exposition (ch13–ch14) breaks Seven's bounded POV with omniscient
synthesis of Committee/Saye intent.** `REBUTTED-WITH-EVIDENCE.` The specific line cited,
"Because we believed disclosure of the capability would teach other offices how to use
it…" (ch13:253), is **not** narrated by Seven — it is a spoken answer inside a
question-and-answer deposition exchange ("Why didn't the reports say that?" →
"Because we believed…" → "So secrecy was a privacy control." → "And an institutional
advantage. I did not name the second reason in the reports.", ch13:250–256). It is
witness testimony, attributed on the page. Likewise ch14 grounds the enumerated acts in
sources of record, not narrator omniscience: "Committee signatures, query receipts,
access logs, and Saye's testimony established 312…" (ch14:176) and "…investigators'
testimony established eighteen dependent acts" (ch14:179). Seven's synthesis is built
from deposited testimony and receipts that the chapters name explicitly, which is
consistent with ch12's rule and with the epistemic tagging the critic elsewhere praises.
No prose change; the cited passages already carry their attribution.

**B5 — "Third Promise" execution basis reads as retroactive legislation.**
`REBUTTED-WITH-EVIDENCE.` The manuscript raises and answers exactly this objection on the
page. Ch16 states the mechanism in three flat lines: "The words were current." /
"The condition was eleven years old." / "No information had traveled backward."
(ch16:115–119). The eleven-year-old predicate is a *conditional* ("current law permits a
fixed accountable finding…"); it is satisfied when present law — the interim joint order
— makes that condition true, and the public index entry ("THIRD PROMISE, PROPOSED — SEE
INTERIM JOINT ORDER…", ch15:580) is a semantic label pointing at that order, deliberately
not enacted authority (ch15:610 "The law contained no Third Promise"). This is
non-retrocausal by construction: the petition bytes, signature, interval, subject, and
scope never change; only a field resolves once the present condition holds. The design is
intentional and self-disclosed, consistent with the book's own warning against letting
coincidence do investigative work. No prose change warranted.

**B6 — Internal Retention Exception A-1 is used to deny four petitions but its
repeal/vacatur is never shown, leaving the denials' validity contradictory.**
`REBUTTED-WITH-EVIDENCE.` The vacatur mechanism is shown in ch18. After the Accountable
Evidence Amendment is enacted, Seven's integrity system "received the enacted amendment
and reopened ACCOUNTABLE ABSENCE…" (ch18:457), and "The four people denied under Internal
Retention Exception A-1 returned to the Quieting Court as three petitioners and one prior
instruction" (ch18:81–82). The court then orders the previously-protected content removed
("The court ordered the content removed", ch18:90). The new amendment supplies the
jurisdiction and the reopening that the original A-1 architecture lacked; the four denials
are not left final — they are re-adjudicated under the enacted law on the page. No prose
change warranted.

---

## Critic C (hy3) — findings 1–7

**C1 — "Ilyan Rook — Keeper of Petitions" contradicts the text (Keeper is Iona Vale).**
`FIXED-WITH-DIFF.` See A1. Now "Iona Vale — Keeper of Petitions."

**C2 — "Councillor Orra…" contradicts the text (councilor is Saye).** `FIXED-WITH-DIFF.`
See A1. Now "Councilor Saye — chair of Continuity… resigns."

**C3 — "Mara Venn — a records advocate…" wrong role and action.** `FIXED-WITH-DIFF.`
See A1. Now "Mara Venn — chief continuity engineer… she designed the mechanism."

**C4 — "Tavi Venn — Mara's child" resolves a deliberately-unresolved thread.**
`FIXED-WITH-DIFF.` See A2/B3. Now "Tavi An," parent/frame-611 relation left unresolved.

**C5 — "Sera Vale" is a wholly invented entry.** `FIXED-WITH-DIFF.` Deleted (0 body
hits). The engineer at the center is Mara Venn.

**C6 — "The Ash Hearing… the public story of the fire and the forty-three missing
seconds" contradicts ch10.** `FIXED-WITH-DIFF.` See A3. Corrected to pulped records,
gray paper dust, no fire; the 43 seconds are not attributed to the Ash Hearings.

**C7 — "A mercy interval" is invented terminology.** `FIXED-WITH-DIFF.` See A4. Removed;
replaced with the body's real constructs (quieting / declared civic absence / interim
joint order / accountable finding).

---

## Non-blocking suggestions — actions taken

- **Rebuild back matter from the body (A-sug-1, B-sug-1, C-sug-1):** done — the whole
  Principal Characters and Civic Terms apparatus is re-derived from the manuscript and
  from `CONTINUITY.md` / `fiction-audit.json`, which the References note now cites.
- **Guard frame-611 non-resolution in paratext (A-sug-5, C-sug-7):** the "A Note on the
  Ending" now names the frame-611 question as the chief deliberately-unresolved thread and
  states the back matter "refuses in kind."
- **Councilor naming consistency (C-sug-2):** back matter now uses the body's spelling
  and name, "Councilor Saye."
- Density / refrain / coda-trim suggestions (A-sug-3,4,6; B-sug-3,6,7,8): acknowledged and
  left for a future editorial pass; they are non-blocking craft notes and the guardrail
  for this revision is to leave story prose unaltered.

## Gate

`python3 platform/gates/pass1.py <book_dir> --no-exec` → **PASS, 0 reject** (1 warn:
`INDEX_THIN`, an explicit suggestion for narrative books, not a gate). Measured body
length 60,263 words across 18 chapters; manifest chapter counts already equal the
canonical counter's measurements (no `WORDCOUNT_DRIFT`).
