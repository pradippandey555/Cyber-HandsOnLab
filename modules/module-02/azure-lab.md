# Module 02 - Azure Lab

## Objective
Harden Linux VM baselines in Azure.

## Tools
- Azure CLI
- SSH
- ufw / firewall-cmd
- systemctl / journalctl

## Tool-by-Tool Commands

### 1) Connect via SSH
```bash
ssh <user>@<vm-public-ip>
```
**Expected Output:** Successful shell login.

### 2) Apply updates
```bash
sudo apt update && sudo apt -y upgrade
```
**Expected Output:** Package lists updated and upgrades applied.

### 3) Enable firewall
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow 22/tcp
sudo ufw enable
sudo ufw status verbose
```
**Expected Output:** Firewall active with defined rules.

### 4) Check auth logs
```bash
sudo journalctl -u ssh --since "-1h"
```
**Expected Output:** Recent SSH auth events.

## Validation Checklist
- [ ] VM patched
- [ ] Firewall active
- [ ] SSH hardened
- [ ] Logs visible

## Troubleshooting
- **Issue:** SSH refused  
  **Fix:** Verify NSG inbound rule and VM power state.
- **Issue:** ufw inactive after reboot  
  **Fix:** `sudo systemctl enable ufw`.
