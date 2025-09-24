# Sentinel Labs (Lab-Simulated)

**What this proves** — Hunt (6 KQL) → Detect (3 rules) → Respond (playbook) → Report (workbook + KEV).

**Quick Start**
1) Watchlist: upload `data/watchlists/kev_subset.csv` as `KEV`
2) Workbooks: Add → Advanced Editor → paste `workbooks/workbook_core.json`
3) Analytics: Import 3 rules (enable)
4) Logic Apps: Deploy `playbooks/playbook_tag_assign.json` → grant "Microsoft Sentinel Responder" → Automation (run playbook)

**Note:** events are simulated to avoid real data; replace SVGs in `evidence/` with real redacted screenshots later.

## Components

- **KQL Hunts:** 6 queries for hunting (tamper, local admin, RDP spike, DNS, signins, USB)
- **Analytics Rules:** 3 scheduled rules that create incidents
- **Workbook:** Dashboard with KEV watchlist integration
- **Playbook:** Logic App for auto-tagging and assignment
- **Evidence:** Screenshots of incidents, workbooks, and rule hits

## Test Triggers

Use `kql/test_triggers.kql` to simulate incidents in Sentinel Logs without real data.

## Pages Site

Live documentation: https://matt-c-g.github.io/sentinel-labs/