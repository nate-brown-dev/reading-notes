# Notes on the terminal

## Lesson 1: The Command Line

Arguments after command that start with dash (like -l) are called “options”

Bash stands for “Bourne Again Shell” (lol)

“Echo” is a command to display system messages
Can tell you what shell you are using (echo $SHELL)

I am using zsh, not bash (oh my zsh actually)

I read a page about the differences between zsh and bash here [https://www.educba.com/zsh-vs-bash/]

I learned to use the up and down arrows to recall previously typed commands. This could be useful for redoing really long commands, but I type faster than I can use the arrow keys most of the time and I don’t know that I will use it all that often.

## Lesson 2: Basic Navigation

I always type ls when I enter a directory. I haven’t been using ls -l, that’s new

I learned how to use ls to list the contents of another directory instead of the current one

I practiced using ls -l on my Downloads folder while in another directory, showed me a whole bunch of info, a lot like using “view as list” in a macOS folder

I learned about the difference between absolute and relative paths in the terminal, I should have understood this before but never made the connection

The “tab completion” is kinda neat but it’s much harder to type a tab than to type any alpha characters using the home row, I don’t necessarily think tab completion is faster for me at least. Will try to practice

## Lesson 3: More About Files

The explanation of “everything is a file” needs some work. I get it but it’s a lot of circular logic

I learned that command line options are case sensitive and mean different things, I haven’t had firsthand experience with this going wrong yet thankfully

It’s nice to know that you can write path names as string literals to get around having spaces in the names, but IMO it’s best practice just not to use spaces like that

Ran the 'file' command on some system files, interesting to know that they are ‘universal binaries’ for x86_64 and arm64 (I’m on Ventura and presumably this is for compatibility with apple silicon?)

## Lesson 4: Manual Pages

I learned how to search for man pages with `man -k <search>`

Have found previously that man pages are best used in combination with googling or some other, better documentation

I agree that writing longhand command line options is better for knowing what I’m doing most of the time

I only use shorthand options when it’s a command that I use all the time, or when I’m using some command from instructions that I don’t actually understand and am just copying

In the latter case I wish the instructions would use the longhand form, it would help me learn better

I used man -k to search for ‘octal’ and found man ascii, whereI learned about octal ASCII characters

## Lesson 5: File Manipulation

I agree that dumping everything at the base of the home directory is a terrible practice, as an OCD directory organizing person it drives me crazy

I learned how to remove an empty directory with rmdir. I’ve been removing directories with contents using rm -rf for ages and it would never occur to me to empty a directory before removing it

I rarely use touch to make files, in vscode it’s easier to make them with the GUI

I learned how to copy directories with -r (recursive) to make sure and get all the sub directory contents

Along the above lines I learned what -rf actually means (recursive, force) which explains why it works to delete full directories and everything in them. This is probably the most “aha” moment for me in the whole lesson, I’ve used it so many times for so long without knowing

sudo rm -rf / --no-preserve-root (lol)

## Cheat Sheet

I bookmarked the cheat sheet in my bookmarks bar
