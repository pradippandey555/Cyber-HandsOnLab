# Module 07 - Azure Lab

## Tools
- Log Analytics / SIEM

## Example Query (KQL style)
```kusto
SecurityEvent
| where TimeGenerated > ago(24h)
| summarize count() by EventID
```
**Expected Output:**
- EventID counts over 24h.

## Troubleshooting
- **Issue:** No data returned  
  **Fix:** Verify agent onboarding and correct workspace selection.
