# Bash

![Image](../images/bash.png)

**Jack Simpson**  
*11th of May 2015*

## What is Bash?

BASH is an interpretor that accepts commands you write in the terminal and sends them off to the operating system to be performed. Bash is available on the following platforms:

* Mac
* Linux/Unix
* Windows (with [Cygwin](https://www.cygwin.com) installed)

## Why use Bash?

Until recently, I would have agreed with the statement that there was no need to learn BASH due to the ease of scripting languages like Python. However, BASH makes it incredibly easy to perform tasks that you would have done via the terminal.

**Advantages**

* Great for batch manipulations of files: renaming, compressing, moving
* Easy way to build simple pipelines
* Automate compilation of programs
* Supported on all Unix-based systems

**Disadvantages**

* Longer programs can start to look like spaghetti code

## Simple example

You can use BASH to assign variables right from your terminal without any setup required:

```bash
hi='Hello, world!'
echo hi
>> hi
echo $hi
>> Hello, world!
```
This is how it looks when I ran this code earlier in my terminal:

![Image](../images/interactive.png)

## Useful example

I needed to rename all the images in a folder with a number incrementing from 0:

```bash
#!/bin/sh

increment=0
for i in *.jpg
do
mv "$i" "$increment.jpg"
echo $increment
increment=$[increment+1]
done
```

BASH commands can also be saved in a text file and run as a script:

![Image](../images/script.png)

## Learn more

- [A quick guide to writing scripts using the bash shell](http://www.panix.com/~elflord/unix/bash-tute.html)
- [Bash scripting Tutorial](http://linuxconfig.org/bash-scripting-tutorial)
- [BASH Programming - Introduction HOW-TO](http://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO.html)
- [Linux Shell Scripting Tutorial](http://www.freeos.com/guides/lsst/)