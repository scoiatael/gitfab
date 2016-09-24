# gitfab
Git wrapper for common tasks

## Idea
How does you common Git workflow look like? Mine is:
* Have a repository cloned / initialized - with single origin remote to push to / pull from.
* Have a single branch on origin repository I want to track and issue PRs against (usually master, sometimes develop).
* Create a new branch - either feature / bugfix / refactor (usually named like <nick>/<type>/<short-desc>).
* Hack on my new branch.
* Occasionally run tests / linters - especially before commiting changes!
* Commit early, push to remote repository daily.
* Occasionally rebase against upstream branch.
* When finished, either issue a PR or merge manually.
* Occasionally remove dead branches (i.e. all that are merged to upstream one, or even all that exist in upstream repo).
* Understand what happens in repository by looking at a cool graph of all commits in all branches.
* Sometimes jump around to particular commits from the graph.

## Goal
Git, of course, being a neat tool allows to do this via its porcelain commands - but there's a loot of room for improvement! So the goals are:
* Optimize for flow described above
* Focus on CLI interface, with assumption of having a decent terminal emulator and ncurses - pretty much like [Fish shell](https://fishshell.com/) does.
* Allow adding more interfaces (GUI even) by having clean client - server architecture.

## TODO
- [ ] create repository structure for go
- [ ] create simple integration tests (assume binary is called `gfb`)
- [ ] start hacking!
