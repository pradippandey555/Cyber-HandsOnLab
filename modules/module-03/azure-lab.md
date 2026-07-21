# Module 03 - Azure Lab

## Tools
- nmap
- vulnerability scanner
- Azure CLI

## Commands
```bash
nmap -sn <subnet-cidr>
nmap -sV -O <target-ip>
```
**Expected Output:**
- Live hosts from ping sweep
- Service versions and OS guesses

## Troubleshooting
- **Issue:** OS detection inaccurate  
  **Fix:** Use service fingerprinting and manual validation.
