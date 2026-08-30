# Day 19 Practice Drill

## Task
In a 50-line config file, jump straight to line 10, search for a
keyword, jump between all matches, then replace every occurrence of one
word with another across the whole file.

## Commands run, in order

vim config-sample.txt

:10

/localhost

n

n

:%s/localhost/127.0.0.1/g

:wq
