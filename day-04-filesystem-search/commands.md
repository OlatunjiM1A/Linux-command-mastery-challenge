# Day 04 Commands — Searching the Filesystem

1. **find -name** — It searches a directory tree for files matching a
   specific name pattern (e.g. `find /etc -name "*.conf"`). 

2. **find -type** — Filters find's results by type — `f` for regular
   files, `d` for directories. Useful for narrowing a search when a name
   pattern alone would return too much.

3. **find -size** — Filters results by file size (e.g. `+1M` for files
   larger than 1MB). Good for tracking down unusually large files eating
   up disk space.

4. **find -mtime** — It find files based on when they last modified, it is 
   measured in days. It is useful for finding recently changed files.

5. **find -perm** — it finds result by permission mode, majorly by their Linux permission

6. **locate** — It searches a prebuilt index of the filesystem for a
   filename, it makes it much faster than find. it only knows about files that existed
   the last time the index was updated.

7. **updatedb** — Manually refreshes the index that locate searches
   against. Needed if you've just created a file and locate isn't
   finding it yet.

8. **du** — It shows how much storage space files and directries are using.

    
9. **du -sh** — Same as du, but summarized into a single total (-s) and
   shown in human-readable.

10. **df -h** — It shows how much disk space is available and being used on your storage/filesystems in a human readable format.
