# Module 01 - Azure Lab

## Objective
Perform safe reconnaissance activities against approved lab assets in Azure.

## Tools
- Azure CLI
- nslookup / dig
- nmap (approved targets only)

## Tool-by-Tool Commands

### 1) List resources in lab RG
```bash
az resource list --resource-group <LAB_RG> -o table
```
**Expected Output (example):**
- Table containing VM, NIC, NSG, Public IP resources.

### 2) Resolve target DNS
```bash
nslookup <target-fqdn>
```
**Expected Output (example):**
- Name and Address records returned for the target.

### 3) Safe service discovery (authorized target only)
```bash
nmap -sV -Pn <target-ip>
```
**Expected Output (example):**
- Open ports list with probable service versions.

## Tasks
1. Create a lab target inventory from your Azure resources.
2. Collect passive metadata.
3. Perform controlled active recon on approved targets.
4. Document exposed services and potential risks.

## Validation Checklist
- [ ] Inventory includes all in-scope targets
- [ ] DNS evidence captured
- [ ] Scan evidence captured
- [ ] Findings mapped to risk

## Troubleshooting
- **Issue:** `az` command not found  
  **Fix:** Install Azure CLI and restart terminal.
- **Issue:** DNS lookup times out  
  **Fix:** Verify NSG/DNS settings and target FQDN.
- **Issue:** nmap shows host down  
  **Fix:** Confirm VM is running, NSG allows probe path, and use `-Pn`.

## Deliverable
- Recon technical report and executive summary.
