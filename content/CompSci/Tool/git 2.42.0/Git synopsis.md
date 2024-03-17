---
mindmap-plugin: basic
tags:
  - CompSci/tool/git
---
# Git synopsis
### Placeholders are spelled in lowercase and enclosed in angle brackets:
- 
  ```bash
  <file>
   --sort=<key>
   --abbrev[=<n>]
   ```

- If a placeholder has multiple words, they are separated by dashes:
	- 
	  ```bash
	  <new-branch-name>
		--template=<template-directory>
	   ```
### Possibility of multiple occurrences is indicated by three dots:
- 
  ```bash
  <file>...
   (One or more of <file>.)
   ```

### Optional parts are enclosed in square brackets:
- 
  ```bash
  [<file>...]
   (Zero or more of <file>.)

   --exec-path[=<path>]
   (Option with an optional argument.  Note that the "=" is inside the
   brackets.)

   [<patch>...]
   (Zero or more of <patch>.  Note that the dots are inside, not
   outside the brackets.)
	```
### Multiple alternatives are indicated with vertical bars:
- 
  ```bash
   [-q | --quiet]
   [--utf8 | --no-utf8]
	```

 - Use spacing around "|" token(s), but not immediately after opening or before closing a [] or () pair:
	 - Do: `[-q | --quiet]`
	 - Don't: `[-q|--quiet]`

 - Don't use spacing around "|" tokens when they're used to separate the alternate arguments of an option:
	- Do: `--track[=(direct|inherit)]`
	- Don't: `--track[=(direct | inherit)]`
 ### Parentheses are used for grouping:
- 
	``` bash
		[(<rev> | <range>)...]
	```
	- (Any number of either `<rev>` or `<range>`.  Parens are needed to make it clear that "..." pertains to both `<rev>` and `<range>`.)
- 
	  ``` bash
		[(-p <parent>)...]
	```
	- (Any number of option -p, each with one `<parent>` argument.)
- 
  ```bash
	git remote set-head <name> (-a | -d | <branch>)
	```
	   - (One and only one of "`-a`", "`-d`" or "`<branch>`" _must_ (no square brackets) be provided.)
- And a somewhat more contrived example:
  ```
	--diff-filter=[(A|C|D|M|R|T|U|X|B)...[*]]
	```
	   - Here "=" is outside the brackets, because "--diff-filter=" is a valid usage.  "*" has its own pair of brackets, because it can (optionally) be specified only when one or more of the letters is also provided.