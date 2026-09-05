# Day 23 Practice Drill

## Task
Pick a service, stop it, confirm it is inactive, restart it, enable it
to auto-start at boot in a single combined command, and confirm both
its active and enabled state.

## Commands run, in order

sudo systemctl stop ssh
systemctl is-active ssh
sudo systemctl restart ssh
sudo systemctl enable --now ssh
systemctl is-active ssh
systemctl is-enabled ssh

