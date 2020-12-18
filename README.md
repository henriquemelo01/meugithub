# Git Guide

<h1> Mainly git commans: </h1>

- Create repository:
  git init

- Add files from directory in stage area. Stage area is a local where we storage the files that can be commited.

touch <file> // create a file using terminal
git add . // add all files from directory
git add <file> // add specific file
git add \*.<extension>

- Commit: Send files from Stage Area to Local Repository
  git commit -m "message that describe the file change"

Following this steps we create a local repository.

- Show git infos:
  git status // with this command its possible see which of these files has not been added to the stage area and the files that we modify.

- Show commits: https://git-scm.com/docs/git-log
  git log

- See what are the modifies we did before add the files in stage area:
  git diff

- See what are the modifies that we did when we add the file in stage area:
  git --cache or git --staged

- Remove files:
  git rm <file> or delete file manualy then add file in Stage Area

- Rename files:
  git mv <file renamed> <new file name> // mv: move, when the file is renamed, we change his address (path)

- Move the files:
  git mv <file> <folder>/<file>

- Restore changes
  git restore <fileChanged>

- Restore changes from files that we add in Stage Area:
  git restore --staged <fileChanged>

- Restore all changes:
  git restore . or git restore --staged .

- Correct the last commit
  git commit --amend -m "new msg"

- Restore files:
  git checkout <commitHash>--<file>

- Revert files (Return to a set point)  
  git revert HEAD~5 // return to last commit (HEAD) - 5
  git revert commitHash

- Create a new "time line":
  git branch <nameBranch>

- Change branch:
  git checkout <name>
  Ex: git checkout master // mainly "time line"

- Log Branchs:
  git branch

Obs: Terminal: :q = quit
