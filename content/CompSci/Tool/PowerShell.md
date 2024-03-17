---
tags:
  - CompSci/tool/PowerShell
---
# PowerShell
### Description:
- [[Powershell cmdlet]]
- Has .psi file format
### Variables:
```powershell
$location ="East Asia"
$cred = Get-Credential
```
### Loops:
- Comparision ops:
	- `-lt`: less than
	- `-le`: less than or equal
	- `-eq`: equal
	- `-ne`: not equal
- For:
	- ```powershell
		For($i=1, $i -lt 3, $i++)
		{
			$i
		}
- Do...While:
	- 
- For..each
	- s
### Parameters
- Declare as argument
	- ```powershell
		param([int] $size, [string] $location)
- When calling script:
	- ```powershell
	.\exampleScript.ps1 -size 5 -location "East Asia"
	- ```powershell
	.\exampleScript.ps1 5 "East Asia"