# Day 05 Commands — Paths, Links & Tree Structures (Checkpoint)

1. **tree** — Displays a directory and all its contents as a visual,
   branching tree structure. Much easier to scan than scrolling through
   repeated `ls` calls in every subfolder.

2. **tree -L** — Same as tree, but limits how many levels deep it goes
   (e.g. `tree -L 2` shows only two levels). Useful for getting an
   overview of a large directory without being flooded with every
   nested file.

3. **ln (hard link)** — Creates a second name pointing to the exact same
   file data on disk. Both names are equal — deleting one doesn't remove
   the underlying data as long as the other still exists.

4. **ln -s (symbolic link)** — Creates a shortcut file that points to
   another file's path, not its data. If the original file is deleted or
   moved, the symlink breaks and points to nothing.

5. **readlink** — Shows what a symbolic link is actually pointing to,
   letting you see the real target path behind a shortcut.

6. **realpath** — Resolves and prints the full, absolute path of a file
   or symlink, following any links along the way to show the true
   location.

7. **basename** — Strips the directory part of a path and returns just
   the filename (e.g. `basename /var/log/syslog` returns `syslog`).

8. **dirname** — The opposite of basename — strips the filename and
   returns just the directory path (e.g. `dirname /var/log/syslog`
   returns `/var/log`).

9. **pushd / popd** — pushd saves your current directory onto a stack
   and moves you to a new one; popd jumps back to the last saved
   directory. Like a more powerful version of `cd -` that remembers more
   than one previous location.

10. **ls -lt** — Lists files in long format, sorted by modification time
    with the most recently changed files shown first.
