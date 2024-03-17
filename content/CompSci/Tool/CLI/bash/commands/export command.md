---
tags:
  - CompSci/tool/cli/bash/command/builtin
---
# export command
### Description:
- Mark each name to be passed to child processes in the environment. 
- Then the variable can be printed as $var_name
### Synopis:
- `export [-fn] [-p] [name[=value]]`
	- If the -foption is supplied, the names refer to shell functions; otherwise the names refer to shell variables. 
	- The -n option means to no longer mark each name for export. 
	- If no names are supplied, or if the -p option is given, a list of names of all exported variables is displayed. The -p option displays output in a form that may be reused as input. If a variable name is followed by =value, the value of the variable is set to value.
	- The return status is zero unless an invalid option is supplied, one of the names is not a valid shell variable name, or -f is supplied with a name that is not a shell function.