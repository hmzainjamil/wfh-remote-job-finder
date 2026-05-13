# WFH / REMOTE JOB FINDER — 2026 Edition (always-on)

**Auto-activates on:** "remote job" / "wfh job" / "work from home" / "find remote work" / "job search" / "remote hiring" / "job board india" / "find job india" / "remote apply" / "ats search" / "job tracker"

---

## QUICK COMMANDS

```bash
python3 ~/.claude/bin/remote-job-hunter --daily --role "customer support"
python3 ~/.claude/bin/remote-job-hunter --ats --role "data analyst"
python3 ~/.claude/bin/remote-job-hunter --weekly-plan
python3 ~/.claude/bin/remote-job-hunter --check "https://job-url.com"
python3 ~/.claude/bin/remote-job-hunter --export
python3 ~/.claude/bin/remote-job-hunter --boards-list --role "marketing"
```

---

## 9 PLATFORMS

| Platform | Type | India-friendly |
|---|---|---|
| LinkedIn Jobs | General + remote filter | ✅ |
| We Work Remotely | Remote-first board | ✅ |
| Remote OK | Global remote | ✅ |
| Remotive | Remote-first | ✅ |
| Wellfound | Startup hiring | ✅ |
| Himalayas | Remote-first | ✅ |
| FlexJobs | Curated, scam-reduced | ✅ |
| Naukri | India-specific WFH | ✅ |
| Indeed | WFH filter + India | ✅ |

---

## ATS GOOGLE OPERATORS

```
site:lever.co "Customer Support" "Remote"
site:lever.co "Data Analyst" "Remote" "India"
site:greenhouse.io "Marketing" "Remote"
site:greenhouse.io "Operations" "Remote" "India"
site:myworkdayjobs.com "Remote" "India"
site:jobs.ashbyhq.com "operations" "remote"
site:jobs.ashbyhq.com "customer success" "remote" "india"
```
Add `after:2026-04-01` for fresh results only.

---

## SCAM DETECTION — 8-FLAG AUTO-SCORE

| Flag | Weight |
|---|---|
| Pay unrealistically high for simple work | +3 |
| Weak/missing company website | +3 |
| Recruiter avoids official email domain | +3 |
| Asks for money / deposit / training fee | +5 |
| Vague description copied across titles | +2 |
| Process unusually rushed | +2 |
| Contact via Telegram/WhatsApp only | +2 |
| No LinkedIn company page | +2 |

Score 0–2: Apply · 3–5: Verify · 6+: Skip

---

## RESUME TAILORING (4 zones per role)
1. Headline → match job title family
2. Top summary → mirror top 3 role keywords
3. Tools → add any missing tools from JD
4. Top 2 bullets → reframe to primary responsibility

Remote-readiness: Slack, Zoom, Notion, Jira, async communication, independent execution.

---

## WEEKLY RHYTHM

| Day | Focus | Actions |
|---|---|---|
| Monday | Fresh roles | Check alerts → apply newest → update tracker |
| Tuesday | Company watchlist | Visit 10-15 career pages |
| Wednesday | LinkedIn discovery | Feed posts, founder/recruiter posts |
| Thursday | Resume optimization | 1 resume version + 1 cover template |
| Friday | Follow-up | Reconnect with recruiters |
| Saturday | Skill proof | Portfolio / certs |
| Sunday | Review | Measure + set priorities |

Target: 5-12 quality apps/day · Apply within 48h · Never spray 100 random apps

---

## MAE INTEGRATION

```bash
mae run "Remote job search: customer support for India-based candidate. Search LinkedIn, RemoteOK, Remotive, Wellfound. Filter: remote, India-friendly, posted last 48h. Score scam signals. Export top 10."
mae run "Tailor resume for [ROLE]. Match headline, top 3 keywords, remote tools, 2 bullets. Input: [JD]."
```

---

## DigiMinds Services

| Package | Price |
|---|---|
| Job Search Audit | $150 |
| Resume Makeover | $200 |
| Full Search System | $400 |
| Monthly Managed Search | $800/mo |
