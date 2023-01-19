# ADD FILE TO PRJ AND PULL #
Windows PowerShell
(C) Корпорация Майкрософт, 2012. Все права защищены.

PS C:\Python\GHUB\DZ> git clone https://github.com/KosachevAN/HomeworkThird.git
Cloning into 'HomeworkThird'...
error: could not lock config file C:/Python/GHUB/DZ/HomeworkThird/.git/config: Permission denied
fatal: could not set 'remote.origin.fetch' to '+refs/heads/*:refs/remotes/origin/*'
PS C:\Python\GHUB\DZ> git status
fatal: not a git repository (or any of the parent directories): .git
PS C:\Python\GHUB\DZ> git clone https://github.com/KosachevAN/HomeworkThird.git
Cloning into 'HomeworkThird'...
remote: Enumerating objects: 23, done.
remote: Counting objects: 100% (23/23), done.
remote: Compressing objects: 100% (18/18), done.
remote: Total 23 (delta 1), reused 20 (delta 1), pack-reused 0Receiving objects:   4% (1/23)
Receiving objects: 100% (23/23), 9.16 KiB | 625.00 KiB/s, done.
Resolving deltas: 100% (1/1), done.
PS C:\Python\GHUB\DZ> git branch dzpull
fatal: not a git repository (or any of the parent directories): .git
PS C:\Python\GHUB\DZ> cd HomeworkThird
PS C:\Python\GHUB\DZ\HomeworkThird> git branch dzpull3
PS C:\Python\GHUB\DZ\HomeworkThird> git checkout dzpull3
Switched to branch 'dzpull3'
PS C:\Python\GHUB\DZ\HomeworkThird> git branch
* dzpull3
  main
PS C:\Python\GHUB\DZ\HomeworkThird> git add addfiledz3.md
PS C:\Python\GHUB\DZ\HomeworkThird> git commit 'ADD FILE DZ3'
error: pathspec 'ADD FILE DZ3' did not match any file(s) known to git
PS C:\Python\GHUB\DZ\HomeworkThird> git commit -m 'ADD FILE DZ3'
[dzpull3 fbd6c80] ADD FILE DZ3
 1 file changed, 1 insertion(+)
 create mode 100644 addfiledz3.md
PS C:\Python\GHUB\DZ\HomeworkThird> git push
fatal: The current branch dzpull3 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dzpull3

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Python\GHUB\DZ\HomeworkThird> git push --set-upstream origin dzpull3
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 347 bytes | 115.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dzpull3' on GitHub by visiting:
remote:      https://github.com/KosachevAN/HomeworkThird/pull/new/dzpull3
remote:
To https://github.com/KosachevAN/HomeworkThird.git
 * [new branch]      dzpull3 -> dzpull3
branch 'dzpull3' set up to track 'origin/dzpull3'.
PS C:\Python\GHUB\DZ\HomeworkThird>
