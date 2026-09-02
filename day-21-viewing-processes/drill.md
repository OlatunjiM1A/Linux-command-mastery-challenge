# Day 21 Practice Drill

## Task
Find the PID of a running process by name, view it in top, show it as
part of the process tree, and identify which process is using port 80.

## Commands run, in order

pgrep -f process_name
top -p PID
pstree -p | grep sshd
sudo lsof -i :80

