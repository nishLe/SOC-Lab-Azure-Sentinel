# SOC-Lab-Azure-Sentinel

<img width="858" height="507" alt="honeynet diagram" src="https://github.com/user-attachments/assets/42c31e1c-55ae-41b2-b332-50818d694ca5" />

## Live SOC + Honeynet (Azure) — Lab Repository


This repository organizes the Live SOC + Honeynet lab for Azure Sentinel described in the original `Live_SOC_Honeynet_Azure_Lab.docx`.


### Purpose
- Deploy a small lab in Azure with intentionally vulnerable VMs (Windows + Linux) and an Attacker VM.
- Collect and forward logs to a Log Analytics Workspace.
- Use Microsoft Sentinel to visualize attack maps, run detections, and respond to incidents.


### Repo Contents
- `docs/` — step-by-step lab phases and operational runbook
- `KQL/` — queries used in workbooks and analytics rules
- `workbooks/` — JSON definitions of map visualizations
- `analytics-rules/` — sample detection rule JSON for import into Sentinel
- `scripts/` — automation snippets for auditing, DCRs, and log generation
- `playbooks/` — sample Logic App playbooks to trigger on incidents


### Quickstart (local)
1. Clone this repository:


```bash
git clone https://github.com/<your-org>/SOC-Lab-Azure-Sentinel.git
cd SOC-Lab-Azure-Sentinel
