# Roadpath to Cybersecurity

My hands-on journey into cybersecurity, documenting my learning, lab setup, troubleshooting, and practical exercises.

## Day 1 — Lab Setup and Network Troubleshooting

### Environment
- Host operating system: Windows 11
- Installed RAM: 20 GB
- Storage: 1 TB
- Hypervisor: VMware Workstation
- Virtual machine: Kali Linux Rolling

### What I accomplished
- Started and accessed my Kali Linux virtual machine.
- Inspected the network interface using `ip -br addr`.
- Identified the active `eth0` interface and its IPv4 configuration.
- Inspected the routing table using `ip route`.
- Tested DNS resolution using `getent hosts example.com`.
- Encountered a connectivity issue and worked to resolve it.
- Restored network connectivity in my virtual machine.

### Commands practiced
```bash
ip -br addr
ip route
getent hosts example.com
ping -c 4 1.1.1.1
```

### What I learned
- How to inspect Linux network interfaces.
- How to identify an IP address and default gateway.
- How to test DNS resolution.
- How to begin troubleshooting virtual machine connectivity.

### Next steps
- Verify network connectivity.
- Create a VMware recovery snapshot.
- Practice Linux command-line fundamentals.
- Continue documenting hands-on cybersecurity exercises.
