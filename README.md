# Python Map Reduce

Basic Python introduction and concepts needed in preparation for working with map-reduce solutions.

## Requirements

- Install Chocolatey, the Windows package manager
- Install the Anaconda 3 version for Python + common packages
- Install Visual Studio Code for text editing
- Add Open Command Window Here as Administrator to your File Explorer context menu.

See: [Basic Setup for Big Data](https://github.com/denisecase/basic-setup-for-bigdata)

## Case 1:  Local file-based
To run python files in powershell
```PowerShell
py 11mapper.py
py 12sorter.py
py 13reducer.py
```
After running all 3 files you will get transaction-mapped.txt,transaction-sorted.txt, and transaction-reduced.txt
## Case 2:  Use standard input and output

Use the console (standard input and output) and shell commands to pipe information.  We'll use the built-in shell sort command, so we don't need that anymore. 

cat data | map | sort | reduce

PowerShell and Bash use the same commands:

```Bash
cat part.txt
cat part.txt | python 21mapper.py
cat part.txt | python 21mapper.py | sort
cat part.txt | python 21mapper.py | sort  | python 22reducer.py

```PowerSUphon-map-reduce)
