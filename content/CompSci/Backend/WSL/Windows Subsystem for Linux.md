---
tags:
  - CompSci/dev/backend/vm
aliases:
  - wsl
---
# Windows Subsystem for Linux
### Description:
- s
	- sad
### Common commands:
- `wsl --install -d Debian`
- `wsl -d Debian `
	- to open
- `wsl --export Debian debian.tar`
- `wsl --import Debian1 .\install\location path\to\debian.tar`
	- `wsl --import Debian1 .\Documents\project path\to\debian.tar`
- `wsl -d Debian1`
- `wsl --unregister Debian1`