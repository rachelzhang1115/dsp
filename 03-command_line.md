# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > pwd, mkdir, rmdir, touch filename.txt (or py), rm filename.txt, mv oldfilename.txt newfilename.txt, ls -ad .*, cp filename dirname/, using the * symbol to say "anything" (wildcard matching), apropos (finding help when you don't know the exact command)
  

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > `ls` lists the contents of the directory. `ls -a` lists all (including hidden) contents of the directory. `ls -l` displays the longformat listing. 
> > `ls -lh` displays files in longlisting togehter with file size. `ls -lah` displays all files in longlisting with file size
> > `ls -t` displays newest files first. `ls -Glp` displays files according to content (directories displayed with \ behind them). 

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > `ls -d` (displays only directories), `ls -g` displays the long format listing but exclude the owner name. `ls -p` displays directoreis with /, `ls -R` displays subdirectories as well. `ls -x` displays files as rows across the screen


---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > `xargs` breaks the list of arguments into sublists small enough to be acceptable
> > example: `find /path -type f -print | xargs rm`, here the find utility feeds the input of xargs with a long list of file names. `xargs` then splits this list into sublists and calls `rm` once for every sublist.

 

