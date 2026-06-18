# Supervision Skill Model — Interactive Dashboard

A static, single-page dashboard visualizing **Supervision Skill Model (SSM)** telemetry
for 18 anonymized student software-engineering project repositories. It accompanies the
research paper *“From Prompting to Supervision: A Skill Model for Agentic Software
Engineering Education.”*

**Live:** https://sumonbis.github.io/ssm-dashboard/

## Views

- **Class Overview** — sortable heatmap of S3 (Verify), S6 (Orchestrate), and AI-adoption
  evidence across all repositories.
- **Student Detail** — per-repository radar chart of competency scores plus a
  signal-by-signal AI-adoption breakdown.
- **AI Adoption** — AI-adoption signal strength vs. S3 Verify, with the supervision-gap
  pattern highlighted.

## Running locally

No build step or backend is required — all data is embedded in the page.

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Data and privacy

All repositories are anonymized (identifiers `P01`–`P18`); no student, username, URL, or
institution information is included. Charts are rendered with Chart.js from a CDN.
