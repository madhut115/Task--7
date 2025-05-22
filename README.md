#  Task 7: System Monitoring with Netdata

## Objective
Set up **Netdata** using Docker to monitor real-time system metrics like CPU, memory, disk, and Docker containers.

## Tools
- Netdata
- Docker

## Setup
```bash
docker run -d --name=netdata -p 19999:19999 --cap-add SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata

Access at: http://localhost:19999

# Monitored Metrics
 CPU & RAM usage
 Disk I/O
 Network stats
 Docker containers

# Screenshots
(Screenshot of the dashboard is present in repo)

