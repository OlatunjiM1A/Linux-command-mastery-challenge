# Day 4 — Practice Drill

## Task

Find every .conf file under /etc, find every file larger than 1MB in /var, then report total disk usage of /home and remaining free space on the root filesystem
## Commands I Ran

```bash
find /etc -name "*.conf"
find /var -type f -size +1M
du -sh /home
df -h /
