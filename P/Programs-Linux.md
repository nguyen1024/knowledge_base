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
