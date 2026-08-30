# Day 18 Commands — Vim Fundamentals

1. **vim <file>** — Opens a file in the Vim text editor, creating it if
   it doesn't already exist. Opens in command mode by default, not
   ready for typing right away.

2. **i (insert mode)** — Switches from command mode into insert mode,
   allowing you to actually type and edit text in the file.

3. **Esc (command mode)** — Exits insert mode and returns to command
   mode, where keystrokes are interpreted as commands rather than text
   to type.

4. **:w** — Writes (saves) the current file to disk without exiting
   Vim. Must be run from command mode, not insert mode.

5. **:wq / :x** — Writes the file and quits Vim in one step. :x is
   slightly more efficient since it only writes if changes were
   actually made.

6. **:q!** — Quits Vim without saving, discarding any unsaved changes.
   The ! forces the quit even though normally Vim would warn about
   unsaved work.

7. **dd** — Deletes (cuts) the entire current line the cursor is on,
   also storing it in Vim's internal register for pasting later.

8. **yy / p** — yy copies (yanks) the current line without deleting it;
   p pastes whatever was last yanked or deleted, right below the
   cursor's current line.

9. **:q** — Quits Vim, but only if there are no unsaved changes. Vim
   will refuse and warn you if the file has been modified.

10. **u / Ctrl+r** — u undoes the last change made to the file; Ctrl+r
    redoes a change that was just undone, reversing the undo.
