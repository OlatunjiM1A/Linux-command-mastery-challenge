# Day 30 Capstone Drill

## Task
CAPSTONE PROJECT. Ship one Bash script that connects to a remote server
over SSH, deploys a file with the correct ownership and permissions,
restarts the relevant service, verifies it is healthy using systemctl
and journalctl, and logs the entire run. Then walk a peer through it
end to end, using only commands from this challenge.

## Script (health-check.sh)

#!/bin/bash

# Day 30 Capstone: Deploy, verify, and log a service health check

REMOTE_USER="ubuntu"
REMOTE_HOST="54.237.196.145"
SERVICE_NAME="cron"
LOCAL_FILE="deploy-config.txt"
REMOTE_PATH="/home/$REMOTE_USER/deploy-config.txt"

logger "Starting capstone deployment for $SERVICE_NAME"

# Deploy the file
scp "$LOCAL_FILE" "$REMOTE_USER@$REMOTE_HOST:$REMOTE_PATH"

# Set correct ownership and permissions on the remote file
ssh "$REMOTE_USER@$REMOTE_HOST" "sudo chown $REMOTE_USER:$REMOTE_USER $REMOTE_PATH && chmod 644 $REMOTE_PATH"

# Restart the service and verify it's active
ssh "$REMOTE_USER@$REMOTE_HOST" "sudo systemctl restart $SERVICE_NAME"

if ssh "$REMOTE_USER@$REMOTE_HOST" "systemctl is-active --quiet $SERVICE_NAME"; then
    logger "$SERVICE_NAME restarted successfully and is active."
else
    logger "$SERVICE_NAME failed to restart. Check journalctl for details."
fi

# Pull recent logs for the service to confirm health
ssh "$REMOTE_USER@$REMOTE_HOST" "journalctl -u $SERVICE_NAME --since today -p err"

logger "Capstone deployment run complete."

## Commands run, in order

nano Capstone.sh
chmod +x Capstone.sh
./Capstone.sh
ory | tail -20

