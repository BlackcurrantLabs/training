# Networking & Shell Scripting

## Topics

- Client-server model, IP addresses, ports
- CIDR notation and subnetting - what `10.0.0.0/24` actually means (needed for the VPC section later)
- Public vs private IPs, what NAT is for, and what a default gateway does
- DNS - how a domain becomes an IP (A, AAAA, CNAME records)
- TCP vs UDP (conceptual), the HTTP/HTTPS request-response lifecycle, status codes
- Load balancers - Layer 4 vs Layer 7 (concept)
- Firewalls and security groups (concept)
- Bash scripting: variables, loops, conditionals, cron jobs

## How to learn

- **Networking** - [Cloudflare Learning Center](https://www.cloudflare.com/learning/) - read the DNS, CDN, Load Balancing, and HTTP sections.
- **Bash** - [freeCodeCamp's Bash scripting course](https://www.freecodecamp.org/news/bash-scripting-tutorial-linux-shell-script-and-command-line-for-beginners/).

## How to practice

Run `dig`, `nslookup`, `ping`, `traceroute`, and `curl` against real domains and read the output. Write scripts for a folder backup, an hourly disk-usage logger via `cron`, and a site-down reporter.

## Resources

- [Cloudflare Learning Center](https://www.cloudflare.com/learning/)
- [freeCodeCamp - Bash Scripting](https://www.freecodecamp.org/news/bash-scripting-tutorial-linux-shell-script-and-command-line-for-beginners/)
- [Missing Semester: Command Line](https://missing.csail.mit.edu/2020/course-shell/)
