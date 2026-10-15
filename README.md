# Roadpath to Cybersecurity
Status: In progress

A beginner-friendly, hands-on portfolio documenting my cybersecurity learning journey, home lab, command-line practice, troubleshooting, and authorized security exercises.

> **Learning rule:** Only test systems I own or have explicit permission to assess. Never publish passwords, tokens, private keys, personal data, or sensitive network details.

## Current status

- [x] **Day 1 — Kali Linux lab setup and network troubleshooting** — documented below.
- [ ] **Day 2 — Linux command-line fundamentals**
- [ ] Linux permissions and users
- [ ] Networking fundamentals
- [ ] Security fundamentals
- [ ] Blue Team / SOC exercises
- [ ] Safe, authorized ethical-hacking labs

## Repository map

| Path | Purpose |
|---|---|
| [01-kali-lab-setup](01-kali-lab-setup/) | Kali VM setup, network troubleshooting, and screenshots |
| [02-linux-cli](02-linux-cli/) | Navigation, files, commands, permissions, and notes |
| [03-networking](03-networking/) | IP addressing, DNS, routing, ports, and packet analysis |
| [04-security-fundamentals](04-security-fundamentals/) | Core concepts, threat models, and security notes |
| [05-blue-team-soc](05-blue-team-soc/) | Logs, detection, incident triage, and defensive labs |
| [06-ethical-hacking-labs](06-ethical-hacking-labs/) | Authorized practice labs and clearly scoped write-ups |
| [07-scripts-and-tools](07-scripts-and-tools/) | Small learning scripts and tool notes |
| [resources](resources/) | Learning resources, glossary, and references |
| [templates](templates/) | Reusable lab-report and troubleshooting templates |

## Lab environment

- Host: Windows 11
- Memory: 20 GB RAM
- Storage: 1 TB
- Hypervisor: VMware Workstation
- Security lab VM: Kali Linux Rolling

## Learning workflow

For each session:
1. Set a clear learning objective.
2. Practice in the local VM or an explicitly authorized training environment.
3. Record commands, observations, and any errors.
4. Explain what the results mean in my own words.
5. Add screenshots with sensitive information removed.
6. Record what worked, what remains uncertain, and the next step.

## Daily learning log

### Day 1 — Kali Linux lab setup and network troubleshooting

**Goal:** Start the Kali Linux VM, inspect its network configuration, and troubleshoot connectivity.

#### What I did
- Started Kali Linux in VMware Workstation and opened a terminal.
- Inspected interfaces with `ip -br addr`.
- Observed `eth0` up with private IPv4 address `192.168.175.136/24`.
- Inspected the routing table with `ip route` and observed a default route via `192.168.175.2`.
- Checked name resolution using `getent hosts example.com`; it returned IPv6 addresses.
- Tested connectivity with `ping -c 4 1.1.1.1`; initially, no ping replies were received.
- Troubleshot the VM network configuration and resolved the connectivity issue.

#### Screenshots
The screenshots are stored in [01-kali-lab-setup](01-kali-lab-setup/).

![Kali lab screenshot 1](01-kali-lab-setup/Screenshot%202026-10-15%20131204.png)

[View screenshot 2](01-kali-lab-setup/Screenshot%202026-10-15%20150303.png) · [View screenshot 3](01-kali-lab-setup/Screenshot%202026-10-15%20150720.png) · [View screenshot 4](01-kali-lab-setup/Screenshot%202026-10-15%20151220.png)

#### Commands practiced
```bash
ip -br addr
ip route
getent hosts example.com
ping -c 4 1.1.1.1
```

#### What I learned
- How to inspect Linux interfaces and IP configuration.
- How to identify a default gateway.
- How DNS lookup and basic connectivity tests differ.
- A failed ping alone does not prove that all internet connectivity is unavailable.
- Troubleshooting should be systematic and the fix should be verified.

#### Follow-up
- [ ] Verify connectivity after the fix.
- [ ] Create a VMware recovery snapshot.
- [ ] Practice Linux command-line fundamentals.

> Note: The exact network setting that resolved the original issue has not yet been recorded.

## Documentation standards

Each substantial lab should include:
- Objective and scope
- Lab environment
- Steps and commands
- Observed output (redacted where needed)
- Explanation and lessons learned
- Troubleshooting and limitations
- Screenshots or evidence where useful
- References and next steps

This repository is a learning record. It does not claim professional experience or certifications.
