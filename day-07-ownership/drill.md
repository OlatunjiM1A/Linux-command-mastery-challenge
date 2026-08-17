# Day 7 — Ownership & Special Bits Drill

## Objective

Create a shared project directory, apply the SGID bit so new files inherit its group, and audit the system for unexpected SUID binaries.

## Shared Project Directory

```bash
mkdir ~/day7-practice/shared-project
chmod g+s ~/day7-practice/shared-project
ls -ld ~/day7-practice/shared-project
touch ~/day7-practice/shared-project/newfile.txt
ls -l ~/day7-practice/shared-project/newfile.txt
sudo find / -perm /4000 -type f 2>/dev/null
