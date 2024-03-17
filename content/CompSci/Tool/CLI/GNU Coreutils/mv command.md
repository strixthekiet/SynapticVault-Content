---
tags:
  - CompSci/tool/cli/command
---
# mv command
### Description:
- Moves or renames files (or directories).
- If two file names are given, `mv` moves the first file to the second.
- If the --target-directory (-t) option is given, or failing that if the last file is a directory and the --no-target-directory (-T) option is not given, `mv` moves each source file to the specified directory, using the sources’ names.
### Synopis:
- `mv [option]… [-T] source dest`
- `mv [option]… source… directory`
- `mv [option]… -t directory source…`