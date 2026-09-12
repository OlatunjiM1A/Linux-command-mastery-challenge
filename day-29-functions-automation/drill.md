# Day 29 Practice Drill

## Task
Turn yesterday's script into a reusable function that accepts a service
name as an argument, checks its status, restarts it if stopped, and
schedule it to run hourly with cron.

## Script (monitor-check.sh)

#!/bin/bash

check_service() {
    service_name=$1
    if systemctl is-active --quiet "$service_name"; then
        logger "Service $service_name is running."
    else
        logger "Service $service_name was down. Restarting..."
        sudo systemctl restart "$service_name"
    fi
}

check_service "$1"

## Commands run, in order

nano monitor-check.sh
chmod +x monitor-check.sh
./monitor-check.sh cron
crontab -e
# Added: 0 * * * * /mnt/c/Users/DELL/monitor_check.sh >> /var/log/service_monitor.log 2>&1
crontab -l

