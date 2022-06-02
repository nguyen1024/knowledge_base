# Programs - Linux

## Symbolic Link

```
ln -s <path to the file/folder to be linked> <the path of the link to be created>
```

Reference

- Symlink Tutorial in Linux – How to Create and Remove a Symbolic Link
  - https://www.freecodecamp.org/news/symlink-tutorial-in-linux-how-to-create-and-remove-a-symbolic-link/

## How to Redirect Output to a File
  
Yes it is possible, just redirect the output (AKA stdout) to a file:

```
SomeCommand > SomeFile.txt
```

Or if you want to append data:

```
SomeCommand >> SomeFile.txt
```

If you want stderr as well use this:

```
SomeCommand &> SomeFile.txt 
```

or this to append:

```
SomeCommand &>> SomeFile.txt 
```

if you want to have both stderr and output displayed on the console and in a file use this:

```
SomeCommand 2>&1 | tee SomeFile.txt
```

(If you want the output only, drop the 2 above)
  
Source
- How do I save terminal output to a file?
  - https://askubuntu.com/questions/420981/how-do-i-save-terminal-output-to-a-file

## Diff Tools
  
- Kompare
- DiffMerge
- Meld
- Diffuse
- XXdiff
- KDiff3
- TkDiff
  
Source

- 9 Best File Comparison and Difference (Diff) Tools for Linux
  - https://www.tecmint.com/best-linux-file-diff-tools-comparison/

## Swap Sizes

| Amount of RAM in the system	| Recommended swap space     | Recommended swap space if allowing for hibernation |
| --------------------------- | -------------------------- | -------------------------------------------------- |
| ⩽ 2 GB	                    | 2 times the amount of RAM  | 3 times the amount of RAM                          |
| > 2 GB – 8 GB	              | Equal to the amount of RAM |	2 times the amount of RAM                         |
| > 8 GB – 64 GB	            | At least 4 GB	             | 1.5 times the amount of RAM                        |
| > 64 GB	                    | At least 4 GB	             | Hibernation not recommended                        |

Source

- Chapter 15. Swap Space Red Hat Enterprise Linux 7 _ Red Hat Customer Portal
  - https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/storage_administration_guide/ch-swapspace
