## The Command Line
_What's the first thing you think of when you hear this?_
Go to **www.menti.com** and use the code **9132 7354**
<!-- https://www.albionresearch.com/tools/urlencode -->
<img src="https://api.qrserver.com/v1/create-qr-code/?data=https%3A%2F%2Fwww.menti.com%2Fp6qu6susje&size=100x100&qzone=1&format=svg&ecc=L" alt="Use Menti code 9132 7354" title="Menti QR Code" width = "200px"/>


---
## Results
<div style='position: relative; padding-bottom: 56.25%; padding-top: 35px; height: 0; overflow: hidden;'><iframe sandbox='allow-scripts allow-same-origin allow-presentation' allowfullscreen='true' allowtransparency='true' frameborder='0' height='315' src='https://www.mentimeter.com/embed/c92cb2f99d7edcaa0b0be2a177c5f231/1edf2d837bdd' style='position: absolute; top: 0; left: 0; width: 100%; height: 100%;' width='420'></iframe></div>
---
## What is the command line?
- A text based interface to a computer. <!-- .element: class="fragment" -->
- A programming language.<!-- .element: class="fragment" -->
- A tool with strengths and weaknesses. <!-- .element: class="fragment" -->

---
## Quick demo
<div class="asciicast">
    <!--
    {
        "URL": "casts/task1.cast",
        "idle_time_limit": 0.5, 
        "start":12,
        "speed":1.5,
        "poster": "npt:1:23"
    } 
    -->
</div>

---
## Why use it?

- A lot of great tools are command line only!<!-- .element: class="fragment" -->

- Different tools can be combined easily. <!-- .element: class="fragment" -->

- Task can be automated easily using shell scripts. <!-- .element: class="fragment" -->

---
## Why don't people just make a GUI?
- It's easier and faster. <!-- .element: class="fragment" -->
- CMD tools are more flexible. <!-- .element: class="fragment" -->
---
## Walking the filesystem
<img class="r-stretch" src="./images/filesystem.svg">

---
## Paths
```bash
home/tom/im_a_path/im_a_file.txt
```
- Paths tell commands where to look for files and folders. 
- A way to specifiy a file or folder with a text string.
- They look a bit like URLs because they share some ideas.

---
## Absolute Paths

- When they start with `/` they're **absolute** i.e 
```bash 
/bin/ls
```
This means they start from the root directory.
---
## Relative Paths

Relative paths are specified relative to the current directory.
```bash
tjones/notes.txt
../hpc-0123/data.hdf5 #goes one level up
```
---
### Looking around: ls and pwd
```bash
pwd # print your 'present working directory' 
# i.e where you are right now.
ls # List the files and folders in the pwd
```
---

## Getting around
```bash
$ cd / # go to the root directory
$ cd   # go to your home directory
$ cd ~/foo  # go to some folder in your home directory
$ cd ../  # go up one level from wherever you are
```
---
## Looking in files

```bash
$ cat file # outputs a file to the terminal 
$ nano file # opens a file for basic editing
```
To save the file in nano press `CTRL-O` (for output)
To exit press `CTRL-X`

---
## Messing around

```bash
$ mkdir folder # makes a directory
$ mv file1 folder/file2 # moves and renames
$ cp file1 folder/file2 # copies and renames
$ rm file #deletes the file permenantly
# be careful with rm!
```
---
Ok now you try!

[tomhodson.github.io/command_line_slides/task1](https://tomhodson.github.io/command_line_slides/task1)

Slides at

[tomhodson.github.io/command_line_slides](https://tomhodson.github.io/command_line_slides)
---
<!-- .slide: data-background-iframe="https://tomhodson.github.io/command_line_slides/task1" data-background-interactive data-background-transition="zoom"-->
---
### Demo of me doing task 1
<div class="asciicast">
    <!--
    {
        "URL": "casts/task1.cast",
        "poster": "npt:2:30",
        "font-size": "0.5em",
        "idle_time_limit": 0.5, 
        "start":12
    } 
    -->
</div>
---

## Second Half
---
## A more complex command
```bash
$ git commit --dry-run -m "My commit message" ./*.py 
```
---

---

## A Simple Script
```bash
#!/usr/bin/env bash
echo "Hello World"
echo "You invoked this script with $# arguments, the first one was $1"
variable=42
echo "The variable is ${variable}"
```
---

## Running a script

```bash
chmod +x my_script.sh
./my_script.sh
```

---
demo of running the script

---
Task 2

---
### Demo of me doing task 2
<div class="asciicast">
    <!--
    {
        "URL": "casts/task2.cast",
        "poster": "npt:2:30",
        "font-size": "0.6em",
        "idle_time_limit": 2, 
        "start":0
    } 
    -->
</div>
---
# FIN
---

<!-- .slide: data-background-iframe="https://www.explainshell.com/explain?cmd=wget+-P+%2Fpath%2Fto%2Fdestination%2Fdirectory%2F+-mpck+--user-agent%3D%22%22+-e+robots%3Doff+--wait+1+-E+https%3A%2F%2Fwww.example.com%2F#" data-background-interactive data-background-transition="zoom"-->


---

<div class="asciicast">
    <!--
    {
        "URL": "casts/git.cast",
        "poster": "npt:2:30",
        "autoplay": false,
        "preload": true,
        "font-size": "medium",
        "rows":30
    } 
    -->
</div>
---

```bash
$ command -f --longer-flag --keyword="value" arg1 arg2 ...
```

---
For really complex commands you find online, [explainshell.com]() is nice.

Let's try
```bash
wget -P /path/to/destination/directory/ \ 
    -mpck --user-agent="" -e robots=off --wait 1 \
    -E https://www.example.com/
```
---
<!-- .slide: data-background-iframe="https://www.explainshell.com/explain?cmd=wget+-P+%2Fpath%2Fto%2Fdestination%2Fdirectory%2F+-mpck+--user-agent%3D%22%22+-e+robots%3Doff+--wait+1+-E+https%3A%2F%2Fwww.example.com%2F#" data-background-interactive data-background-transition="zoom"-->


