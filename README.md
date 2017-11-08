# ITP Terminal Workshop

## Basic Commands
### pwd
present working directory(where i am)
```shell
$ pwd

/Users/[UserName]
```  

### ls
list
```shell
$ ls

Applications	Desktop		Dropbox		Music		VirtualBox VMs
BouncingBallApp	Documents	Library		Pictures	node_modules
CinderProject	Downloads	Movies		Public		tmp
```

### cd
change directory
```shell
$ cd Documents
$ pwd

/Users/[UserName]/Documents

move up one directory
$ cd ..

```

### mkdir
make a new directory
```shell
$ ls

C++			javascript_basic	python
cinder_class		js_mvp			sass-sandbox
drive.txt		mobile_app		spa
github			openscad		upload
hue-control		openscad.md

$ mkdir ITP_CAMP_TEST
$ ls

C++			hue-control		openscad.md
ITP_CAMP_TEST(new)		javascript_basic	python
cinder_class		js_mvp			sass-sandbox
drive.txt		mobile_app		spa
github			openscad		upload
```  

### touch
make a new empty file
```shell
$ ls
C++			javascript_basic	python
cinder_class		js_mvp			sass-sandbox
drive.txt		mobile_app		spa
github			openscad		upload
hue-control		openscad.md

$ touch index.html

$ ls
C++			index.html(new)		openscad.md
cinder_class		javascript_basic	python
drive.txt		js_mvp			sass-sandbox
github			mobile_app		spa
hue-control		openscad		upload
```

### cat
display file content
```shell
$ cat file_name
If you want to see a huge file
$ cat file_name | less
```

### open
open current directory with finder
```shell
$ open .

$ open file_name
If you select index.html, Terminal opens your default browser

```

### mv
move a file/folder or rename
```shell
$ mv original_file_name new_file_name
$ mv original_folder_name new_folder_name
```

### cp
copy a file/folder
```shell
$ cp original_file_name copy_file_name
$ cp -r original_folder_name copy_folder_name
```

### rm
remove a file/folder
```shell
$ rm filename
$ rm -r foldername
```

### history
display commands you hit
```shell
$ history
10864  node index.js
10865  clear
10866  npm install --save body-parser
10867  node index.js
10868  nodemon index.js
10869  ls
10870  clear


$ !10870

```

### clear
clear display
```shell
$ clear
```

### ifconfig
ifconfig is a system administration utility
```shell
$ ifconfig interface_name
$ ifconfig -a
$ ifconfig en0
```

### man
read commands manual to check options
```shell
$ man [command name]
$ man ls

NAME
     ls -- list directory contents

SYNOPSIS
     ls [-ABCFGHLOPRSTUW@abcdefghiklmnopqrstuwx1] [file ...]

DESCRIPTION
     For each operand that names a file of a type other than directory, ls
     displays its name as well as any requested, associated information.  For
     each operand that names a file of type directory, ls displays the names
     of files contained within that directory, as well as any requested, asso-
     ciated information.

     If no operands are given, the contents of the current directory are dis-
     played.  If more than one operand is given, non-directory operands are
     displayed first; directory and non-directory operands are sorted sepa-
     rately and in lexicographical order.

     The following options are available:

     -@      Display extended attribute keys and sizes in long (-l) output.
```  

scroll down   [Enter]  
close manual  q  

## Editor 

### atom
If you install atom, "atom" command will be useful
```shell
$ atom filename

$ atom .
```
"atom ." can open files that are in the current directory


### Sublime
```shell
$ sudo ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/bin/subl
you need to change Sublime Text.app -> Sublime Text 2.app or Sublime Text 3.app

If you get the message "Operation not permitted", try the following command
$ sudo ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl

open sublime text
$ subl

open folder by sublime text
$ subl .

open a file by sublime text
$ subl file_name

```  

### Visual Studio Code
You need to install command line plugin(https://code.visualstudio.com/docs/setup/mac)
```shell
$ code .

$ code file_name
```

## Python localserver
```shell
Check your python version
$ python --version

python2 default port is 8000
$ python -m SimpleHTTPServer

python3
$ python3 -m http.server
If you want use another port
$ python3 -m http.server 5000

If you prefer to use nodejs instead of python, you can install a npm package
https://www.npmjs.com/package/http-server
https://www.npmjs.com/package/simple-server
https://www.npmjs.com/package/simple-http-server

terminate
ctrl + c
```

## Version check
```shell
Git
$ git --version
git version 2.14.1

Nodejs
$ node -v
v6.11.4

npm
$ npm -v
3.10.10

Ruby
$ ruby -v
ruby 2.0.0p648 (2015-12-16 revision 53162) [universal.x86_64-darwin16]

PHP
$ php -v
PHP 5.6.30 (cli) (built: Feb  7 2017 16:18:37)
Copyright (c) 1997-2016 The PHP Group
Zend Engine v2.6.0, Copyright (c) 1998-2016 Zend Technologies

Mac OS
$ sw_vers
ProductName:	Mac OS X
ProductVersion:	10.12.6
BuildVersion:	16G29

```

## Homebrew
The missing package manager for macOS which means you can install software via Terminal.
```shell
Install 
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

$ brew install wget

```

## Option 
### Homebrew-Cask
https://caskroom.github.io/  
You can install macOS applications via Terminal like Chrome
```shell
$ brew tap phinze/homebrew-cask
$ brew install brew-cask

Install Google Chrome
$ brew cask search chrome
$ brew cask install google-chrome
```

### Reload Terminal's settings
```shell
$ ~/.bash_profile
```

## After Workshop

[command-line tutorial]  
https://www.learnenough.com/command-line-tutorial  

[basic commands]  
http://mally.stanford.edu/~sr/computing/basic-unix.html  

codecademy's command-line is good for begineers.  
https://www.codecademy.com/en/courses/learn-the-command-line/lessons/navigation/exercises/your-first-command  

[commands list]
my markdown is including how to install homebrew and nvm(node version manager)  
https://github.com/hackyGQ/ITP-Camp2015/tree/master/dev_env  

