# Module 01 - VMware Lab

## Objective
Perform safe reconnaissance in an isolated local VM environment.

## Tools
- ipconfig/ifconfig
- nmap
- arp

## Tool-by-Tool Commands

### 1) Identify local interface/network
```bash
ip a
```
**Expected Output:** Interface list with local subnet range.

### 2) ARP table review
```bash
arp -a
```
**Expected Output:** Known hosts and MAC mappings.

### 3) Service scan in isolated subnet
```bash
nmap -sV 192.168.56.0/24
```
**Expected Output:** Host list and service banners for reachable lab VMs.

## Validation Checklist
- [ ] Local subnet identified
- [ ] Hosts discovered in isolated network
- [ ] Service evidence recorded

## Troubleshooting
- **Issue:** No hosts discovered  
  **Fix:** Ensure VMs are on same host-only/internal network and powered on.
- **Issue:** Permission denied on scan  
  **Fix:** Run with elevated privileges where required.
