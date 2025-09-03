| Windows | Linux / Mac | Action |
| ---     | ---         | ---    |
| help    | man         | displays a list of commands and the functions that they perform.|
| Get-Location | pwd    | Shows your current working directory.|
| Get-ChildItem | ls    |Lists files and folders in the current working directory.|
| mkdir   | mkdir       |Creates a folder where items can be stored in.|
| Set-Location | cd     |Changes the directory you are working on at a specific moment.|
| New-Item | touch      |Creates a new folder/file based on parameters.|
| Move-Item | mv        |Moves the folder to a different location in the directory.|
| Copy-Item | cp        |Makes a duplicate of a folder or file.|
| Remove-Item | rm      |Gets rid of the folder or file.|
| notepad.exe | vim     |Enables a text editor to pop-up on the screen.|
My OS is: Windows
- [x] Windows
- [] Linux
- [] Mac

My Command Line Shell is: Powershell

### Navigating My OS on the Command Line

1. Full / absolute path to your user's home directory:C:\Users\rishi>
2. Create a directory named `DirA`: New-Item -Name "DirA" -ItemType Directory
3. Create a directory named `Dir B`:New-Item -Name "Dir B" -ItemType Directory
4. Go into `DirA`: cd DirA
5. Go into `Dir B` from `DirA`: Set-Location "$HOME\DirB"
6. Return to your user's home directory: cd "C:\Users\rishi"
7. Create a file named `test.txt`: "Keep pushing forward" | Out-File test.txt
8. Move the file named `test.txt` into `DirA`: Move-Item test.txt .\DirA\
9. Contents of `test.txt`: Get-Content .\DirA\test.txt
```
"Keep pushing forward"
```
10. Make a copy of `test.txt` named `copy.txt` in `DirA`: Copy-Item .\DirA\test.txt .\DirA\copy.txt
11. View the contents of `DirA`: Get-ChildItem .\DirA\
12. Make a copy of `test.txt` in `Dir B` named `fodder.txt`: Copy-Item .\DirA\test.txt .\DirB\fodder.txt
13. Delete / remove both `fodder.txt` AND `Dir B`: Remove-Item .\DirB -Recurse



## Citations

To add citations, provide the site and a summary of what it assisted you with.  If generative AI was used, include which generative AI system was used and what prompt(s) you fed it.
Used Microsoft Copilot to summarize command functions.  
Prompt: "Explain PowerShell and Unix command equivalents for man, pwd, ls, mkdir, cd, touch, mv, cp, rm, vim".
