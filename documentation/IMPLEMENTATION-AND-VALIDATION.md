# Implementation and validation notes

## Configuration areas visible in supplied worksheet

1. AD DS and DNS management consoles
2. HR OU and group membership properties
3. IP configuration on router, servers, and clients
4. DNS forward lookup zone and zone-transfer settings; secondary SOA
5. DFS namespace and HR file permissions
6. DHCP scopes and leases
7. RRAS/NAT and DHCP relay configuration
8. Connectivity command outputs

## Validation limitations

These screenshots are historical evidence, not current lab test results. No running VMs or live credentials were provided, so the portfolio does not claim that the network was retested. Blank worksheet fields remain unverified. Screenshots show examples of command output; individual host connectivity should be confirmed by inspecting the full-resolution images.

## Suggested future verification

- Confirm DC and DNS health (`dcdiag`, `nslookup`)
- Check secondary DNS zone transfer and SOA serial
- Verify DHCP scope allocation and client leases
- Test NAT and relay across both internal subnets
- Validate department user read/write/delete permissions with separate test accounts
- Test DFS paths from both Windows clients
