# git authorship

**Usage:** `git authorship [<options>] [<revision>] [-- <paths...>]`

Summarizes authorship of a repository by the current number of
lines.

This is a more fine-grained version of `git shortlog -ns`, which
counts commits instead of lines.

Provide a revision to use a specific point-in-time instead of the
current HEAD.  Provide paths to limit to a set of files or
directories.  You may exclude certain paths by prefixing them with a
`!` (bang).  Note that paths are actually basic globs as interpreted
by `git ls-tree` and bash pattern matching.

Any options provided are passed to git blame, although only one makes sense:

    -w    ignore whitespace when tracing the origins of lines

This is useful to avoid attributing whitespace-only changes to people.

## Installation

Copy `git-authorship` into your `PATH` anywhere you'd like, or run

    make install

to copy it into `/usr/local/bin`.  You can run

    make install prefix=$HOME

to put it in `$HOME/bin`, if you'd prefer.
