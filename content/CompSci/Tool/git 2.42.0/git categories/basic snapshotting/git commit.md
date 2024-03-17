---
mindmap-plugin: basic
aliases:
  - commit
tags:
  - CompSci/tool/git/command
---

# git commit

### Description:
- A commit is a snapshot of the code
- A file is called a "blob" and it is a bunch of bytes
- Move the [[head]]

### git commit
- ...
- \[-F \<file> | -m \<msg>] 
	- Use the given \<msg> as the commit message. 
		- If multiple `-m` options are given, their values are concatenated as separate paragraphs.
	- Take the commit message from the given file. Use `-t` to read the message from the standard input.
	- The `-m` option is mutually exclusive with `-c`, `-C`, and `-F`.
- ...