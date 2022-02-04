# The Command Line
_What's the first thing you think of when you hear this?_
Go to **www.menti.com** and use the code **9132 7354**
<!-- https://www.albionresearch.com/tools/urlencode -->
<img src="https://api.qrserver.com/v1/create-qr-code/?data=https%3A%2F%2Fwww.menti.com%2Fp6qu6susje&size=100x100&qzone=1&format=svg&ecc=L" alt="Use Menti code 9132 7354" title="Menti QR Code" width = "200px"/>


---
## Results
<div style='position: relative; padding-bottom: 56.25%; padding-top: 35px; height: 0; overflow: hidden;'><iframe sandbox='allow-scripts allow-same-origin allow-presentation' allowfullscreen='true' allowtransparency='true' frameborder='0' height='315' src='https://www.mentimeter.com/embed/c92cb2f99d7edcaa0b0be2a177c5f231/1edf2d837bdd' style='position: absolute; top: 0; left: 0; width: 100%; height: 100%;' width='420'></iframe></div>

---
## What is the command line?
A text based interface to your computer <!-- .element: class="fragment" -->

---
<div>
    <!--
    {
        "URL": "casts/ping.cast",
        "poster": "npt:1:23",
        "autoplay": false,
        "preload": true,
        "font-size": "medium",
        "theme": "asciinema"
    } 
    -->
</div>

---
## Why use it?
- A lot of great tools are command line only!<!-- .element: class="fragment" -->
- Some of these tools are better as command line applications. <!-- .element: class="fragment" -->
---
## Why don't people just make a GUI?
---
## What is the command line itself?
---
A REPL or Read Evaluate Print Loop

Let's write one
```python
while True:
    try:
        input_line = input('>>> ')
        print(eval(input_line))
    except KeyboardInterrupt: break
```
---
<div class="asciicast">
    <!--
    {
        "URL": "casts/repl.cast",
        "poster": "npt:0:5",
        "autoplay": false,
        "preload": true,
        "font-size": "medium",
        "theme": "asciinema",
        "rows":10
    } 
    -->
</div>
---
The command line is also a REPL, it just uses different syntax.  
---
<div class="asciicast">
    <!--
    {
        "URL": "casts/git.cast",
        "poster": "npt:2:30",
        "autoplay": false,
        "preload": true,
        "font-size": "medium",
        "theme": "asciinema",
        "rows":30
    } 
    -->
</div>
---

```bash
$ command -f --longer-flag --keyword="value" arg1 arg2 ...
```

---

```bash
$ git commit --dry-run -m "My commit message" ./*.py 
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
---
## Getting around
```bash
$ pwd # print your 'present working directory' 
# i.e where you are right now.
$ cd / # go to the root directory
$ cd   # go to your home directory
$ cd ~/foo  # go to some folder in your home directory
$ cd ../  # go up one level from wherever you are
```

---
## Paths

- A way to specifiy a file or folder with a string.
- They look a bit like URLs because they share some ideas.
- Paths tell commands where to look for files and folders. 

---
## Absolute Paths

- When they start with `\` they're **absolute** i.e 
```bash 
/bin/bash
```
---
---
## Relative Paths

- Relative paths are specified relative to the current directory. `pwd`
- If you're at `/home/name` then `folder/file` would refer to `/home/name/folder/file`
---
- `./folder/file` would also refer to `/home/name/folder/file`
- `../folder/file` would refer 'one level up' to `/home/folder/file`

---
## Looking around

```bash
$ ls #prints a list of files in the current directory
$ cat file # outputs a file to the terminal 
$ nano file # opens a file for basic editing
```

---
## Messing around

```bash
$ mkdir folder # makes a directory
$ mv file1 folder/file2 # moves and renames a file or folder
$ cp file1 folder/file2 # copies and renames a file or folder
$ chmod +x script #changes the permissions of a file, google this. 
```

---
Ok now you try:
[tomhodson.github.io/command_line_slides/task1](https://tomhodson.github.io/command_line_slides/task1)

---
### Package managers
- apt-get, brew, pacman, conda, pip, npm


---
### SSH

---

### Git

---
## Bash Scripts
```bash [1-2|3|4]
#!/usr/bin/env bash
echo "Hello World"
echo "You invoked this script with $# arguments, the first one was $1"
variable=42
echo "The variable is ${variable}"
```

---
## using ping to check if an address is available
<div class="asciicast">
    <!--
    {
        "URL": "casts/ping.cast",
        "poster": "npt:1:23",
        "autoplay": false,
        "preload": true,
        "font-size": "medium",
        "theme": "asciinema"
    } 
    -->
</div>

---
## using ping to check if an address is available
<div class="asciicast">
    <!--
    {
        "URL": "casts/brew.cast",
        "poster": "npt:1:23",
        "autoplay": false,
        "preload": true,
        "font-size": "medium",
        "theme": "asciinema"
    } 
    -->
</div>

---


