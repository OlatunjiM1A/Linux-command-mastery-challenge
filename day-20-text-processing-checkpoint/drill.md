# Day 20 Practice Drill

## Task
CHECKPOINT. From a raw log file, build one pipeline that filters for
'error' entries, extracts the timestamp column, sorts the results, and
removes duplicates, all in a single chained command.

## Commands run, in order

grep -i "error" sample.log | awk '{print $1, $2}' | sort | uniq
