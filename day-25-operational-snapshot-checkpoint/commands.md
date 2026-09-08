# Day 25 Commands — Process & Service Checkpoint

1. **ps aux | grep** — Lists all running processes, piped through grep
   to filter down to processes matching a specific name or keyword.

2. **systemctl status <svc>** — Shows the current status of a specific
   service, including whether it's active, enabled, and its recent log
   output.

3. **journalctl -u <svc> --since today** — Shows today's log entries for
   one specific service, filtered by time.

4. **kill -0 (liveness check)** — Sends no actual signal (signal 0),
   just checks whether a process with a given PID exists and is
   reachable. A safe way to test if a process is alive without
   affecting it.

5. **uptime** — Shows how long the system has been running since its
   last boot, along with load averages over the past 1, 5, and 15
   minutes.

6. **free -h** — Shows memory usage — total, used, and free RAM and
   swap — in human-readable units.

7. **vmstat** — Reports a snapshot of system performance: processes,
   memory, swap, I/O, and CPU activity, all in one combined view.

8. **iostat** — Reports CPU usage and input/output statistics for
   storage devices, useful for spotting disk bottlenecks.

9. **watch** — Repeatedly runs a given command at a set interval,
   refreshing the output on screen — useful for monitoring something
   that changes over time without manually rerunning a command.

10. **crontab -e / crontab -l** — crontab -e opens the current user's
    scheduled cron jobs for editing; crontab -l lists them without
    opening an editor.
