# git authorship

**Usage:** `git authorship [<revision>] [-- <paths...>]`

Summarizes authorship of a repository by the current number of
lines.

This is a more fine-grained version of `git shortlog -ns`, which
counts commits instead of lines.

Provide a revision to use a specific point-in-time instead of the
current HEAD.  Provide paths to limit to a set of files or
directories.
