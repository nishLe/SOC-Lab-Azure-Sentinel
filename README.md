# SOC-Lab-Azure-Sentinel

<img width="600" height="507" alt="honeynet diagram" src="https://github.com/user-attachments/assets/42c31e1c-55ae-41b2-b332-50818d694ca5" />

## Live SOC + Honeynet (Azure) — Lab Repository


This repository organizes the Live SOC + Honeynet lab for Azure Sentinel described in the original `Live_SOC_Honeynet_Azure_Lab.docx`.


### Purpose
- Deploy a small lab in Azure with intentionally vulnerable VMs (Windows + Linux) and an Attacker VM.
- Collect and forward logs to a Log Analytics Workspace.
- Use Microsoft Sentinel to visualize attack maps, run detections, and respond to incidents.


### Repo Contents
- `docs` — step-by-step lab phases and operational runbook
- `KQL` — queries used in workbooks and analytics rules
- `workbooks` — JSON definitions of map visualizations
- `analytics-rules` — sample detection rule JSON for import into Sentinel
- `scripts` — automation snippets for auditing, DCRs, and log generation
- `playbooks` — sample Logic App playbooks to trigger on incidents
  
### Example Attack Map for Windows RDP Authentication Failed 
<img width="600" height="513" alt="image" src="https://github.com/user-attachments/assets/6d4d0b61-77f7-4f71-9d28-f5b704ae2f1b" />

### Incident Report
<img width="700" height="723" alt="image" src="https://github.com/user-attachments/assets/b0b27bf1-0f8b-4c7a-86ba-78a704a3cae2" />


### Quickstart (local)
1. Clone this repository:


```bash
git clone https://github.com/<your-org>/SOC-Lab-Azure-Sentinel.git
cd SOC-Lab-Azure-Sentinel
