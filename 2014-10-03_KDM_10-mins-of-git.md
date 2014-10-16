Git
===

Git is a way of keeping track of differences in your "thing".


What's Your "thing"
-------------------

Git can be used to track differences through time in any kind of file. However,
it works best for text files.

What have I used git to track:

  - Code: All my code is in git, and it makes life so much easier.
  - Analysis scripts: Normally the first thing I do to a dataset is `git init`.
    Then, I keep track of what I run using git, adding only the scripts.
  - Presentations: I'll normally use LaTeX & Brewer to write my presentations,
    and git keeps me from making stupid mistakes. [GitHub](https://github.com)
    is a good way to share them, too.
  - Thesis: I wrote my thesis in latex, tracking the changes with git. I even
    got comments as git pull requests from Justin...
  - Papers: Ditto to the last two points
  - Documentation: Most code that has documentation keeps it in the same git
    repo as the actual code.


How to use git
--------


So, there are many git commands.

```
mkdir git_repo
cd git_repo
git init # makes a repo
```

Now you have an actual repo, you better do some actual work. To "commit" or
save it, use `git commit`, which is the time resolution of git. You make a
commit when you're happy with whatever you're adding, or at least when it is
finished for the day/week

```
git add . # adds everything in the current folder to the git repo.
git commit # makes the commit
```

You can use `git add --patch` to modify the commit on the fly, which is
**REALLY** helpful!
