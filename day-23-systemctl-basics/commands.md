# Day 23 Commands — Init Systems & systemctl Basics

1. **systemctl start** — Starts a systemd service immediately, without
   affecting whether it starts automatically on future boots.

2. **systemctl stop** — Stops a currently running service immediately,
   without changing whether it's set to start automatically at boot.

3. **systemctl restart** — Stops and then starts a service again in one
   command, useful after a configuration change that requires a full
   reload.

4. **systemctl reload** — Tells a service to reload its configuration
   without fully restarting, avoiding downtime for services that
   support this.

5. **systemctl enable** — Configures a service to start automatically
   at boot, without starting it right now if it isn't already running.

6. **systemctl disable** — Removes a service from starting automatically
   at boot, without stopping it if it's currently running.

7. **systemctl enable --now** — Combines enable and start into a single
   command: the service starts immediately and is also set to
   auto-start at every future boot.

8. **systemctl status** — Shows a detailed snapshot of a service:
   whether it's active, enabled, its process ID, recent log lines, and
   more.

9. **systemctl is-active** — Returns a simple yes/no style answer for
   whether a service is currently running, without the full status
   detail.

10. **systemctl is-enabled** — Returns a simple yes/no style answer for
    whether a service is set to start automatically at boot.
