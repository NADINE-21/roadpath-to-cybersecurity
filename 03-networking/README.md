# Networking Fundamentals

## Topics
- [ ] IPv4 addresses and CIDR
- [ ] Private vs. public IP addresses
- [ ] Default gateways and routing tables
- [ ] DNS resolution
- [ ] TCP vs. UDP and common ports
- [ ] Basic connectivity troubleshooting
- [ ] Packet capture concepts

## Suggested commands
```bash
ip -br addr
ip route
getent hosts example.com
ping -c 4 1.1.1.1
ss -tuln
```

Record what each command tells you; do not treat a single failed ping as conclusive proof of an internet outage. Practice only on your own lab or authorized targets.