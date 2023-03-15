# shell_basics

To print the absolute path name of the current working directory
```bash
#!/bin/bash
pwd
```
<br>

To display the contents list of your current directory
```bash
#!/bin/bash
ls
```
<br>

To change the working directory to the user’s home directory
```bash
#!/bin/bash
cd ~
```
<br>

To display current directory contents in a long format
```bash
#!/bin/bash
ls -l
```
<br>

To display current directory contents, including hidden files (starting with .). Use the long format
```bash
#!/bin/bash
ls -al
```

<br>

To display current directory contents
- Long format
- with user and group IDs displayed numerically
- And hidden files (starting with .)
```bash
#!/bin/bash
ls -al
```
<br>

To create a directory named `my_first_directory` in the `/tmp/` directory
```bash
#!/bin/bash
mkdir /tmp/my_first_directory/
```
<br>

To move the file `betty` from `/tmp/` to `/tmp/my_first_directory`
```bash
#!/bin/bash
mv /tmp/betty /tmp/my_first_directory/betty
```
<br>

Delete the file `betty`.
- The file `betty` is in `/tmp/my_first_directory`
```bash
#!/bin/bash
rm /tmp/my_first_directory/betty
```
<br>

Delete the directory `my_first_directory` that is in the `/tmp directory`
```bash
#!/bin/bash
rm -rf /tmp/my_first_directory
```
<br>

To change the working directory to the previous one
```bash
#!/bin/bash
cd -
```
<br>

To list all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the `/boot` directory (in this order), in long format
```bash
#!/bin/bash
ls -la . .. /boot
```
<br>

To print the type of the file named `iamafile`. The file `iamafile` will be in the `/tmp` directory when we will run your script.
```bash
#!/bin/bash
file /tmp/iamafile
```
<br>

To create a symbolic link to `/bin/ls`, named `__ls__`. The symbolic link should be created in the current working directory
```bash
#!/bin/bash
ln -s /bin/ls __ls__
```
<br>

To copy all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.

You can consider that all HTML files have the extension `.html`
```bash
#!/bin/bash
cp -u *.html ..
```
<br>

To move all files beginning with an uppercase letter to the directory `/tmp/u`.

You can assume that the directory `/tmp/u` will exist when we will run this script
```bash
#!/bin/bash
mv [[:upper:]]* /tmp/u
```
<br>

To delete all files in the current working directory that end with the character `~`.
```bash
#!/bin/bash
rm *~
```
<br>

To create the directories `welcome/`, `welcome/to/` and `welcome/to/school` in the current directory.

We are only allowed to use two spaces (and lines) in your script, not more.
```bash
#!/bin/bash
mkdir -p welcome/to/school
```
<br>

To list all the files and directories of the current directory, separated by commas (`,`).

- Directory names should end with a slash (`/`)
- Files and directories starting with a dot (`.`) should be listed
- The listing should be alpha ordered, except for the directories `.` and `..` which should be listed at the very beginning
- Only digits and letters are used to sort; Digits should come first
- You can assume that all the files we will test with will have at least one letter or one digit
- The listing should end with a new line
```bash
#!/bin/bash
ls -xamp
```
<br>
