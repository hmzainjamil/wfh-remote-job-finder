# WFH Remote Job Finder

A Python helper and companion guidance files for planning remote job searches. The script builds job-board URLs and ATS search operators, prints a weekly plan, asks the user to score listing risk flags, and can export a blank Excel tracker. It does not scrape listings, verify jobs, submit applications, tailor resumes, or create a company watchlist.

## Repository map

| Path | Purpose |
|---|---|
| `remote-job-hunter` | Standalone Python CLI for URL/operator generation, manual scam-flag scoring, weekly-plan output, and blank tracker export |
| `SKILL.md` | Search prompts, board list, ATS examples, and general job-search guidance |
| `remote-job-hunter-agent.md` | Agent behavior proposal; includes capabilities and service claims beyond the checked-in CLI |
| `README.md` | Repository guide |

The guidance files are not wired into a Claude Code installation by this repository. The agent document describes resume tailoring and company watchlists, but those features are not implemented in the tracked script.

## Requirements

- Python 3
- The standard library for URL/operator generation and other CLI modes
- Optional `openpyxl` for `--export`
- Optional local executable at `~/.claude/bin/llm-burst` for the AI analysis portion of `--daily`

No dependency manifest or automated tests are included. The script creates `~/Downloads/job-search` when it starts.

## Use

Run from the repository root:

```bash
python3 remote-job-hunter --boards-list --role "marketing" --location "Canada"
python3 remote-job-hunter --ats --role "data analyst"
python3 remote-job-hunter --weekly-plan
python3 remote-job-hunter --check "https://example.com/job"
python3 remote-job-hunter --export
python3 remote-job-hunter --daily --role "customer support" --location "India"
```

The supported board keys in the script are LinkedIn, Remote OK, Remotive, Wellfound, We Work Remotely, Himalayas, FlexJobs, Indeed, and Naukri. The script formats search URLs; it does not open a browser or confirm that a listing exists. Search sites may change their URL formats.

`--check` asks the user yes/no questions for eight scam indicators and totals the selected weights. It is a self-reported checklist, not an automated verification or fraud detector. `--export` writes an empty tracker workbook. `--daily` writes a Markdown search sheet and calls `~/.claude/bin/llm-burst` when available; without it, the script records a fallback message.

## Data and safety

The daily mode sends a prompt containing the requested role to the local `llm-burst` executable, which may route it to configured model providers. This repository does not establish which providers are configured or how they handle data. Review that executable and configuration before use. Do not send private resumes, contact details, or employer data through it without understanding the destination.

The helper only constructs links and local reports. Review each employer and listing independently, and use official employer channels before sharing personal information or paying any fee.

## Evidence and limitations

- Commands above are documented from the tracked script; they have not been executed as part of this README review.
- Board URLs, availability, search results, scam thresholds, job-market advice, and weekly targets are not validated by tests or live checks.
- The repository has no license file and GitHub metadata reports no declared license. Do not infer permission to reuse or redistribute its materials.
- Prices and service packages in the agent reference are not verified or implemented by this CLI.

## Maintainer

[hmzainjamil](https://github.com/hmzainjamil)
