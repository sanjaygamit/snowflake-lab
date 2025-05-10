# user settings

(base) SanjaykumarsAir:~ sanjaykumarshantilal$ git config --global user.name "sanjay gamit"
(base) SanjaykumarsAir:~ sanjaykumarshantilal$ git config --global user.email "sanjugamit@gmail.com"
(base) SanjaykumarsAir:~ sanjaykumarshantilal$ git config --list

# Clone and Status

clone - Cloning a repository on our local machine.
git clone <some link>

status - display the status of the code.
git status

github % git clone https://github.com/sanjaygamit/snowflake-lab.git

ls -a -- to show hidden files.
git status --
On branch main
Your branch is up to date with 'origin/main'.

after modified file. process 1. add 2. commit

1. untracked (New files that git does't yet track.)
2. Modified (changed)
3. staged (file is ready to be commited)
4. unmodified (unchanged)

Add & Commit

add - adds new or changed files in your working directory to the Git staging area.
git add <file name>

commit - it is the record of change
git commit -m "Some message"
ex : git add README.md
git commit -m "file appended 10/5"

Push Command
push - upload local repo content to remote repo
git push origin main

# Init Command

init - used to create a new git repo
git init
git remote add origin <-link->
git remote-v (to verigy remote)
git branch -M main (to rename branch)
git push origin main
(base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git init
Initialized empty Git repository in /Users/sanjaykumarshantilal/Documents/github/LocalRepo/.git/
(base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % ls -a
. .. .git
(base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git status
On branch master

        No commits yet

        Untracked files:
        (use "git add <file>..." to include in what will be committed)

                index.html
                style.css

        nothing added to commit but untracked files present (use "git add" to track)

(base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git commit -m "Add Initial Files"
[master (root-commit) f811a09] Add Initial Files
2 files changed, 4 insertions(+)
create mode 100644 index.html
create mode 100644 style.css
(base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git status
On branch master
nothing to commit, working tree clean
(base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % get remote add origin https://github.com/sanjaygamit/localrepo.git
zsh: command not found: get
(base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git remote add origin https://github.com/sanjaygamit/localrepo.git
(base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git remote -v
origin https://github.com/sanjaygamit/localrepo.git (fetch)
origin https://github.com/sanjaygamit/localrepo.git (push)
(base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git branch

- master
  (base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git branch -M main
  (base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git branch
- main
  (base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo % git push origin main
  Counting objects: 4, done.
  Delta compression using up to 8 threads.
  Compressing objects: 100% (2/2), done.
  Writing objects: 100% (4/4), 310 bytes | 310.00 KiB/s, done.
  Total 4 (delta 0), reused 0 (delta 0)
  To https://github.com/sanjaygamit/localrepo.git
- [new branch] main -> main
  (base) sanjaykumarshantilal@SanjaykumarsAir LocalRepo %
