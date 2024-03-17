---
mindmap-plugin: basic
tags:
  - CompSci/tool/git/command
---
# git merge
### Description:
- Join two or more development histories together
### git merge:
- git merge 
	- `[-n]`
	- `[--stat] `
	- `[--no-commit] `
	- `[--squash] `
	- `[--[no-]edit]`
	- `[--no-verify] `
	- `[-s <strategy>] `
	- `[-X <strategy-option>] [-S[<keyid>]]`
	- `[--[no-]allow-unrelated-histories]`
	- `[--[no-]rerere-autoupdate] [-m <msg>] [-F <file>]`
	- `[--into-name <branch>] [<commit>…​]`
- git merge (--continue | --abort | --quit)
### Pre-merge checks:
- _git pull_ and _git merge_ will stop without doing anything when local uncommitted changes overlap with files that _git pull_/_git merge_may need to update.
- To avoid recording unrelated changes in the merge commit, _git pull_ and _git merge_ will also abort if there are any changes registered in the index relative to the `HEAD` commit. 
	- (Special narrow exceptions to this rule may exist depending on which merge strategy is in use, but generally, the index must match HEAD.)
- If all named commits are already ancestors of `HEAD`, _git merge_ will exit early with the message "Already up to date."
### Fast-forward merge:
- Often the current branch head is an ancestor of the named commit. 
- This is the most common case especially when invoked from _git pull_: you are tracking an upstream repository, you have committed no local changes, and now you want to update to a newer upstream revision. 
- In this case, a new commit is not needed to store the combined history;
	- instead, the `HEAD` (along with the index) is updated to point at the named commit, without creating an extra merge commit.
- This behavior can be suppressed with the `--no-ff` option.

### True merge
### Merging tags
### How conflicts are represented:
### How to resolve conflicts:
### Merge strategies:
### Configuration