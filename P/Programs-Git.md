# Programs - Git

## How to Create Comments in .gitignore

```
#
```

Source

* Comments in .gitignore?
  * https://stackoverflow.com/questions/8865848/comments-in-gitignore

## ...

```
git add *.c
```

Source

* Is there a way to just commit one file type extension from a folder?
  * https://stackoverflow.com/questions/26682744/is-there-a-way-to-just-commit-one-file-type-extension-from-a-folder

## ...

Source

```
git diff --name-only --cached
```

* Git list of staged files
  * https://stackoverflow.com/questions/33610682/git-list-of-staged-files

## ...

Switch from HTTPS to SSH.

```
$ git remote add origin git@github.com:username/project.git
```

## ...

Adjust Git/HTTPS buffer.

```
git config http.postBuffer 524288000
```

A high-latency network?

Source

* Git, fatal: The remote end hung up unexpectedly
  * https://stackoverflow.com/questions/15240815/git-fatal-the-remote-end-hung-up-unexpectedly

## ...

> If you get error 413, then the issue doesn't lie with git but with your web server. It's your web server that is blocking big upload files.

Modify server or switch to SSH.

Source

* Github Push Error: RPC failed; result=22, HTTP code = 413
  * https://stackoverflow.com/questions/7489813/github-push-error-rpc-failed-result-22-http-code-413

## ...

> This turned out to be no problem at all. I simply had to wait until the upload was complete. I had added several large files and there is not a progress indicator. Maybe someone else will find this helpful.

Source

* git push hangs after Total line
  * https://stackoverflow.com/questions/15843937/git-push-hangs-after-total-line

## ...

```
git config --global http.postBuffer 524288000
```

Source

* Git hangs while writing objects
  * https://stackoverflow.com/questions/6887228/git-hangs-while-writing-objects

## ...

```
$ git push <remote> <branch>
```

Source

* How To Push Git Branch To Remote
  * https://devconnected.com/how-to-push-git-branch-to-remote/

## How to Delete a Commit

Delete the most recent commit, keeping the work you've done:

```
git reset --soft HEAD~1
```

Delete the most recent commit, destroying the work you've done:

```
git reset --hard HEAD~1
```

Source

* How do I delete unpushed git commits?
  * https://stackoverflow.com/questions/3197413/how-do-i-delete-unpushed-git-commits
