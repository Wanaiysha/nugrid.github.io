#  The unix command line

This section uses material compiled by Brian O'Shea for his ICP 490 class at MSU.

## the shell
The program that provides the command line (not all of the commands) is the shell. A common shell is `bash`. Try `> man bash`. The command line is a unix process. Launching a command on the command line interface (CLI) spawns a child process.

## file manipulation
* you will need a terminal command line editor without GUI, such as `emacs` or `vi`
* more/less/tail/head
* cat, touch
* cp, rm
* grep
* wc (-l)

## file system
* ls (-l, many other options)
* cd  (. or .. or ~ or actual directory)
* pwd
* mkdir
* rmdir
* mv  (works on files and directories)
* du (-sh)
* df (-h)

## helpful commands
* man (command)
* history

## networking
* ssh
* scp
* whoami
* rsync
* ftp
* wget

## processes
* top
* ps
* pipes and filters: use | to pipe between command, use > to redirect output

## customizing your CLI
You can define variables and aliases in the .bashrc file. The details on how this is set up depends on the particular Linux/Unix/Mac flavour.

* alias
* environment variables

##Shell scripts

You can combine a sequence of shell commands into a file and use as a shell script. You have to make the file with the script executable (`chmod u+x file_name.sh`). See file `example.sh` in the [example directory](https://github.com/fherwig/physmath248_pilot/blob/master/examples/example.sh).

## Resources
You can find numerous online tutorials and support resources on the internet, such as (search yourself for other and let us know what you find useful) [last updated: 01/2015]:

* <http://linuxcommand.org/lc3_learning_the_shell.php>
* <http://www.emacswiki.org/emacs/LearningEmacs>
* <https://www.youtube.com/watch?v=hbzRWQjA6kI>
* <https://www.youtube.com/watch?v=pYUGzgYAgEo>
* <https://www.youtube.com/watch?v=3DA1grSp4mU>
* you can do very advanced things, as shown, for example, in this [bash tutorial](http://www.funtoo.org/Bash_by_Example,_Part_1), [thanks for the suggestion](https://github.com/Hoverbear)

These tutorials may differ in which shell and/or command line editor they us. Don't get confused by that.

**Exercise:**

- create a directory and go into it
- create a text file (with touch), edit it with the CLI editor of your choice to fill it with the names of lots of people you know
- move the file to another name.
- how many lines does it have?
- search through the file for all incidences of a particular letter or string, and count them with 'wc'
- use 'man' to look at the various options for 'grep', and then look for lines that do NOT have the letter 'e' in it.
- go up one directory, and use 'du -h' on 1) the entire directory tree, and 2) just the new directory.
- use 'man' to look at the options for 'rm', and then delete *ONLY* the entire directory you just created in one command.
- use 'history' to see what you just did!
- save 