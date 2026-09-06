# Day 24 Commands — Deeper Service Management & Logs

1. **systemctl list-units --type=service** — Lists all currently loaded
   service units on the system, showing their load, active, and sub
   states at a glance.

2. **systemctl list-units --state=failed** — Filters the unit list down
   to only services that have failed, making it fast to spot problems
   without scanning the full list.

3. **systemctl daemon-reload** — Reloads systemd's configuration after
   a unit file has been changed, so systemd picks up the new definition
   without needing a full reboot.

4. **journalctl** — Displays the systemd journal, which centralizes log
   messages from services and the kernel into one queryable log system.

5. **journalctl -f** — Follows the journal live, printing new log
   entries as they're written — similar to tail -f but for the
   systemd journal specifically.

6. **journalctl -u** — Filters journal output to logs from one specific
   service unit, instead of the entire system's combined log stream.

7. **journalctl --since** — Filters journal output to entries after a
   specific point in time (e.g. "today", "1 hour ago"), narrowing a
   search by time range.

8. **journalctl -p err** — Filters journal output by priority level,
   showing only entries at "error" severity or higher, cutting out
   informational noise.

9. **tail -f /var/log/syslog** — Follows the traditional system log
   file live, showing general system-level messages as they happen in
   real time.

10. **tail -f /var/log/auth.log** — Follows the authentication log live,
    showing login attempts, sudo usage, and other security-relevant
    events as they occur.
