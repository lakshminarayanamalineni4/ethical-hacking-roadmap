# Module 2 — Linux and Windows fundamentals

**Weeks:** 4–5  
**Outcome:** Navigate systems, inspect services, permissions and logs, and understand the execution environment.

| ID | Submodule | Concepts |
|---|---|---|
| 2.1 | Linux shell | Filesystem, paths, pipes, redirection, grep, find, sed, awk, environment variables |
| 2.2 | Users and permissions | Users/groups, sudo, rwx, chmod, chown, umask, least privilege |
| 2.3 | Processes and services | ps, top, systemctl, service status, signals, listening sockets |
| 2.4 | Logs and troubleshooting | journalctl, /var/log, auth logs, timestamps, basic filtering |
| 2.5 | Windows security basics | PowerShell, services, processes, Event Viewer, Windows Defender Firewall, local users |
| 2.6 | Shell automation | Bash/PowerShell scripts, exit codes, safe input handling, scheduled tasks |

## Practical work
- Use WSL2 Ubuntu; create a non-root user and practice permissions in a disposable directory.
- Start a local web service, inspect its process/listening port, then stop it.
- Write a script that checks whether a local service is reachable and logs the result.
- Engineering link: inspect Docker container users, mounted volumes, environment variables and logs; avoid running app containers as root.

## Exit criteria
Inspect a process, service, port, permission and relevant log on both Linux and Windows.