# my-git-hooks
Git hook scripts that I want to reuse across projects.   Generally very personal to my own workflows.

## Hooks

### bin/post-commit-gitlog-tracker

Use case is to keep track of all my commits over many machines.  This will generate a two line log entry for a text gitlog file.
The first line identifies when and where the work was done.   The second line summarises the commit.
The script will look for a GITLOG variable, but then default to $HOME/.gitlog otherwise.

Intended use is to have a repository that is generally checked out in the same location on all machines, to which these log
entries be added.

TODO: support scripts for searching this repository.

CAVEAT: the GITLOG should not be public as the metadata recorded can be confidential to a project/client (username, hostname, project data).


## Oddities

Initially, I tried to create a project entry with a .git folder.   These turn out to be banned from being added to git.   Disappointing.


Adam Stephen 2019-11-13
