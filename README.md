# Sentinel Labs — SOC/SC-200 Proof Pack

**Purpose:** Demonstrate Microsoft Sentinel capability: KQL hunting, analytics rules, a workbook, a basic playbook, and a KEV watchlist. All importable and demo-friendly.

## Included
- `kql/` — 6 hunting queries
- `analytics-rules/` — 3 scheduled rules (JSON)
- `workbooks/` — 1 workbook (JSON)
- `playbooks/` — 1 Logic App (ARM) to tag & assign incidents
- `data/watchlists/` — KEV subset CSV
- `evidence/` — add screenshots here after import/tests
- `onepager/` — recruiter one-pager

## Quick start (import order)
1. Upload `data/watchlists/kev_subset.csv` as a **Watchlist** named `KEV`.
2. Import `workbooks/workbook_core.json` (Workbooks → Add → Advanced Editor).
3. Import rules from `analytics-rules/` and enable them.
4. Deploy `playbooks/playbook_tag_assign.json` (Logic Apps). Give its managed identity **Microsoft Sentinel Responder** on the workspace and wire it to rules (Automation).

## Talk track
- **Hunt** with KQL (sign-ins, DNS, tamper, local admin, USB, RDP).
- **Detect** by promoting high-signal hunts to **scheduled rules**.
- **Respond** automatically: playbook **tags + assigns** incidents to Tier‑1.
- **Report**: workbook shows **KEV exposure** and detection activity.

— Updated 2025-09-24
