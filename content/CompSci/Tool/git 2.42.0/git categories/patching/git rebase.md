---
mindmap-plugin: basic
tags:
  - CompSci/tool/git/command
---

# git rebase

## Description:
- Reapply commits on top of another base tip
- Example:
	- from this:

		-
		  ```mermaid
		  %%{init: { 'theme': 'dark' } }%%
		  gitGraph:
		  commit id: "main first"
		  commit id: "main second"
		  branch new-branch
		  commit id: "new first"
		  commit id: "new second" type: HIGHLIGHT
		  checkout main
		  commit id: "main third"
		  ```

	- to this:

		-
		  ```mermaid
		  %%{init: { 'theme': 'dark' } }%%
		  gitGraph:
		  commit id: "main first"
		  commit id: "main second"
		  commit id: "main third"
		  branch new-branch
		  commit id: "new first"
		  commit id: "new second" type: HIGHLIGHT
		  checkout main
		  ```


## git rebase:
- git rebase
	- `[-i | --interactive]`
	- `[< options >]`
	- `[--exec < cmd >]`
	- `[--onto < newbase > | --keep-base] [< upstream > [< branch >]]`
- git rebase
	- `[-i | --interactive]`
	- `[< options >]`
	- `[--exec < cmd >]`
	- `[--onto < newbase >]`
	- `--root [< branch >]`
- git rebase
	- (--continue | --skip | --abort | --quit | --edit-todo | --show-current-patch)
		- --continue: Restart the rebasing process after having resolved a merge conflict.