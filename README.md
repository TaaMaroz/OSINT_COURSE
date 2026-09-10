# 🔍 Challenge #1 — The Disappeared Developer
## Brief

---

### Scenario

A cybersecurity non-profit called **ClearPath Tech** (`clearpath-tech.io`) has
reported a disturbing situation to your team. One of their senior developers — who
went by the online handle **`devk0re`** — suddenly vanished three weeks ago.

Before disappearing, they emailed the board saying they were "being watched" and
had uncovered evidence of internal fraud. Their personal laptop was wiped, and the
company's incident log showed a login from an unfamiliar IP the night before they
went silent.

Your team has been hired to conduct a **passive OSINT investigation**.

---

### Intelligence Requirements

1. What platforms is `devk0re` registered on?
2. What email address(es) are linked to this identity?
3. Does the domain `clearpath-tech.io` expose subdomains or sensitive files?
4. Does breach data connect any recovered email to a known leak?
5. What is the most probable explanation for the disappearance?

---

### Flags to Capture 🚩

| Flag | Question |
|------|----------|
| **FLAG-1** | How many platforms is `devk0re` confirmed active on? (must use ≥2 tools) |
| **FLAG-2** | One email address linked to this identity |
| **FLAG-3** | A subdomain of `clearpath-tech.io` that exposes a login/admin portal |
| **FLAG-4** | The hash algorithm type of the password found in breach data |
| **FLAG-5** | Your ACH conclusion — which hypothesis has the fewest inconsistencies? |

---

### Evidence Files Provided

The following files simulate real tool outputs you would get by running the tools
yourself. Analyze each file carefully — the flags are embedded in the data.

```
evidence/
├── sherlock_devk0re.csv         ← Sherlock username scan output
├── blackbird_devk0re.txt        ← Blackbird username scan output
├── maigret_devk0re_report.txt   ← Maigret scan summary
├── theharvester_clearpath.txt   ← TheHarvester domain output
├── sublist3r_clearpath.txt      ← Sublist3r subdomain list
├── carbon14_admin_portal.txt    ← Carbon14 page-age output
├── h8mail_results.txt           ← H8Mail breach query output
├── hash_sample.txt              ← Hash string recovered from breach data
├── holehe_output.txt            ← Holehe email-to-service mapping
└── ddgs_results.csv             ← DDGS automated search results
```

---

### Deliverable

Submit a **1–2 page investigation report** containing:
1. Timeline of findings (source + timestamp for each)
2. Completed ACH matrix (template in `/templates/ach_matrix_template.md`)
3. Your confidence level on the conclusion (0–100%)
4. One assumption that, if wrong, would invalidate your conclusion

### Rules
- Passive only — no active scanning, no login attempts
- Every flag must cite its source file
- Complete the ACH matrix **before** writing FLAG-5
