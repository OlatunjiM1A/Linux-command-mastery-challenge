# Day 19: Vim Navigation & Search/Replace

## Phase 4 - Environment, Vim & Text Processing | Day 19 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
In a 50-line config file, I jumped straight to line 10, searched for a
keyword, jumped between all the matches, then replaced every occurrence
of one word with another across the whole file in a single command.

## What surprised me
I didn't expect :%s/old/new/g to replace across the entire file in one
shot — I was expecting to need a loop or repeat the search-and-replace
manually for each match. The % at the start is what tells vim "apply
this to every line," not just the current one.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-18-vim-fundamentals/
Next day: ../day-20-text-processing-checkpoint/
