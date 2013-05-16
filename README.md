git-submodule-move
==================

A script for quickly moving a git submodule within a repo

This command is based upon the stackoverflow answer
[here](http://stackoverflow.com/a/13942859).  Basically, it re-clones
the repo (using the existing repo as the origin), updates the internal
git references, and cleans things up as necessary.

It works for me, but your mileage may vary.  No warranty implied or
given.

## Usage:

Put the script in your `PATH`.  Go to your repository's root directory.

Now, let's say you want to move a submodule at `bar` to `foo/bar`.
Simply issue:

    % git-submodule-move bar foo/bar
    
See the original post for details.  Note that this script will
automatically commit the changes and there is no error handling.

