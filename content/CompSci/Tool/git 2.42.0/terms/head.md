---
mindmap-plugin: basic
tags:
  - CompSci/tool/git/term
---
# head
### Description:
- Reference to the current commit in Git.
- It is a pointer to the commit that is most likely to be the next commit made to the [[Repository|repository]].
- When you make a change to a file and commit it, Git updates HEAD to point to the new commit
- You can also manually update HEAD to point to a different commit.
	- To do this, you can use the `git reset HEAD` command.
- Be careful when using this command, as it can undo all of your uncommitted changes.