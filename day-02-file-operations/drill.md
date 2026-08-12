# Day 2 — Practice Drill

## Task

Create a nested directory structure, create three empty files,
copy the directory to a backup location, rename one file, and
remove only the empty directories left behind.

## Commands I Ran

```bash
mkdir -p practice/2026/april

touch practice/2026/april/20.txt \
practice/2026/april/30.txt \
practice/2026/april/40.txt

cp -r practice backup

mv practice/2026/april/20.txt \
practice/2026/april/renamed

ls -R practice
ls -R backup
