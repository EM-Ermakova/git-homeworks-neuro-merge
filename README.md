#log of task

## link for [forked rep] (https://github.com/EM-Ermakova/git-homeworks-neuro-merge.git)
 
Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub
$ git clone git@github.com:EM-Ermakova/git-homeworks-neuro-merge.git
Cloning into 'git-homeworks-neuro-merge'...
remote: Enumerating objects: 26, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 26 (delta 3), reused 2 (delta 2), pack-reused 18 (from 1)
Receiving objects: 100% (26/26), 4.59 MiB | 804.00 KiB/s, done.
Resolving deltas: 100% (4/4), done.

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub
$ git branch
fatal: not a git repository (or any of the parent directories): .git

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub
$ cd git
Git инструкция.docx        git-homeworks-neuro-merge/

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub
$ cd git-homeworks-neuro-merge/

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git branch
* main

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git log --oneline --all
6aa1c0b (HEAD -> main, origin/main, origin/HEAD) Merge branch 'feature/copywriting'
461fac5 (origin/feature/earlyorder) Early Order
b775bae (origin/feature/copywriting) Rewriting
5b415cb Первоначальная версия

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git merge origin/feature/earlyorder
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main|MERGING)
$ git add -a -m "merge branches"
error: unknown switch `a'
usage: git add [<options>] [--] <pathspec>...

    -n, --[no-]dry-run    dry run
    -v, --[no-]verbose    be verbose

    -i, --[no-]interactive
                          interactive picking
    -p, --[no-]patch      select hunks interactively
    -e, --[no-]edit       edit current diff and apply
    -f, --[no-]force      allow adding otherwise ignored files
    -u, --[no-]update     update tracked files
    --[no-]renormalize    renormalize EOL of tracked files (implies -u)
    -N, --[no-]intent-to-add
                          record only the fact that the path will be added later
    -A, --[no-]all        add changes from all tracked and untracked files
    --[no-]ignore-removal ignore paths removed in the working tree (same as --no-all)
    --[no-]refresh        don't add, only refresh the index
    --[no-]ignore-errors  just skip files which cannot be added because of errors
    --[no-]ignore-missing check if - even missing - files are ignored in dry run
    --[no-]sparse         allow updating entries outside of the sparse-checkout cone
    --[no-]chmod (+|-)x   override the executable bit of the listed files
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character


Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main|MERGING)
$ git commit -a -m "merge branches"
[main 5e0b2b8] merge branches

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git log --oneline --all
5e0b2b8 (HEAD -> main) merge branches
6aa1c0b (origin/main, origin/HEAD) Merge branch 'feature/copywriting'
461fac5 (origin/feature/earlyorder) Early Order
b775bae (origin/feature/copywriting) Rewriting
5b415cb Первоначальная версия

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git push -u origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 619 bytes | 619.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:EM-Ermakova/git-homeworks-neuro-merge.git
   6aa1c0b..5e0b2b8  main -> main
branch 'main' set up to track 'origin/main'.

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git remote -v
origin  git@github.com:EM-Ermakova/git-homeworks-neuro-merge.git (fetch)
origin  git@github.com:EM-Ermakova/git-homeworks-neuro-merge.git (push)

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git remote remove origin

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git remote -v

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git remote add origin git@github.com:EM-Ermakova/neuro-merge-task3.git

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git remote -v
origin  git@github.com:EM-Ermakova/neuro-merge-task3.git (fetch)
origin  git@github.com:EM-Ermakova/neuro-merge-task3.git (push)

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git push -u origin main
To github.com:EM-Ermakova/neuro-merge-task3.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'github.com:EM-Ermakova/neuro-merge-task3.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git pull
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 863 bytes | 172.00 KiB/s, done.
From github.com:EM-Ermakova/neuro-merge-task3
 * [new branch]      main       -> origin/main
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main


Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git push -u origin main
To github.com:EM-Ermakova/neuro-merge-task3.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'github.com:EM-Ermakova/neuro-merge-task3.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Admin@WIN-MP25Z1BJ MINGW64 ~/Desktop/Курс СА/GitHub/git-homeworks-neuro-merge (main)
$ git push --force
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.
