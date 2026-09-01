# Day 20 Commands — Text Processing & Pipes

1. **grep** — Searches text for lines matching a pattern and prints
   only those lines. The core tool for filtering large files down to
   what actually matters.

2. **grep -r** — Searches recursively through every file in a directory
   and its subdirectories, instead of just one file.

3. **grep -i** — Performs a case-insensitive search, matching a pattern
   regardless of uppercase or lowercase letters.

4. **sort** — Sorts lines of text alphabetically by default. Often used
   right after grep to organize filtered results.

5. **sort -n** — Sorts lines numerically instead of alphabetically,
   which matters because alphabetical sort treats "10" as coming before
   "2".

6. **uniq** — Removes consecutive duplicate lines from sorted input.
   Only works correctly on data that's already sorted, since it only
   compares neighboring lines.

7. **cut -d',' -f** — Extracts a specific column from delimited text
   (e.g. CSV data), where -d sets the delimiter character and -f
   chooses which field/column to extract.

8. **awk '{print $1}'** — A more flexible text-processing tool that can
   print specific fields from each line; $1 refers to the first
   whitespace-separated field.

9. **sed 's/old/new/g'** — Stream editor that finds and replaces text
   directly from the command line, without opening a file in an editor
   like vim.

10. **pipe chains (|)** — Connects the output of one command directly
    into the input of the next, letting you chain several simple tools
    together into one combined operation.
