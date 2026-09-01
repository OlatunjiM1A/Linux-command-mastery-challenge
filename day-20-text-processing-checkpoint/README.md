# Day 20: Text Processing & Pipes

## Phase 4 - Environment, Vim & Text Processing | Day 20 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
CHECKPOINT. From a raw log file, I built one pipeline that filtered for
"error" entries, extracted the timestamp column, sorted the results,
and removed duplicates — all chained together in a single command.

## What surprised me
I didn't expect how naturally each command's output could feed straight
into the next one's input. Instead of running four separate commands
and manually copying results between them, piping let me build one
continuous flow — grep filters, cut extracts, sort orders, uniq
dedupes — each stage only doing one small job.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-19-vim-search-replace/
Next day: ../day-21-viewing-processes/
