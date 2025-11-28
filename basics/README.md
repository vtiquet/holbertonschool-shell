<div align="center"><img src="https://github.com/vtiquet/holbertonschool-resources/blob/main/image/Holberton-Logo.svg" width=40% height=40%/></div>

# Resources

## Table of Contents :

  - [0. Where am I?](#subparagraph0)
  - [1. What’s in there?](#subparagraph1)
  - [2. There is no place like home](#subparagraph2)
  - [3. The long format](#subparagraph3)
  - [4. Hidden files](#subparagraph4)
  - [5. I love numbers](#subparagraph5)
  - [6. Welcome](#subparagraph6)
  - [7. Betty in my first directory](#subparagraph7)
  - [8. Bye bye Betty](#subparagraph8)
  - [9. Bye bye My first directory](#subparagraph9)
  - [10. Back to the future](#subparagraph10)
  - [11. Lists](#subparagraph11)
  - [12. File type](#subparagraph12)
  - [13. We are symbols, and inhabit symbols](#subparagraph13)
  - [14. Copy HTML files](#subparagraph14)
  - [15. Let’s move](#subparagraph15)
  - [16. Clean Emacs](#subparagraph16)
  - [17. Tree](#subparagraph17)

## Resources
### Read or watch:
* [What Is “The Shell”?](/rltoken/aygkrwOyI_yLtXHF1Yj0QQ)
* [Navigation](/rltoken/fMDkg3TKjANJSPTROMQSpA)
* [Looking Around](/rltoken/isPTWCOgTjeLaonZg8Rl5g)
* [A Guided Tour](/rltoken/GznRkhU3QTWAWwDeZ-k9Pw)
* [Manipulating Files](/rltoken/GA2UvOhDOjwa-NtbazvlCQ)
* [Working With Commands](/rltoken/ylGnKaanTSp3jIpXme9krg)
* [Reading Man pages](/rltoken/52aXMywgSkXV07rFrX8eWw)
* [Keyboard shortcuts for Bash](/rltoken/L8zadP97oAbt2j9LWDhYKA)
* [LTS](https://wiki.ubuntu.com/LTS)
* [Shebang](/rltoken/_pJ5Fl2TaZVzW3jJy_mwKA)
* [Linux file systems explained](/rltoken/0XMp-7-ibZ3uKpDF6V_9Mw)

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:
* What does RTFM mean?
* What is a Shebang

## Requirements
### General
* Allowed editors:vi,vim,emacs
* All your scripts will be tested on Ubuntu 22.04 LTS
* All your scripts should be exactly two lines long ($ wc -l fileshould print 2)
* All your files should end with a new line (why?)
* The first line of all your files should be exactly#!/bin/bash
* AREADME.mdfile at the root of the repo, containing a description of the repository
* AREADME.mdfile, at the root of the folder ofthisproject, describing what each script is doing
* You are not allowed to use backticks,&&,||or;
* All your scripts must be executable. To make your file executable, use thechmodcommand:chmod u+x FILENAME_GOES_HERE. Later, we’ll learn more about how to utilize this command.

## Task
### 0. Where am I? <a name='subparagraph0'></a>

Write a script that prints the absolute path name of the current working directory.

Example:

```
$ ./0-current_working_directory
/basics
$
```

---

### 1. What’s in there? <a name='subparagraph1'></a>

Display the contents list of your current directory.

Example:

```
$ ./1-listit
Applications    Documents   Dropbox Movies Pictures
Desktop Downloads   Library Music Public
$
```

---

### 2. There is no place like home <a name='subparagraph2'></a>

Write a script that changes the working directory to the user’s home directory.

* You are not allowed to use any shell variables

Example:

```
julien@ubuntu:/tmp$ pwd
/tmp
julien@ubuntu:/tmp$ echo $HOME
/home/julien
julien@ubuntu:/tmp$ source ./2-bring_me_home
julien@ubuntu:~$ pwd
/home/julien
julien@ubuntu:~$
```

---

### 3. The long format <a name='subparagraph3'></a>

Display current directory contents in a long format

Example:

```
$ ./3-listfiles
total 40
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:19 0-current_working_directory
-rwxr-xr-x@ 1 sylvain staff 19 Jan 25 00:23 1-listit
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:29 2-bring_me_home
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:39 3-listfiles
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:20 README.md
$
```

---

### 4. Hidden files <a name='subparagraph4'></a>

Display current directory contents, including hidden files (starting with <code>.</code>). Use the long format.

Example:

```
$ ./4-listmorefiles
total 48
drwxr-xr-x@ 6 sylvain staff 204 Jan 25 00:29 .
drwxr-xr-x@ 43 sylvain staff 1462 Jan 25 00:19 ..
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:19 0-current_working_directory
-rwxr-xr-x@ 1 sylvain staff 19 Jan 25 00:23 1-listit
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:29 2-bring_me_home
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:39 3-listfiles
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:41 4-listmorefiles
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:20 README.md
$
```

---

### 5. I love numbers <a name='subparagraph5'></a>

Display current directory contents.

* Long format
* with user and group IDs displayed numerically
* And hidden files (starting with .)

Example:

```
$ ./5-listfilesdigitonly
total 56
drwxr-xr-x@ 6 501 20 204 Jan 25 00:29 .
drwxr-xr-x@ 43 501 20 1462 Jan 25 00:19 ..
-rwxr-xr-x@ 1 501 20 18 Jan 25 00:19 0-current_working_directory
-rwxr-xr-x@ 1 501 20 18 Jan 25 00:23 1-listfiles
-rwxr-xr-x@ 1 501 20 19 Jan 25 00:29 2-bring_me_home
-rwxr-xr-x@ 1 501 20 20 Jan 25 00:39 3-listfiles
-rwxr-xr-x@ 1 501 20 18 Jan 25 00:41 4-listmorefiles
-rwxr-xr-x@ 1 501 20 18 Jan 25 00:43 5-listfilesdigitonly
-rwxr-xr-x@ 1 501 20 18 Jan 25 00:20 README.md
$
```

---

### 6. Welcome <a name='subparagraph6'></a>

Create a script that creates a directory named <code>my_first_directory</code> in the <code>/tmp/</code> directory.

Example:

```
$ ./6-firstdirectory
$ file /tmp/my_first_directory/
/tmp/my_first_directory/: directory
$
```

---

### 7. Betty in my first directory <a name='subparagraph7'></a>

Move the file <code>betty</code> from <code>/tmp/</code> to <code>/tmp/my_first_directory</code>.

Example:

```
$ ./7-movethatfile
$ ls /tmp/my_first_directory/
betty
$
```

---

### 8. Bye bye Betty <a name='subparagraph8'></a>

Delete the file <code>betty</code>.

* The file <code>betty</code> is in <code>/tmp/my_first_directory</code>

Example:

```
$ ./8-firstdelete
$ ls /tmp/my_first_directory/
$
```

---

### 9. Bye bye My first directory <a name='subparagraph9'></a>

Delete the directory <code>my_first_directory</code> that is in the <code>/tmp</code> directory.

Example:

```
$ ./9-firstdirdeletion
$ file /tmp/my_first_directory
/tmp/my_first_directory: cannot open `/tmp/my_first_directory' (No such file or directory)
$
```

---

### 10. Back to the future <a name='subparagraph10'></a>

Write a script that changes the working directory to the previous one.

```
julien@ubuntu:/tmp$ pwd
/tmp
julien@ubuntu:/tmp$ cd /var
julien@ubuntu:/var$ pwd
/var
julien@ubuntu:/var$ source ./10-back
/tmp
julien@ubuntu:/tmp$ pwd
/tmp
```

---

### 11. Lists <a name='subparagraph11'></a>

Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the <code>/boot</code> directory (in this order), in long format.

Be careful with the <code>/</code>

---

### 12. File type <a name='subparagraph12'></a>

Write a script that prints the type of the file named <code>iamafile</code>. The file <code>iamafile</code> will be in the <code>/tmp</code> directory when we will run your script.

Example

```
ubuntu@ip-172-31-63-244:~$ ./12-file_type
/tmp/iamafile: ELF 64-bit LSB  executable, x86-64, version 1 (SYSV), dynamically linked (uses shared libs), for GNU/Linux 2.6.24, BuildID[sha1]=bd39c07194a778ccc066fc963ca152bdfaa3f971, stripped
```

Note that depending on the file, the output of your script will be different.

---

### 13. We are symbols, and inhabit symbols <a name='subparagraph13'></a>

Create a symbolic link to <code>/bin/ls</code>, named <code>__ls__</code>.
The symbolic link should be created in the current working directory.

```
ubuntu@ip-172-31-63-244:/tmp/sym$ ls -la
total 144
drwxrwxr-x  2 ubuntu ubuntu   4096 Sep 20 03:24 .
drwxrwxrwt 12 root   root   139264 Sep 20 03:24 ..
ubuntu@ip-172-31-63-244:/tmp/sym$./13-symbolic_link
ubuntu@ip-172-31-63-244:/tmp/sym$ ls -la
total 144
drwxrwxr-x  2 ubuntu ubuntu   4096 Sep 20 03:24 .
drwxrwxrwt 12 root   root   139264 Sep 20 03:24 ..
lrwxrwxrwx  1 ubuntu ubuntu      7 Sep 20 03:24 __ls__ -> /bin/ls
```

---

### 14. Copy HTML files <a name='subparagraph14'></a>

Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.

You can consider that all HTML files have the extension <code>.html</code>

---

### 15. Let’s move <a name='subparagraph15'></a>

Create a script that moves all files beginning with an uppercase letter to the directory <code>/tmp/u</code>.

You can assume that the directory <code>/tmp/u</code> will exist when we will run your script

```
ubuntu@ip-172-31-63-244:/tmp/sym$ ls -la
total 148
drwxrwxr-x  3 ubuntu ubuntu   4096 Sep 20 03:33 .
drwxrwxrwt 12 root   root   139264 Sep 20 03:26 ..
-rw-rw-r--  1 ubuntu ubuntu      0 Sep 20 03:32 My_file
lrwxrwxrwx  1 ubuntu ubuntu      7 Sep 20 03:24 __ls__ -> /bin/ls
-rw-rw-r--  1 ubuntu ubuntu      0 Sep 20 03:32 Elif_ym
-rw-rw-r--  1 ubuntu ubuntu      0 Sep 20 03:32 random_file
ubuntu@ip-172-31-63-244:/tmp/sym$ ls -la /tmp/u
total 8
drwxrwxr-x 2 ubuntu ubuntu 4096 Sep 20 03:33 .
drwxrwxr-x 3 ubuntu ubuntu 4096 Sep 20 03:33 ..
ubuntu@ip-172-31-63-244:/tmp/sym$ ./15-lets_move
ubuntu@ip-172-31-63-244:/tmp/sym$ ls -la
total 148
drwxrwxr-x  3 ubuntu ubuntu   4096 Sep 20 03:33 .
drwxrwxrwt 12 root   root   139264 Sep 20 03:26 ..
lrwxrwxrwx  1 ubuntu ubuntu      7 Sep 20 03:24 __ls__ -> /bin/ls
-rw-rw-r--  1 ubuntu ubuntu      0 Sep 20 03:32 random_file
ubuntu@ip-172-31-63-244:/tmp/sym$ ls -la /tmp/u
total 8
drwxrwxr-x 2 ubuntu ubuntu 4096 Sep 20 03:33 .
drwxrwxr-x 3 ubuntu ubuntu 4096 Sep 20 03:33 ..
-rw-rw-r-- 1 ubuntu ubuntu    0 Sep 20 03:32 My_file
-rw-rw-r-- 1 ubuntu ubuntu    0 Sep 20 03:32 Elif_ym
```

---

### 16. Clean Emacs <a name='subparagraph16'></a>

Create a script that deletes all files in the current working directory that end with the character <code>~</code>.

```
ubuntu@ip-172-31-63-244:/tmp/sym$ ls
main.c  main.c~  Makefile~
ubuntu@ip-172-31-63-244:/tmp/sym$ ./16-clean_emacs
ubuntu@ip-172-31-63-244:/tmp/emacs$ ls
main.c
ubuntu@ip-172-31-63-244:/tmp/emacs$
```

---

### 17. Tree <a name='subparagraph17'></a>

Create a script that creates the directories <code>welcome/</code>, <code>welcome/to/</code> and <code>welcome/to/school</code> in the current directory.

You are only allowed to use two spaces (and lines) in your script, not more.

```
julien@ubuntu:/tmp/h$ ls -l
total 4
-rwxrw-r-- 1 julien julien 44 Sep 20 12:09 17-tree
julien@ubuntu:/tmp/h$ wc -l 17-tree 
2 17-tree
julien@ubuntu:/tmp/h$ head -1 17-tree 
#!/bin/bash
julien@ubuntu:/tmp/h$ tr -cd ' ' < 17-tree | wc -c # you do not have to understand this yet, but the result should be 2, 1 or 0
2
julien@ubuntu:/tmp/h$ ./17-tree 
julien@ubuntu:/tmp/h$ ls
17-tree  welcome
julien@ubuntu:/tmp/h$ ls welcome/
to
julien@ubuntu:/tmp/h$ ls -l welcome/to
total 4
drwxrwxr-x 2 julien julien 4096 Sep 20 12:11 school
julien@ubuntu:/tmp/h$
```

---


## Authors
vtiquet - [GitHub Profile](https://github.com/vtiquet)
