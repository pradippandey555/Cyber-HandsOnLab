# Azure Setup Guide

## Objective
Create a safe, cost-aware Azure lab environment for cybersecurity learning.

## Steps
1. Create a dedicated Resource Group (RG) for labs.
2. Create a virtual network (VNet) and segmented subnets.
3. Deploy 2-3 VMs for attacker/defender simulation in approved lab scenarios.
4. Enable Microsoft Defender for Cloud (if available).
5. Configure Azure Monitor / Log Analytics workspace.
6. Apply NSG rules to restrict exposure.
7. Tag resources by module and owner.
8. Set budgets and cost alerts.

## Safety Controls
- Do not expose management ports publicly unless strictly needed.
- Use JIT access or Bastion where possible.
- Shut down unused VMs to control costs.

## Deliverables
- Architecture screenshot
- Cost alert proof
- NSG baseline policy export
