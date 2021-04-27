# Matroyoshka

This is a proof of concept for a fast and user friendly commandline interface based on [Babashka](https://github.com/babashka/babashka).

The main features are:
- lazy loading of code (fast start time) 
- support for (nested) autocompletion of tasks.

## Demo 

<a href="https://www.loom.com/share/4f56217c9c5c4d32a70b9e8b4316fcb7"> <p>- Watch Video</p> <img style="max-width:300px;" src="https://cdn.loom.com/sessions/thumbnails/4f56217c9c5c4d32a70b9e8b4316fcb7-with-play.gif"> </a>

## Setup

Tested on Macos, inspired by [AWS cli tool](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-completion.html#cli-command-completion-linux)

Clone this repository, go to its directory and copy the following:
```
autoload bashcompinit && bashcompinit
autoload -Uz compinit && compinit
compinit
export PATH=".:$PATH"
matryoshka # to make sure we're on the right path
complete -C matryoshka matryoshka
```

## Credits to

@russmatney for [creating a Babashka demo for task completion](https://github.com/russmatney/bb-task-completion). I wasn't able to figure out how to complete nested commands this way so I decided to follow the example of AWS cli eventually.




