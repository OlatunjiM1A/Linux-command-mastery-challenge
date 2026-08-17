# Day 7 — Ownership & Special Bits Drill

## Objective

Create a shared project directory, apply the SGID bit so new files inherit its group, and audit the system for unexpected SUID binaries.

## Shared Project Directory

```bash
mkdir ~/day7-practice/shared-project
chmod g+s ~/day7-practice/shared-project
