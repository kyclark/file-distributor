# File Distributor

Given an input file of file sizes (in bytes) and file names, e.g.:

    10 foo
    20 bar
    50 baz
    60 blip

This script will place files into groups that have similar sizes, e.g.:

    1   baz
    1   foo
    2   blip
    3   bar

This is useful for distributing data sets to compute nodes so that each node
gets a similar load and therefore all jobs will complete in relatively the
same amount of time (all other things being equal, of course).
