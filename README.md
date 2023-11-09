<div>

<table style="width:100%;height: auto;">

  <tr colspan="2">
  <h1 style="text-align: center;"> GIT CHEAT SHEET </h1>
  <p>
Git is the free and open source distributed version control system that's responsible for everything GitHub related that happens locally on your computer. This cheat sheet features the most important and commonly used Git commands for easy reference.
</p>
    </tr>
  <tr style="width:50%;height: auto;position: absolute;left:0">
  <td>

## SETUP

<div style="">
<p >
Configuring user information used across all local repositories

**git config --global user.name “[firstname lastname]”**<br/>
_set a name that is identifiable for credit when review version history_

**git config --global user.email “[valid-email]”**<br/>
_set an email address that will be associated with each history marker_

**git config --global color.ui auto**<br/>
_set automatic command line coloring for Git for easy reviewing_

</p>
</div>

## SETUP & INIT

<p>
Configuring user information, initializing and cloning repositories

**git init**<br/>
_initialize an existing directory as a Git repository_

**git clone [url]**<br/>
_retrieve an entire repository from a hosted location via URL_

</p>

## INSPECT & COMPARE

Examining logs, diffs and object information

**git log**<br/>
_show the commit history for the currently active branch_

**git log branchB..branchA**<br/>
_show the commits on branchA that are not on branchB_

**git log --follow [file]**<br/>
_show the commits that changed file, even across renames_

**git diff branchB...branchA**<br/>
_show the diff of what is in branchA that is not in branchB_

**git show [SHA]**<br/>
_show any object in Git in human-readable format_

## TRACKING PATH CHANGES

Versioning file removes and path changes

**git rm [file]**<br/>
_delete the file from project and stage the removal for commit_

**git mv [existing-path] [new-path]**<br/>
_change an existing file path and stage the move_

**git log --stat -M**<br/>
_show all commit logs with indication of any paths that moved_

## IGNORING PATTERNS

Preventing unintentional staging or commiting of files

**logs/ <br/>
\*.notes <br/>
pattern\*/**

_Save a file with desired patterns as .gitignore with either direct string matches or wildcard globs._

**git config --global core excludesfile [file]**<br/>
_system wide ignore pattern for all local repositories_

</td>

  </tr>
  </tr>
  <tr style="width:50%;height: auto;position: absolute;left: 50%; right: 0">
<td>

## STAGE & SNAPSHOT

<p>
Working with snapshots and the Git staging area

**git status**<br/>
_show modified files in working directory, staged for your next commit_

**git add [file]**<br/>
_add a file as it looks now to your next commit (stage)_

**git reset [file]**<br/>
_unstage a file while retaining the changes in working directory_

**git diff**<br/>
_diff of what is changed but not staged_

**git diff --staged**<br/>
_diff of what is staged but not yet committed_

**git commit -m “[descriptive message]”**<br/>
_commit your staged content as a new commit snapshot_

</p>

## BRANCH & MERGE

<p>
Isolating work in branches, changing context, and integrating changes

**git branch**<br/>
_list your branches. a \* will appear next to the currently active branch_

**git branch [branch-name]**<br/>
_create a new branch at the current commit_

**git checkout**<br/>
_switch to another branch and check it out into your working directory_

**git merge [branch]**<br/>
_merge the specified branch’s history into the current one_

**git log**<br/>
_show all commits in the current branch’s history_

</p>

## SHARE & UPDATE

Retrieving updates from another repository and updating local repos

**git remote add [alias] [url]**<br/>
_add a git URL as an alias_

**git fetch [alias]**<br/>
_fetch down all the branches from that Git remote_

**git merge [alias]/[branch]**<br/>
_merge a remote branch into your current branch to bring it up to date_

**git push [alias] [branch]**<br/>
_Transmit local branch commits to the remote repository branch_

**git pull**<br/>
_fetch and merge any commits from the tracking remote branch_

## REWRITE HISTORY

Rewriting branches, updating commits and clearing history

**git rebase [branch]**<br/>
_apply any commits of current branch ahead of specified one_

**git reset --hard [commit]**<br/>
_clear staging area, rewrite working tree from specified commit_

## TEMPORARY COMMITS

Temporarily store modified, tracked files in order to change branches

**git stash**<br/>
_Save modified and staged changes_

**git stash list**<br/>
_list stack-order of stashed file changes_

**git stash pop**<br/>
_write working from top of stash stack_

**git stash drop**<br/>
_discard the changes from top of stash stack_

</td>
  </tr>

</table>

</div>
