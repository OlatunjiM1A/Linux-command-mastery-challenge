# Day 23 Practice Drill

## Task
Pick a service, stop it, confirm it is inactive, restart it, enable it
to auto-start at boot in a single combined command, and confirm both
its active and enabled state.

## Commands run, in order

sudo systemctl stop cron
systemctl is-active cron
sudo systemctl restart cron
sudo systemctl enable --now cron
systemctl is-active cron
systemctl is-enabled cron

