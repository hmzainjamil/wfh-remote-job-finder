<div align="center">

# wfh-remote-job-finder

![Platform](https://img.shields.io/badge/platform-multi--board-blue?style=flat)
![Boards](https://img.shields.io/badge/boards-9%2B-green?style=flat)
![India](https://img.shields.io/badge/India-friendly-orange?style=flat)
![MAE](https://img.shields.io/badge/MAE-integrated-purple?style=flat)
![License](https://img.shields.io/badge/license-MIT-lightgrey?style=flat)

**Complete 2026 WFH/remote job search automation system.**
Multi-board scraping · ATS operator blasts · Scam detection · Resume tailoring · Weekly rhythm enforcement.

*Based on the WFH/Remote Job Finding Guide by Qadir @kaamkibaatein_*

</div>

---

## What this does

| Feature | Detail |
|---|---|
| **9 job boards** | LinkedIn, RemoteOK, Remotive, Wellfound, WWR, Himalayas, FlexJobs, Indeed, Naukri |
| **ATS operator blasts** | Google site: operators for Lever, Greenhouse, Ashby, Workday — finds hidden roles |
| **Scam detection** | 8-flag scoring system — APPLY / VERIFY / SKIP verdict on any listing |
| **Resume tailoring** | Edit 4 zones per role: headline, summary, tools, top 2 bullets |
| **Weekly rhythm** | Day-by-day action plan, 5-12 quality apps/day target |
| **MAE integration** | Full MAE orchestration via `mae run` commands |

## 🔥 Hot — Quick Start

```bash
# Install
git clone https://github.com/hmzainjamil/wfh-remote-job-finder ~/installed-repos/wfh-remote-job-finder
cp ~/installed-repos/wfh-remote-job-finder/remote-job-hunter ~/.claude/bin/
chmod +x ~/.claude/bin/remote-job-hunter

# Daily sweep — all 9 boards + ATS operators
python3 ~/.claude/bin/remote-job-hunter --daily --role "customer support"

# ATS Google operators (finds hidden roles)
python3 ~/.claude/bin/remote-job-hunter --ats --role "data analyst"

# Weekly plan
python3 ~/.claude/bin/remote-job-hunter --weekly-plan

# Scam check any listing
python3 ~/.claude/bin/remote-job-hunter --check "https://job-url.com"

# Export blank tracker to Excel
python3 ~/.claude/bin/remote-job-hunter --export
```

## ATS Google Operator Patterns

```
site:lever.co "Customer Support" "Remote"
site:lever.co "Data Analyst" "Remote" "India"
site:greenhouse.io "Marketing" "Remote"
site:myworkdayjobs.com "Remote" "India"
site:jobs.ashbyhq.com "operations" "remote" "india"
```

Paste these directly into Google → filter by date → apply on official company page.

## Scam Detection (auto-score)

| Red Flag | Score |
|---|---|
| Pay unrealistically high for simple work | +3 |
| Weak/missing company website | +3 |
| Recruiter avoids official email domain | +3 |
| Asks for money/deposit/training fee | +5 |
| Vague copied description | +2 |
| Rushed/too easy process | +2 |
| Telegram/WhatsApp contact only | +2 |
| No LinkedIn company page | +2 |

`0-2` → Apply · `3-5` → Verify first · `6+` → Skip

## Weekly Rhythm

| Day | Focus | Actions |
|---|---|---|
| Monday | Fresh roles | Check alerts → apply newest → update tracker |
| Tuesday | Company watchlist | Visit 10-15 career pages |
| Wednesday | LinkedIn discovery | Feed posts, founder/recruiter posts |
| Thursday | Resume optimization | 1 resume version + 1 cover template |
| Friday | Follow-up | Reconnect with recruiters |
| Saturday | Skill proof | Portfolio / certs |
| Sunday | Review | Measure + set next-week priorities |

## ■ tip

> Apply within **24–48 hours** of posting. After 72h, response rate drops 40%.
> Quality target: **5–12 tailored apps/day** — NOT 100 spray-and-pray applications.

## DigiMinds Service Tiers

| Package | Price |
|---|---|
| Job Search Audit | $150 |
| Resume Makeover | $200 |
| Full Search System | $400 |
| Monthly Managed Search | $800/mo |

---

*Part of [hmzainjamil/claude-ai-system](https://github.com/hmzainjamil/claude-ai-system) · Based on guide by [@kaamkibaatein_](https://twitter.com/kaamkibaatein_)*
