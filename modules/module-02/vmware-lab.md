# Module 02 - VMware Lab

## Objective
Build and harden Linux VMs in local lab.

## Commands
```bash
sudo adduser analyst
sudo usermod -aG sudo analyst
sudo passwd -l root
sudo sed -i 's/^#\?PermitRootLogin.*/PermitRootLogin no/' /etc/ssh/sshd_config
sudo systemctl restart ssh
sudo ufw enable
sudo ufw status
```

**Expected Output:**
- New user created, root login disabled, SSH restarted, firewall enabled.

## Troubleshooting
- **Issue:** Locked out after SSH config change  
  **Fix:** Use VM console snapshot rollback and correct `sshd_config`.
