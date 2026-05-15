# wfh-remote-job-finder
2026 WFH/remote job search automation — 9 boards, ATS operators, scam detection, weekly rhythm

![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat&labelColor=555&logo=python)
![Shell](https://img.shields.io/badge/Shell-Bash-4EAA25?style=flat&labelColor=555)
![LinkedIn](https://img.shields.io/badge/LinkedIn-Jobs-0077B5?style=flat&labelColor=555)
![Boards](https://img.shields.io/badge/Job_Boards-9-orange?style=flat&labelColor=555)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat&labelColor=555)

[Concepts](#-concepts) · [How It Works](#️-how-it-works) · [Install](#-install) · [Boards](#-job-boards) · [Tips](#-tips-and-tricks-10) · [Startups](#️-startups--businesses)

---

## 🧠 CONCEPTS

| Feature | Location | Description |
|---------|----------|-------------|
| [**remote-job-hunter**](remote-job-hunter) | `~/.claude/bin/remote-job-hunter` | CLI: daily sweep across 9 job boards + ATS operators |
| [**ATS Operators**](remote-job-hunter) | `--ats` flag | Google site: operators for Lever, Greenhouse, Ashby, Workday |
| [**Scam Detector**](remote-job-hunter) | `--check URL` | 22-point scam score: red flags, company verify, salary sanity |
| [**Job Tracker**](remote-job-hunter) | `--export` | 11-column Excel tracker: status, applied date, follow-up |
| [**Weekly Rhythm**](remote-job-hunter) | `--weekly-plan` | Mon–Sun action plan: apply, follow-up, network, research days |
| [**Quality Filter**](remote-job-hunter) | `--quality` | Filters: remote-first only, 48h freshness, no-spray-and-pray |

### 🔥 Hot

| Feature | Location | Description |
|---------|----------|-------------|
| [**ATS Direct Search**](remote-job-hunter) | `--ats --role "PPC"` | Bypass aggregators — find jobs on company ATS before they're listed |
| [**Scam Score 0–22**](remote-job-hunter) | `--check URL` | 8 red flags scored: vague pay, no company info, urgency pressure |
| [**5–12 tailored apps/day**](remote-job-hunter) | Target | Quality over quantity — this system's core metric |

---

## ⚙️ HOW IT WORKS

```
remote-job-hunter --daily --role "Google Ads Specialist"
         ↓
Sweeps 9 boards simultaneously:
  LinkedIn · RemoteOK · Remotive · Wellfound
  WeWorkRemotely · Himalayas · Indeed · Naukri · FlexJobs
         ↓
ATS operators: site:lever.co "google ads" "remote"
         ↓
Scam filter removes low-quality listings
         ↓
Top 5–12 jobs → Excel tracker + cover letter queue
         ↓
Apply within 48h of posting (before ATS buries listing)
```

---

## 🚀 INSTALL

```bash
git clone https://github.com/hmzainjamil/wfh-remote-job-finder
cd wfh-remote-job-finder
cp remote-job-hunter ~/.claude/bin/
chmod +x ~/.claude/bin/remote-job-hunter
pip install requests openpyxl beautifulsoup4
```

---

## 📋 JOB BOARDS

| Board | Strength | Best Role Types |
|---|---|---|
| [LinkedIn](https://linkedin.com/jobs) | Volume + network | Any |
| [RemoteOK](https://remoteok.com) | Pure remote | Tech, marketing, design |
| [Remotive](https://remotive.com) | Curated remote | Tech, ops, customer success |
| [Wellfound](https://wellfound.com) | Startups | Tech, growth, product |
| [WeWorkRemotely](https://weworkremotely.com) | Premium remote | Dev, design, marketing |
| [Himalayas](https://himalayas.app) | Remote-first | All roles |
| [Indeed](https://indeed.com) | Volume | Any |
| [Naukri](https://naukri.com) | South Asia | Any |
| [FlexJobs](https://flexjobs.com) | Vetted remote | Any |

---

## 💡 TIPS AND TRICKS (10)

[search](#tips-search) · [ats](#tips-ats) · [scam](#tips-scam) · [apply](#tips-apply)

<a id="tips-search"></a>■ **Search Strategy (3)**

| Tip | Source |
|-----|--------|
| Apply within 48h — after 48h, ATS ranking drops applicants to page 2 | [HMZ](https://github.com/hmzainjamil) |
| Remote-first > remote-friendly — "remote friendly" means office-first with occasional WFH | [DigiMinds](https://github.com/hmzainjamil) |
| Search by skill not title: "Google Ads" beats "PPC Manager" — more results, less competition | [HMZ](https://github.com/hmzainjamil) |

<a id="tips-ats"></a>■ **ATS Direct (3)**

| Tip | Source |
|-----|--------|
| `site:lever.co "google ads" "remote"` — finds jobs before they hit aggregators | [HMZ](https://github.com/hmzainjamil) |
| `site:greenhouse.io "ppc" "remote"` — Greenhouse used by 5,000+ companies | [DigiMinds](https://github.com/hmzainjamil) |
| Ashby ATS growing fast among funded startups: `site:ashbyhq.com "paid media"` | [HMZ](https://github.com/hmzainjamil) |

<a id="tips-scam"></a>■ **Scam Detection (2)**

| Tip | Source |
|-----|--------|
| Red flag #1: vague salary "competitive" with no range = low pay or scam | [HMZ](https://github.com/hmzainjamil) |
| Verify company on LinkedIn before applying — no company page = likely fake | [HMZ](https://github.com/hmzainjamil) |

<a id="tips-apply"></a>■ **Application (2)**

| Tip | Source |
|-----|--------|
| 5–12 tailored apps > 50 spray-and-pray — ATS scores relevance, personalized wins | [DigiMinds](https://github.com/hmzainjamil) |
| Follow up at day 5 if no response — 35% of offers come from follow-up, not initial apply | [HMZ](https://github.com/hmzainjamil) |

---

## ☠️ STARTUPS / BUSINESSES

| This Repo / Feature | Replaced |
|-|-|
| **9-board daily sweep** | [Jobscan](https://jobscan.co), [Huntr](https://huntr.co), [Teal](https://tealhq.com) |
| **ATS direct search** | [LinkedIn Premium](https://linkedin.com/premium), [Indeed Resume](https://indeed.com) paid features |
| **Scam detector** | Manual Google research — 22-point automated check |
| **Job tracker Excel** | [Notion job tracker](https://notion.so), [Trello boards](https://trello.com) — local, offline |

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hmzainjamil/wfh-remote-job-finder&type=Date)](https://star-history.com/#hmzainjamil/wfh-remote-job-finder&Date)

---

<div align="center">
Built by <a href="https://github.com/hmzainjamil">HMZ</a> · Remote job search automation for PPC/digital marketing specialists
</div>
