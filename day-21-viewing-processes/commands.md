# Day 21 Commands — Viewing Processes

1. **ps aux** — Lists every running process on the system in a
   detailed, BSD-style format, showing user, PID, CPU/memory usage, and
   the command that started it.

2. **ps -ef** — Similar to ps aux but in a different (System V-style)
   format, showing parent process IDs as well — useful for tracing
   which process spawned which.

3. **ps -u** — Filters ps output to show only processes owned by a
   specific user, instead of everyone on the system.

4. **top** — Opens a live, continuously updating view of running
   processes, sorted by resource usage by default. Good for watching
   what's consuming CPU or memory in real time.

5. **htop** — An improved, more visual version of top with color output,
   scrolling, and easier process management — not installed by default
   on every system, so it may need to be installed separately.

6. **pgrep** — Searches for processes by name and returns their PIDs
   directly, without needing to scroll through full ps output to find
   them.

7. **pstree** — Displays running processes as a tree, showing the
   parent-child relationships between them — which process started
   which.

8. **lsof -i** — Lists open network connections and which process owns
   each one, including which ports are currently in use.

9. **jobs** — Lists background and suspended jobs running in the
   current shell session specifically, not the whole system.

10. **nice / renice** — nice starts a new process with an adjusted
    priority level; renice changes the priority of a process that's
    already running. Lower numbers mean higher priority for CPU time.
