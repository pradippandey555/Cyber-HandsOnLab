# Lab Troubleshooting Playbook

## Common Problems

### 1) Network Connectivity Failures
- Verify VM NIC mode (host-only/internal/NAT as required)
- Confirm IP assignment and subnet alignment
- Test with ping and traceroute in isolated range

### 2) Tool Installation Errors
- Check OS compatibility and package sources
- Run package manager update first
- Review service status after install

### 3) No Logs or Missing Telemetry
- Confirm logging agents running
- Check time sync/NTP
- Validate destination workspace/index configuration

### 4) Scan Results Inconsistent
- Re-validate scope and target reachability
- Repeat with same parameters and compare
- Account for firewall/EDR interference

### 5) Azure Access/Permission Issues
- Verify role assignments and scope
- Reauthenticate CLI: `az login`
- Confirm subscription context: `az account show`
