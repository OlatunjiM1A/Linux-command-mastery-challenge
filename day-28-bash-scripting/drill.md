# Day 28 Practice Drill

## Task
Write and execute a script that reads the user's name, checks whether
a config file exists using an if statement, and loops through three
server names pinging each one.

## Script (check-servers.sh)

#!/bin/bash

read -p "Enter your name: " name
echo "Hello, $name"

if [ -f "config.txt" ]; then
    echo "config.txt found."
else
    echo "config.txt not found."
fi

servers=("8.8.8.8" "1.1.1.1" "9.9.9.9")

for server in "${servers[@]}"; do
    echo "Pinging $server..."
    ping -c 2 "$server"
done

## Commands run, in order

nano check-servers.sh
chmod +x check-servers.sh
./check-servers.sh

