# Day 19 Commands — Vim Navigation & Search/Replace

1. **gg / G** — gg jumps to the very first line of the file; G (capital)
   jumps to the very last line. Fast way to get to either end of a large
   file instantly.

2. **:10 (go to line)** — Jumps directly to a specific line number
   (line 10 in this case), instead of scrolling manually to find it.

3. **/ (search forward)** — Searches for a pattern starting from the
   cursor's position and moving forward through the file.

4. **? (search backward)** — Same as /, but searches backward from the
   cursor's current position instead of forward.

5. **n / N** — After a search, n jumps to the next match in the same
   direction as the search; N jumps to the previous match, reversing
   direction.

6. **:%s/old/new/g** — Substitutes every occurrence of "old" with "new"
   across the entire file. The % applies it to all lines, and the g
   flag ensures every match on each line is replaced, not just the
   first one.

7. **dw** — Deletes from the cursor's current position to the start of
   the next word, without touching the rest of the line.

8. **x** — Deletes a single character under the cursor.

9. **o / O** — o opens a new line below the current one and enters
   insert mode; O (capital) opens a new line above the current one
   instead.

10. **ZZ** — Saves the file and quits Vim in one motion, similar to :wq
    but typed without the colon.
