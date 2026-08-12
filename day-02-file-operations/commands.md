# Day 02 Commands — Creating, Copying, Moving, Deleting

1. **mkdir** — Creates a new, empty directory. If the parent folder
   doesn't already exist, this command fails.

2. **mkdir -p** — Creates a directory along with any missing parent
   directories in the path, all in one go. This is what lets you build
   a nested structure like `practice/2026/april` with a single command.

3. **touch** — Creates a new, empty file if it doesn't exist. If the file
   already exists, it just updates its "last modified" timestamp without
   changing its content.

4. **cp** — Copies a file from one location to another, leaving the
   original in place. Fails if you try to use it on a directory without
   the -r flag.

5. **cp -r** — Copies a directory recursively, meaning it copies the
   folder and everything inside it, including subfolders.

6. **mv** — Moves a file or folder to a new location. Also used to
   rename a file, since renaming is really just "moving" it to a new
   name in the same place.

7. **rm** — Deletes a single file permanently. There's no recycle bin —
   once it's gone, it's gone.

8. **rm -r** — Deletes a directory and everything inside it, recursively.
   Needed because plain `rm` refuses to touch directories.

9. **rm -rf** — Same as rm -r, but the -f (force) flag skips any
   confirmation prompts and ignores errors like missing files. This is
   the most dangerous command on this list — one wrong path and there's
   no undo.

10. **rmdir** — Deletes a directory, but only if it's completely empty.
    Safer than rm -r since it refuses to touch a folder that still has
    files in it.
