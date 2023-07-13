# Software engineering

## Debugging

### What techniques can you use while debugging a program in Python?

> We can use the ``print()`` function to print to the console, but the best is to set breakpoint and run the IDE's
> debugger.

### What does step over, step into and step out mean, while using the debugger?

> ``Step over`` jumps to the next function call. ``Step into`` runs the function line by line. ``Step out`` exits the
> current function and jumps to the next.

### How can you start to debug a program from a certain line using the debugger?

> I set a breakpoint to the line I want to run the debugger from.

## Version control

### What are the advantages of using a version control system?

> We can keep track of the changes we and/or our teammates made in the codebase

### What is the difference between the working directory, the staging area and the repository in git?

> Working directory is our local project directory, where we actively work on the code. Staging area is, where the file
> we want to include in the next commit are staged using the ``git add`` command. A repository is a storage for our code
> history

### What are remote repositories in git?

> Remote repositories are stored on a remote server, where anyone on a team (or anyone around the world, if public) can
> reach and modify it through pull requests

### Why does a merge conflict occur?

> Merge conflicts occur, when multiple people changes the same file and without knowing and pushing both to the remote
> repository git can't handle the commit smoothly

### Through what series of commands could you put a new file into a remote repository connected to your existing local repository?

> ``git add`` > ``git commit`` > ``git push``

### What does it mean atomic commits and descriptive commit messages?

> With atomic commits we mean, that each commit should be about one change only with a descriptive commit message,
> which defines the change that commit introduced to the code base

### What’s the difference between git and GitHub?

> ``Git`` is a version control system, while ``GitHub`` is a repository hosting service