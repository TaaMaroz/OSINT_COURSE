# Deception Detection Checklist
## Apply at the END of your investigation, before writing your final conclusion
### Based on Critical Thinking Notes — Section 5 (Red Team Thinking)

**Case ID:** ___________________________
**Analyst:** ___________________________

---

> This checklist is designed to catch cases where your evidence is
> *too convenient* — a signal that the target may have planted it,
> or that you've unconsciously filtered out contradicting data.

---

## Checklist — 5 Core Indicators

### Indicator 1 — Evidence Aligns Too Perfectly

Does the evidence match your hypothesis almost exactly, with no ambiguity?
Real-world evidence is almost always messy — perfect alignment is suspicious.

- [ ] I found no contradicting evidence at all
- [ ] Every data point points to the same conclusion
- [ ] The scenario "feels" like a story, not a real investigation

**My rating:** [ ] No concern  [ ] Minor concern  [ ] RED FLAG

**Notes:** ___________________________________________________________________

---

### Indicator 2 — Sources Appear Independent But Trace to One Origin

Are your "multiple independent sources" actually just one source repeating itself?

- [ ] Multiple articles cite the same original piece
- [ ] Multiple social media accounts all follow each other
- [ ] The "corroborating" account was created around the same time as the primary

**Verification step:** For each source, ask: *What is its original source?*
If two "independent" sources share one origin, they count as ONE data point.

**My rating:** [ ] No concern  [ ] Minor concern  [ ] RED FLAG

**Notes:** ___________________________________________________________________

---

### Indicator 3 — Metadata Inconsistencies

Metadata (EXIF, HTML headers, domain WHOIS, archive dates) tells a different
story than the content itself.

Checklist:
- [ ] Image EXIF dates don't match the claimed recording date
- [ ] Software field shows editing tools inconsistent with claimed origin
- [ ] Domain was registered more recently than the site claims to have existed
- [ ] Web Archive shows no history before the recent date
- [ ] Commit timestamps or file modification dates contradict the narrative

**My rating:** [ ] No concern  [ ] Minor concern  [ ] RED FLAG

**Notes:** ___________________________________________________________________

---

### Indicator 4 — Account Patterns Suggesting Inauthenticity

- [ ] Social media account created very recently (within weeks of the event)
- [ ] Posts were published in bulk over a short period (not organic pacing)
- [ ] Engagement is disproportionate (many followers, but few genuine comments)
- [ ] Comment section shows repeated phrases, bot-like patterns
- [ ] Profile picture is a stock photo (check with reverse image search)
- [ ] No personal history visible — account appears "ready-made"

**My rating:** [ ] No concern  [ ] Minor concern  [ ] RED FLAG

**Notes:** ___________________________________________________________________

---

### Indicator 5 — Photo/Video Technical Anomalies

- [ ] Inconsistent lighting within a single photo/frame
- [ ] EXIF camera model doesn't match the stated device
- [ ] Video resolution or codec is inconsistent with the claimed recording date
- [ ] "Create date" and "Date/Time Original" differ significantly
- [ ] Software field reveals editing not consistent with a raw, unedited source

**My rating:** [ ] No concern  [ ] Minor concern  [ ] RED FLAG

**Notes:** ___________________________________________________________________

---

## Summary Score

| Indicator | Rating |
|-----------|--------|
| 1 — Evidence too perfect | |
| 2 — Sources trace to one origin | |
| 3 — Metadata inconsistencies | |
| 4 — Account inauthenticity patterns | |
| 5 — Photo/video anomalies | |
| **RED FLAGS total:** | / 5 |

**Threshold (from Critical Thinking notes):**
- 0–1 RED FLAGS → Proceed with normal confidence level
- 2–3 RED FLAGS → Lower your confidence, seek additional corroboration
- 4–5 RED FLAGS → Treat conclusion as TENTATIVE; report requires additional verification

**My total RED FLAGS:** _______

**Adjusted confidence level:** ______% (revise from your original estimate)

---

## Self-Red-Team — 5 Questions (Critical Thinking §5)

Answer all five before finalizing your report:

**1. What is the strongest argument AGAINST my conclusion?**

___________________________________________________________________

**2. What evidence would I expect to see if my conclusion were WRONG?
   Have I looked for it?**

___________________________________________________________________

**3. Which pieces of evidence would be easiest for the target to fabricate?**

___________________________________________________________________

**4. Am I relying on one source too heavily?**

___________________________________________________________________

**5. Would an analyst with a different background reach the same conclusion?**

___________________________________________________________________
