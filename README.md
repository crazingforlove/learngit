# learngit
exists before push



        readme.txt.bak

F:\GitHub\repository\learngit\text [master +0 ~1 -0 | +1 ~0 -0 !]> git commit -m "change reademe.txt"
[master 81c3549] change reademe.txt
 1 file changed, 1 insertion(+), 1 deletion(-)
F:\GitHub\repository\learngit\text [master +1 ~0 -0 !]>
F:\GitHub\repository\learngit\text [master +1 ~0 -0 !]> git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        readme.txt.bak

nothing added to commit but untracked files present (use "git add" to track)
F:\GitHub\repository\learngit\text [master +1 ~0 -0 !]>
F:\GitHub\repository\learngit\text [master]> git status
On branch master
nothing to commit, working directory clean
F:\GitHub\repository\learngit\text [master]>
F:\GitHub\repository\learngit\text [master]>
F:\GitHub\repository\learngit\text [master]> git add readme.txt
F:\GitHub\repository\learngit\text [master +0 ~1 -0 | +1 ~0 -0 !]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        readme.txt.bak

F:\GitHub\repository\learngit\text [master +0 ~1 -0 | +1 ~0 -0 !]> git add *.bak
F:\GitHub\repository\learngit\text [master +1 ~1 -0]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0]> rm *.bak
F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> cat .\readme.txt.bak
Get-Content : 找不到路径“F:\GitHub\repository\learngit\text\readme.txt.bak”，因为该路径不存在。
所在位置 行:1 字符: 4
+ cat <<<<  .\readme.txt.bak
    + CategoryInfo          : ObjectNotFound: (F:\GitHub\repos...\readme.txt.bak:String) [Get-Content], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Commands.GetContentCommand

F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> git checkout --readme.txt.bak
error: unknown option `readme.txt.bak'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -q, --quiet           suppress progress reporting
    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --detach              detach the HEAD at named commit
    -t, --track           set upstream info for new branch
    --orphan <new-branch>
                          new unparented branch
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unmerged files
    -f, --force           force checkout (throw away local modifications)
    -m, --merge           perform a 3-way merge with the new branch
    --overwrite-ignore    update ignored files (default)
    --conflict <style>    conflict style (merge or diff3)
    -p, --patch           select hunks interactively
    --ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --ignore-other-worktrees
                          do not check if another worktree is holding the given ref

F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> git checkout -- readme.txt.bak
F:\GitHub\repository\learngit\text [master +1 ~1 -0]> ls


    目录: F:\GitHub\repository\learngit\text


Mode                LastWriteTime     Length Name
----                -------------     ------ ----
-a---          2016/9/8     14:23          0 file1.txt
-a---          2016/9/8     14:23          0 file2.txt
-a---          2016/9/8     14:23          0 file3.txt
-a---          2016/9/8     14:44         93 readme.txt
-a---          2016/9/8     14:54         67 readme.txt.bak


F:\GitHub\repository\learngit\text [master +1 ~1 -0]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0]> git rm .\readme.txt.bak
error: the following file has changes staged in the index:
    text/readme.txt.bak
(use --cached to keep the file, or -f to force removal)
F:\GitHub\repository\learngit\text [master +1 ~1 -0]> git rm readme.txt.bak
error: the following file has changes staged in the index:
    text/readme.txt.bak
(use --cached to keep the file, or -f to force removal)
F:\GitHub\repository\learngit\text [master +1 ~1 -0]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0]> rm readme.txt.bak
F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> git checkout -- readme.txt.bak
F:\GitHub\repository\learngit\text [master +1 ~1 -0]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0]> rm *.bak
F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> ls


    目录: F:\GitHub\repository\learngit\text


Mode                LastWriteTime     Length Name
----                -------------     ------ ----
-a---          2016/9/8     14:23          0 file1.txt
-a---          2016/9/8     14:23          0 file2.txt
-a---          2016/9/8     14:23          0 file3.txt
-a---          2016/9/8     14:44         93 readme.txt


F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt
        new file:   readme.txt.bak

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    readme.txt.bak

F:\GitHub\repository\learngit\text [master +1 ~1 -0 | +0 ~0 -1]> git rm readme.txt.bak
rm 'text/readme.txt.bak'
F:\GitHub\repository\learngit\text [master +0 ~1 -0]>
F:\GitHub\repository\learngit\text [master +0 ~1 -0]>
F:\GitHub\repository\learngit\text [master +0 ~1 -0]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt

F:\GitHub\repository\learngit\text [master +0 ~1 -0]> git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>

F:\GitHub\repository\learngit\text [master +0 ~1 -0]> cd ..
F:\GitHub\repository\learngit [master +0 ~1 -0]> git remote add learngit
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=<push|fetch>]
                          set up remote as a mirror to push to or fetch from

F:\GitHub\repository\learngit [master +0 ~1 -0]> git remote add learngit https://github.com/crazingforlove/learngit.git
F:\GitHub\repository\learngit [master +0 ~1 -0]> git push learngit
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream learngit master

F:\GitHub\repository\learngit [master +0 ~1 -0]> git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   text/readme.txt

F:\GitHub\repository\learngit [master +0 ~1 -0]> git remote add learngit https://github.com/crazingforlove/learngit.git  -m
error: switch `m' requires a value
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=<push|fetch>]
                          set up remote as a mirror to push to or fetch from

F:\GitHub\repository\learngit [master +0 ~1 -0]> git remote add learngit https://github.com/crazingforlove/learngit.git  -m master
fatal: remote learngit already exists.
F:\GitHub\repository\learngit [master +0 ~1 -0]> git push learngit
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream learngit master

F:\GitHub\repository\learngit [master +0 ~1 -0]> git push --set-upstream learngit master
remote: Repository not found.
fatal: repository 'https://github.com/crazingforlove/learngit.git/' not found
F:\GitHub\repository\learngit [master +0 ~1 -0]>
