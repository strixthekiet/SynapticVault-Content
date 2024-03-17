---
mindmap-plugin: basic
tags:
  - CompSci/tool/git/command
---
# git checkout
### Description:
- Switch branches or restore working tree files
- Updates files in the working tree to match the version in the index or the specified tree. 
	- If no pathspec was given, _git checkout_ will also update `HEAD` to set the specified branch as the current branch.
### git checkout
- git checkout 
	- [-q] 
	- [-f] 
	- [-m] 
	- [< branch >]
- git checkout 
	- [-q] 
	- [-f] 
	- [-m] 
	- --detach [< branch >]
- git checkout 
	- [-q] 
	- [-f] 
	- [-m] 
	- [--detach] < commit >
- git checkout 
	- [-q] 
	- [-f] 
	- [-m] 
	- [[-b|-B|--orphan] < new-branch >] 
	- [< start-point >]
- git checkout 
	- [-f|--ours|--theirs|-m|--conflict=< style >] 
	- [< tree-ish >]
	- [--] 
	- < pathspec >…​
- git checkout 
	- [-f|--ours|--theirs|-m|--conflict=< style >] 
	- [< tree-ish >] 
	- --pathspec-from-file=< file > 
	- [--pathspec-file-nul]
- git checkout 
	- (-p|--patch) 
	- [< tree-ish >] 
	- [--] 
	- [< pathspec >…​]