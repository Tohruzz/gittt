git courseeeeeeeeeeeee
PS D:\gittt> git config --global user.name 'Tohruzz'
PS D:\gittt> git config --global user.email 'reyorijinrojin@gmail.com'
PS D:\gittt> git config user.name
Tohruzz
PS D:\gittt> git config user.email
reyorijinrojin@gmail.com
PS D:\gittt> git config --global init.defaultBranch main
PS D:\gittt> git init
Initialized empty Git repository in D:/gittt/.git/
PS D:\gittt> git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        readme.md
        script.js

nothing added to commit but untracked files present (use "git add" to track)
PS D:\gittt> git add readme.md
PS D:\gittt> git commit -m 'readme'
[main (root-commit) 1e9a2f1] readme
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md
PS D:\gittt> git log
commit 1e9a2f1b81d432154636c705bca8254d2301820b (HEAD -> main)
Author: Tohruzz <reyorijinrojin@gmail.com>
Date:   Thu Sep 10 21:40:29 2026 +0530

    readme
PS D:\gittt> git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        script.js

nothing added to commit but untracked files present (use "git add" to track)
PS D:\gittt> git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add
PS D:\gittt> git add .
PS D:\gittt> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   index.html
        new file:   script.js

PS D:\gittt> git commit -m 'initial commit'
[main e29560d] initial commit
 2 files changed, 12 insertions(+)
 create mode 100644 index.html
 create mode 100644 script.js
PS D:\gittt> git status                    
On branch main
nothing to commit, working tree clean
PS D:\gittt> git log
commit e29560db222bc0d927fc4ca12aa34130ab5431f3 (HEAD -> main)
Author: Tohruzz <reyorijinrojin@gmail.com>
Date:   Thu Sep 10 22:05:50 2026 +0530

    initial commit

commit 1e9a2f1b81d432154636c705bca8254d2301820b
Author: Tohruzz <reyorijinrojin@gmail.com>
Date:   Thu Sep 10 21:40:29 2026 +0530

    readme
PS D:\gittt> git checkout 1e9a2f1b81d432154636c705bca8254d2301820b
Note: switching to '1e9a2f1b81d432154636c705bca8254d2301820b'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 1e9a2f1 readme
PS D:\gittt> git checkout main
Previous HEAD position was 1e9a2f1 readme
Switched to branch 'main'
PS D:\gittt> git checkout 1e9a2f1b81d432154636c705bca8254d2301820b
Note: switching to '1e9a2f1b81d432154636c705bca8254d2301820b'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 1e9a2f1 readme
PS D:\gittt> git checkout main                                    
M       readme.md
Previous HEAD position was 1e9a2f1 readme
Switched to branch 'main'
PS D:\gittt> git checkout -f  main