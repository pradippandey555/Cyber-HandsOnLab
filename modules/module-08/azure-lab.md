# Module 08 - Azure Lab

## Commands
```bash
az network nsg rule list -g <RG> --nsg-name <NSG> -o table
```
**Expected Output:**
- Ordered NSG rules with priorities and access decisions.

## Troubleshooting
- **Issue:** Rule not taking effect  
  **Fix:** Check priority conflicts and subnet/NIC NSG association.
