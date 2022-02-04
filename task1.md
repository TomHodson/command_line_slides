# Task 1
## Making a simple python project

### Decide where you'd like to put the project
First navigate somewhere we can make a temporary project, I suggest either your home directory or a subdirectory of it:
```bash
cd ~
# or
cd ~/Documents
```

### Make a folder to hold it
We're going to write a script to print the size of files, so let's call it filesize
```bash
pwd #check you're in the right place
mkdir filesize #make a folder here called filesize
```

### Make README.md and requirments.txt files
These files are a de facto standard to have in your python project. README.md describes your project as in written in [MarkDown][MD], which is also what this [document is written in](task1.md).

```bash
nano README.md
```
In nano, `# FileSize` and then `CTRL-O` and then `ENTER` to save and `CTRL-X` to exit.

I'll show you a differnt trick to quickly make a one line file:
```bash
echo "numpy" > requirements.txt
```
This uses two things I haven't told you about, `echo` outputs whatever you give it and `>` saves the output of a command to file.

Check the files contain what you think:
```bash
cat requirements.txt
cat README.md
```
If not you can use nano to edit them. You can also use your own text editor to do this.

### Make a python script 
At this point `pwd` should print something like `/home/user/filesize/` and `ls` should print `requirements.txt` and `README.md`

It's a convention for python project that the actual source code goes in `project_name/project_name/source_code.py`
So make a second folder called `filesize` inside the first.

Now make a python file called "filesize.py" inside it so that it ends up at `filesize/filesize/filesize.py`

Arrange that it contains:
```python
import os, sys
arguments = sys.argv[1:] # The first argument is actually the name of the script
if len(arguments) == 1: print(os.path.getsize(arguments[0]))
else: print(f'filesize requires exactly one argument! Got {len(arguments)}')
```

### Try it out
To run a python script as a command you can use
```bash
python filesize/filesize.py
```
To give it an argument, let's try README.md, run:
```bash
python filesize/filesize.py README.md
```

### A recording of me doing the above, mistakes and all
[![asciicast](https://asciinema.org/a/466633.svg)](https://asciinema.org/a/466633)


[MD]: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
