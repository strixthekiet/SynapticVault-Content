---
mindmap-plugin: basic
tags:
  - CompSci/tool/cli/bash/command
---
# man
### Description:
- System's manual pager.  
- Each page argument given to `man` is normally the name of a program, utility or function. 
- The manual page associated with each of these  arguments is then found and displayed. 
- A section, if provided, will direct `man` to look only in that section of the manual.  
- The default action is to search in all of the available sections following a pre-defined order (see DEFAULTS), and to show only the first page found, even if page exists in several sections.
### Synopis
- `man`
	- `[man options]`
	- `[[section] page ...]`
	- `...`
- `man`
	- `-k`
		- 
	- `[apropos options]`
	- `regexp`
	- `...`
- `man`
	- `-K`
	- `[man options]`
	- `[section]`
	- `term`
	- `...`
- `man`
	- `-f|--whatis`
		- -f, --whatis
		- Equivalent to whatis.  
		- Display a short description from  the  manual  page,  if available.  See whatis(1) for details.
	- `[whatis options]`
	- `page`
	- `...`
- `man` 
	- `-l`
	- `[man options]`
	- `file`
	- `...`
- `man` 
	- `-w|-W` 
	- `[man options]` 
	- `page` 
	- `...`
### Sections
1. Executable programs or shell command
2. System calls
4. special files
5. file formats and conventions
6. Games
7. 
8. System administration commands
9. Kernel routines
### Built-in commands:
- run `man builtins`
### How to read?
- Conventional  section  names  include:
	- NAME
	- SYNOPSIS
	- CONFIGURATION
	- DESCRIPTION
	 - OPTIONS
	- EXIT STATUS
	- RETURN VALUE
	- ERRORS
	- ENVIRONMENT
	- FILES
	- VERSIONS
	- CONFORMING TO
	- NOTES
	- BUGS
	- EXAMPLE
	- AUTHORS
	- SEE ALSO

- 