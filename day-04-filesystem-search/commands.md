# Day 04 Commands — Searching the Filesystem

1. **find -name** — Searches a directory tree for files matching a
   specific name pattern (e.g. `find /etc -name "*.conf"`). This is the
   most direct way to hunt for a file when you know roughly what it's
   called.

2. **find -type** — Filters find's results by type — `f` for regular
   files, `d` for directories. Useful for narrowing a search when a name
   pattern alone would return too much.

3. **find -size** — Filters results by file size (e.g. `+1M` for files
   larger than 1MB). Good for tracking down unusually large files eating
   up disk space.

4. **find -mtime** — Filters results by when a file was last modified,
   measured in days. Useful for finding recently changed files, which
   can also matter when investigating unexpected activity.

5. **find -perm** — Filters results by permission mode, letting you find
   files with a specific, sometimes risky, permission setting (like
   world-writable files).

6. **locate** — Searches a prebuilt index of the filesystem for a
   filename, which makes it much faster than find. The trade-off is it
   only knows about files that existed the last time the index was
   updated.

7. **updatedb** — Manually refreshes the index that locate searches
   against. Needed if you've just created a file and locate isn't
   finding it yet.

8. **du** — Reports disk usage, showing how much space files and
   directories are taking up, broken down item by item.

9. **du -sh** — Same as du, but summarized into a single total (-s) and
   shown in human-readable units like K, M, G (-h) instead of raw
   bytes.

10. **df -h** — Shows disk space usage and availability for entire
    mounted filesystems, in human-readable format. This is what tells
    you how much free space is left on a drive, not just inside one
    folder.
