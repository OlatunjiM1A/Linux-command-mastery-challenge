# Day 30 Capstone Tasks — Full System Command Mastery Review

1. **Build a full system health-check script** — Combines uptime,
   memory, disk, and service checks into one script that reports
   overall system health in a single run, rather than checking each
   thing manually and separately.

2. **Combine ps + systemctl + journalctl in one report** — Pulls
   process status, service state, and recent logs together, since no
   single command gives the full picture of whether something is
   actually healthy on its own.

3. **SSH into a remote host and run a command** — Connects to a remote
   server over an encrypted session and executes a command there
   directly, without needing an interactive login first.

4. **scp a file as part of a deployment** — Securely copies a file to a
   remote server as part of an automated deployment step, rather than
   as a one-off manual transfer.

5. **Apply chmod/chown to deployed files** — Sets the correct
   permissions and ownership on a file immediately after deploying it,
   so it isn't left with default or overly permissive access.

6. **Schedule the health check with cron** — Adds the health-check
   script to crontab so it runs automatically on a schedule, instead of
   needing to be triggered manually every time.

7. **Parse logs with grep, awk, and sed** — Filters, extracts, and
   transforms log data using a pipeline of small text-processing tools
   chained together, rather than reading raw logs manually.

8. **Use find to clean up stale files** — Searches for old or unused
   files (e.g. based on modification time) and removes them as part of
   routine system maintenance.

9. **Run a security audit (last, who, history)** — Reviews login
   history, currently active sessions, and command history together as
   a basic security check on the system.

10. **Present the 300-command journal for review** — Walks through the
    full Command Journal built across all 30 days, demonstrating that
    each command and its purpose can be explained clearly, unprompted.
