# Day 03 Commands — Reading & Inspecting Files

1. **cat** — It prints the entire contents of a file straight to the
   terminal. It is good for short files, but it is impractical for anything long
   since it dumps everything at once with no scrolling control.

2. **less** — It opens a file for paging through one screen at a time.
   Lets you scroll up and down ↑ / ↓, search inside the file, and quit without
   loading the whole thing into memory — very good for large files.
   
    Space     → next page
    b         → previous page
    ↑ / ↓     → move line by line
    q         → quit

3. **head** — Shows the first 10 lines of a file by default. Useful for
   quickly checking a file's structure or header without opening the
   whole thing.

4. **head -n** — Same as head, but lets you specify exactly how many
   lines to show (e.g. `head -n 15` shows the first 15 lines).

5. **tail** — Shows the last 10 lines of a file by default. It is good for
   checking the most recent entries in something like a log file.

6. **tail -f** — Follows a file in real time, printing new lines as
   they're written. This is what one use to watch a log file update
   live while a process is running.

7. **wc** — Word count. It reports the number of lines, words, and bytes
   in a file all at once.

8. **wc -l** — Same as wc, but shows only the line count. Quick way to
   check how many entries are in a log or list.

9. **file** — Identifies what type of file something actually is (text,
   binary, script, image, etc.) by inspecting its content, not just its
   extension.

10. **stat** — Shows detailed metadata about a file: size, permissions,
    owner, and timestamps for when it was created, modified, and last
    accessed.
