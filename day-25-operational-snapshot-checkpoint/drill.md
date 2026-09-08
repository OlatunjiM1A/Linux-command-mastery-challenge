# Day 25 Practice Drill

## Task
CHECKPOINT. Build a one-screen operational snapshot of a server
covering uptime, memory, the status of three key services, and any
scheduled cron jobs.

## Commands run, in order

uptime
free -h
systemctl status cron
echo "=== CRON SERVICE ===" && sudo systemctl status cron --no-pager
crontab -l
