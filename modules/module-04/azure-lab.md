# Module 04 - Azure Lab

## Tools
- tcpdump / packet capture extension
- Azure Network Watcher logs

## Commands
```bash
sudo tcpdump -i eth0 -w capture.pcap
```
**Expected Output:**
- PCAP file generated with network packets.

## Troubleshooting
- **Issue:** Empty capture  
  **Fix:** Generate test traffic and verify capture interface.
