---
mindmap-plugin: basic
tags:
  - CompSci/tool/git
---
# git

### Description:
- Version control
### Git storage places:
1. Stash
	- A place to hide modifications while you work on something else.
2. Workspace
	- Also called 'working copy', 'working tree' or just 'checkout'
	- Local checkout of your code. 
	- It's any directory on your filesystem that has a repository associated with it (typically indicated by the presence of a sub-directory within it named `.git`). 
	- It includes all the files and sub-directories in that directory
3. Index
	- A staging area for file changes to commit. 
	- Before you “commit” (or checkin) files, you need to first add them to the index. 
	- This is also called "current directory cache", "staging area", "cache" or "staged files
4. Local repository
	- A directory named `.git` that contains all of your necessary repository files — a Git repository skeleton. 
	- Typical branches: `main`, `master`, `feature-x`, `bugfix-y`. 
	- The local repository has exactly the same features and functionality as any other Git repository.
5. Upstream repository
	- A repository of your code to share and collaborate with other developers. 
	- It's hosted on some the Internet or a remote, eg. [[Github]]. 
	- The default name is `origin`. 
		- Typical branches here: `main`, `master`, `shared-feature-x`, `release-y`. 
		- Also called 'remote repository', or just 'remote'.
###  Git glossary
- [[git branch|Branch]]
- [[git checkout|Checkout]]
- [[Cherry-picking]]
- [[git clone|Clone]]
- [[Fetch]]
- [[Fork]]
- [[head]]
- [[git index]]
- [[Master]]
- [[Merge]]
- [[Origin]]
- [[Pull]]
- [[Pull Request]]
- [[Push]]
- [[git rebase|Rebase]]
- [[Remote]]
- [[Repository]]
- [[Stash]]
- [[Tag]]
- [[Upstream]]

### Categories:
1. [[Setup and Config]]
2. [[git branching and merging]]
3. [[Getting and Creating Projects]]
4. [[git basic snapshotting]]
5. [[Inspecting and Comparision]]
6. [[git patching]]
```
git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch <path to the file or directory>' --prune-empty --tag-name-filter cat -- --all
git push origin --force --all
```
### [[Git synopsis]]