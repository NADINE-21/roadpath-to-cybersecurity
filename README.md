# Roadpath to Cybersecurity

A hands-on record of my journey learning cybersecurity through practical labs and documented troubleshooting.

## Day 1 — Kali Linux Lab Setup and Network Troubleshooting

### Environment
- Host operating system: Windows 11
- Installed RAM: 20 GB
- Storage: 1 TB
- Hypervisor: VMware Workstation
- Virtual machine: Kali Linux Rolling

### What I did
- Started Kali Linux in VMware Workstation and opened a terminal.
- Inspected network interfaces with `ip -br addr`.
- Confirmed that `eth0` was up and had the private IPv4 address `192.168.175.136/24`.
- Inspected the routing table with `ip route` and observed a default route via `192.168.175.2`.
- Tested name resolution with `getent hosts example.com`; it returned IPv6 addresses.
- Tested connectivity with `ping -c 4 1.1.1.1`; initially, no ping replies were received.
- Troubleshot the VM's network configuration and resolved the connectivity issue.

### Commands practiced
```bash
ip -br addr
ip route
getent hosts example.com
ping -c 4 1.1.1.1
```

### What I learned
- How to inspect Linux network interfaces and IP configuration.
- How to identify a default gateway from the routing table.
- How to test DNS resolution and basic network connectivity.
- Why a failed ping alone does not prove that all internet connectivity is unavailable.
- The value of troubleshooting systematically and verifying a fix.

### Next steps
- Verify connectivity after the fix.
- Create a VMware recovery snapshot.
- Practice Linux command-line fundamentals.
- Continue documenting hands-on cybersecurity exercises.

> This report records only the work completed and observations made during this session. The exact network change that resolved the issue has not been documented yet.
