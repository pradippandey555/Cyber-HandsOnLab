# Module 05 - Azure Lab

## Tools
- PowerShell
- AD tools

## Commands
```powershell
Get-ADUser -Filter * | Select-Object Name,Enabled
Get-ADGroupMember "Domain Admins"
```
**Expected Output:**
- User inventory and privileged membership list.

## Troubleshooting
- **Issue:** AD cmdlets unavailable  
  **Fix:** Install RSAT/AD module and run as domain-joined admin.
