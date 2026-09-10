# ACH Matrix — Challenge #1: The Disappeared Developer
## Analysis of Competing Hypotheses (ACH)
### Based on: Critical Thinking Notes, Section 3

---

## Step 1 — Define Your Hypotheses

| Code | Hypothesis |
|------|-----------|
| H1 | Developer was suppressed/silenced by the company (insider threat by employer) |
| H2 | Developer fabricated the story (disgruntled employee seeking attention) |
| H3 | A real external threat actor targeted the developer independently |
| H4 | Developer staged their own disappearance for personal reasons |

> Add a 5th hypothesis if your evidence suggests one not listed above.

---

## Step 2 — List All Significant Evidence

| # | Evidence Item | Source File |
|---|--------------|-------------|
| E1 | Admin portal publicly reachable (HTTP 200) | sublist3r_clearpath.txt |
| E2 | Admin subdomain has a separate TLS certificate issued 2026-06-01 | theharvester_clearpath.txt |
| E3 | Target email found in 3 breach databases | h8mail_results.txt |
| E4 | Password stored as MD5 (weak hashing) | hash_sample.txt |
| E5 | Reddit post about "weird auth logs" deleted 3 days after posting | blackbird_devk0re.txt |
| E6 | Commit pushed with work email "DO NOT PUSH TO PUBLIC" message | maigret_devk0re_report.txt |
| E7 | 14-month gap in Web Archive snapshots of admin portal | carbon14_admin_portal.txt |
| E8 | Target accounts went silent simultaneously ~2026-08-18 | blackbird_devk0re.txt |
| E9 | Target has no personal social media (no Facebook/Instagram/Twitter) | holehe_output.txt |
| E10 | Full name, employer, location confirmed via conference breach + LinkedIn scrape | h8mail_results.txt |

---

## Step 3 — Fill in the Matrix

Mark each cell: **C** (consistent with H), **I** (inconsistent with H), **N/A** (not relevant)

| Evidence | H1: Employer suppression | H2: Developer fabricated | H3: External threat | H4: Staged disappearance |
|----------|:---:|:---:|:---:|:---:|
| E1 — Admin portal publicly accessible | | | | |
| E2 — Separate cert for admin (2026-06) | | | | |
| E3 — Email in 3 breach databases | | | | |
| E4 — MD5 password hashing (weak security) | | | | |
| E5 — Deleted Reddit post | | | | |
| E6 — Accidental commit with work email | | | | |
| E7 — 14-month Web Archive gap | | | | |
| E8 — All accounts silent since Aug 18 | | | | |
| E9 — No personal social media presence | | | | |
| E10 — Real identity confirmed externally | | | | |
| **Inconsistency Count (I)** | | | | |

---

## Step 4 — Sensitivity Check

> Which single piece of evidence is most likely to be wrong or fabricated?
> If you remove it, does your conclusion change?

My most fragile evidence item: _______________________________________________

If this evidence is wrong, my conclusion changes to: _________________________

---

## Step 5 — Preliminary Conclusion

**Most supported hypothesis (fewest I's):** ___________________________________

**Confidence level (0–100%):** ______%

**Why:** ___________________________________________________________________

---

## Step 6 — Key Assumptions Check (Critical Thinking §4.1)

| Assumption | What if this is wrong? | Rating (Certain / Moderate / Low / Unsupported) |
|------------|----------------------|------------------------------------------------|
| 'devk0re' username is exclusively used by one person | | |
| clearpath-tech.io is the legitimate company domain | | |
| The Reddit post deletion was by the target, not by Reddit admins | | |
| The 14-month archive gap is meaningful, not a crawling artifact | | |
