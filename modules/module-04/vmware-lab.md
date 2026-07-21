# Module 04 - VMware Lab

## Tools
- Wireshark

## Steps
1. Start capture on host-only adapter.
2. Apply filter `tcp.port == 445 or dns`.
3. Export packet list and notable conversations.

**Expected Output:**
- Filtered packet stream and observable behavior timeline.

## Troubleshooting
- **Issue:** Wrong adapter selected  
  **Fix:** Re-run capture on VM host-only/internal adapter.
