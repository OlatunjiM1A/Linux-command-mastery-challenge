# Day 22 Commands — Controlling Processes with Signals

1. **kill** — Sends a termination signal to a process by its PID,
   requesting it to shut down gracefully by default (SIGTERM).

2. **kill -9** — Sends the SIGKILL signal, forcing the process to stop
   immediately without giving it a chance to clean up or shut down
   gracefully. Used as a last resort when a process won't respond to a
   normal kill.

3. **kill -HUP** — Sends the hangup signal, which many services
   interpret as "reload your configuration" rather than "stop
   completely."

4. **killall** — Kills all processes matching a given name, rather than
   requiring a specific PID like kill does.

5. **pkill** — Similar to killall, but matches processes based on a
   pattern rather than an exact name, giving more flexible matching.

6. **fg** — Brings a background or suspended job back into the
   foreground, resuming its output and control in the current terminal.

7. **bg** — Resumes a suspended job, but keeps it running in the
   background instead of bringing it back to the foreground.

8. **Ctrl+Z (suspend)** — Pauses (suspends) the currently running
   foreground process without terminating it, freeing up the terminal
   until you resume it with fg or bg.

9. **nohup** — Runs a command in a way that ignores the hangup signal,
   meaning the process keeps running even after the terminal session
   that started it closes or you log out.

10. **disown** — Removes a job from the shell's job table, detaching it
    so it won't be affected by the shell closing, even without nohup
    having been used when it started.
