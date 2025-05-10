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
