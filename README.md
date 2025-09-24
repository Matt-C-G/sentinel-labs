# Sentinel Labs (Lab-Simulated)

**What this proves** — Hunt (6 KQL) → Detect (3 rules) → Respond (playbook) → Report (workbook + KEV).

**Quick Start**
1) Watchlist → upload `data/watchlists/kev_subset.csv` as `KEV`
2) Workbooks → Add → Advanced Editor → paste `workbooks/workbook_core.json`
3) Analytics → Import the 3 rules (enable)
4) Logic Apps → Deploy `playbooks/playbook_tag_assign.json` → grant "Microsoft Sentinel Responder" → Automation: run playbook

> Lab-simulated; replace SVG evidence with redacted screenshots when available.