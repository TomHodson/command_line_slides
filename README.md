# Intro to the Command Line - A slide deck
[Click here to view the slide deck on github.io][slides]

![image](https://user-images.githubusercontent.com/2063944/153746049-6e4c10e2-63b3-4759-b436-5dc0eda5b728.png)

## What is this

It's a slide deck I used to introduce some students to the command line for the first time.

It's also an example of how to integrate two things:
- [reveal.js](https://revealjs.com/), a JS library for making really nice presentations which supports a mix of MarkDown, CSS, HTML and JS.
- [asciinema](https://asciinema.org/) A tool to record interactive command line usage and then play it back beautifully with control over formatting and speed.

I've added a hook to automatically play/pause each player when you enter/exit that slide.

## Technical background
This uses the [anything][anything] plugin for reveal.js and the current stable version 2.x of asciinema. There is a new v3.x of asciinema but at the time of writing the [v3.x dev branch][asciinema-dev] of asciinema-player does not expose a API to play and pause the player. If you want to use v3.x of the player see my comment [here][using3] for a some working code.
 
[slides]: https://tomhodson.github.io/command_line_slides/#/22
[anything]: https://github.com/rajgoel/reveal.js-plugins/tree/master/anything
[using3]: https://github.com/rajgoel/reveal.js-plugins/issues/11
[asciinema-dev]: https://github.com/asciinema/asciinema-player
