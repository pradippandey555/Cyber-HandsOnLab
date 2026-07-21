# VMware Local Lab Setup Guide

## Objective
Build an isolated and repeatable local cybersecurity lab.

## Steps
1. Install VMware and create dedicated lab folder structure.
2. Create virtual network segments (host-only / internal).
3. Deploy attacker VM, defender VM, and optional server VM.
4. Enable snapshots before each module.
5. Configure local DNS/hosts entries for lab convenience.
6. Validate inter-VM connectivity and firewall rules.

## Safety Controls
- Keep lab network isolated from production/home networks where possible.
- Do not run scans against unauthorized systems.
- Revert to snapshots after risky tests.

## Deliverables
- VM inventory sheet
- Network topology diagram
- Snapshot and rollback checklist
