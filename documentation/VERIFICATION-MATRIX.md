# Evidence and verification matrix

This matrix is intentionally conservative. **Screenshot present** means a related configuration image exists, not that the whole service is operational.

| Workstream | Assignment/design objective | Historical worksheet evidence | What remains to validate |
|---|---|---|---|
| AD DS | Centralized domain identity and departmental OUs | AD consoles, HR membership images | All users/groups and successful sign-in |
| DNS | Primary and secondary name resolution | Zone and SOA/transfer settings | Live queries and successful zone transfers |
| Subnets | Routed /27 internal networks | Interface/IP configuration images | Correct gateways and bidirectional routing |
| DHCP | Automatic address assignment and relay | Scopes, leases and relay screens | Fresh client renewals on each subnet |
| DFS & file shares | Centralized department file access | DFS and HR permissions images | Effective access for all roles and departments |
| RRAS/NAT | Connectivity between networks and WAN | Routing/NAT screens and command outputs | Repeatable end-to-end tests |
| Availability | Resilient services | Selected setup screens | DNS failover and storage/service recovery tests |

**Evidence IDs:** Filenames such as `evidence-01.png` are extraction-order identifiers, not assignment step numbers. See [Evidence Gallery](EVIDENCE-GALLERY.md).
