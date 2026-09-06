# Day 24 Practice Drill

## Task
List every failed service on the box, then pull today's logs for one
specific service, filtered to errors only, and follow it live for one
minute.

## Commands run, in order

systemctl list-units --state=failed
journalctl -u cron --since today -p err
journalctl -u cron -f

