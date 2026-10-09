# Network design

The provided NOS 145 scenario specifies a **192.168.25.0/24** internal base network, **30 usable hosts per internal subnet**, and excludes subnet zero. A /27 mask (255.255.255.224) provides 30 usable host addresses per subnet.

| Logical subnet | Network | Usable host range | Broadcast |
|---|---|---|---|
| Subnet 2 | 192.168.25.32/27 | 192.168.25.33–192.168.25.62 | 192.168.25.63 |
| Subnet 3 | 192.168.25.64/27 | 192.168.25.65–192.168.25.94 | 192.168.25.95 |

These are **scenario-derived planning ranges**, not verified live addresses. The external WAN is supplied by the ISP/home network. The worksheet contains `ipconfig /all` captures, but precise assignments should be checked against the original screenshots before describing them as operational facts.

![Conceptual topology](../architecture/topology.svg)
