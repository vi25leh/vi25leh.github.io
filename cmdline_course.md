---
layout: default
---

# The Command-line Course

The Command-line course serves as an introduction to working on the command-line and using the terminal for executing different kinds of tasks. The starting point is the very basic commands to handle directories and files. From there the contents shift into more complex commands and combining them in order to modify files and create new ones with a specific purpose. Then scripting is introduced alongside with environment variables and configuration files. This allows the modification of the terminal for a more efficient and personalised experience on the command-line. Installing software allows for executing programs and retrieving specific information from files. After that, the use of remote servers and their benefits is discussed. The course ends with the theme of version control and GitHub. The final project of creating a personal webpage with GitHub Pages allows the student to put all the knowledge acquired throughout the course into use.

The methods learned on this course can be very useful for linguists who use technological tools in their work/studies and want to find ways to work more efficiently. 

#### Contents of the course

| *MODULE*      | *THEMES*    |
| ------------- |:-------------:|
| Module 1 | setting up the command-line, basic commands for directories and text files |
| Module 2 | encoding systems, text file operations, regular expressions, piping for combining commands    |
| Module 3 | scripting, modifications to .bshrc-file, becoming the root user, installing software and python packages      |
| Module 4 | remote servers, GitHub and version control, GitHub pages |


## Module 1: Introduction to Command-line Environments

During the first module, we went through the very basics of the command-line starting from setting up the terminal on our own devices.

### Contents

* Directories
    * Getting familiar with the root directory and its functions
    * Creating, removing and copying directories
    * Displaying the contents of a directory
    * Changing the contents of a directory
* Files
    * Creating, copying, renaming and moving files
    * Displaying the contents of a text file using '$ less'
    * Opening and editing a text file on a text editor
    * Retrieving files from the internet using '$ wget':
````
$ wget https://linktothefile.txt
````
        * The 'wget'-command downloads the retrieved file from the internet into the current directory


### Reflection

This module introduced me to the essential commands and operations that can be executed on the command-line. I also learned about different operating systems and how these can be operated through the terminal. In addition to knowing the basic commands to managing files, I also got to learn about the permissions of a file; how to display and modify them.

## Module 2: Text Processing in UNIX

In the second module the different character encoding systems were discussed and their differences were compared. Then some more complex commands were introduced for a more complex file management and edition. For example, frequency lists are created by combining said commands, which can be useful in creating a corpus.

### Contents

* Encoding systems
    * Introduction to the similarities and differences of the Latin-1, ASCII and UTF-8 encoding systems
    * Changing the encoding system of a file into another
* File operations
    * Printing certain lines from a file
    * Sorting lines
    * Finding lines that include a certain character/type of character/combination of characters
    * Transforming certain characters in a file
    * Cutting and pasting columns
* Text Processing
    * Using '$ sed' for
        * deleting lines and finding and replacing patterns
        * piping commands
        * using regular expressions
* Linguistic Tasks
    * Creating a frequency list

Example of finding certain words in a text file:
````
$ egrep "\b[a-zåäö]*nen\ finnishsurnames.txt > nensurnames.txt
````
In this example, we take a text file called "finnishsurnames.txt" where each line consists of one Finnish surname. We want to find out which surnames end in the common suffix "-nen". We use the command 'egrep' to find patterns in our chosen file. We have determined the pattern with the help of regular expressions. The pattern we want to find is a sequence of characters that ends in the suffix "-nen". The command finds all instances of this in the file and prints the results in a new file called "nensurnames.txt"
### Reflection

This module deepened my understanding of everything we're capable of doing on the command-line. I found the regular expressions and piping commands very useful. I didn't know beforehand how versatile the tasks performed through piping could be. I was surprised how I would be able to benefit from these commands in my own linguistic research work.

## Module 3

In the third module, the main themes were scripting and installing software. The basics of scripting were taught and the concepts of configuration files and environment variables were discussed. Later on, the process of installing software and different packages was gone through.

### Contents

* Scripting
    * Writing simple scripts with/without if-statements or while-loops
* Configuration file
    * Making changes to the appearance of the command-line
    * Making settings (e.g. regarding variables) permanent
* Environment variables
    * Displaying current variable values
    * Changing variable values and defining new ones
* Installing software
    * Using '$ apt-get'
    * Installing python packages with '$ pip'

Creating a shortcut for accessing the command-line course directory 'cmdline-course':
* Enter your .bashrc-file
* Create the shortcut for the environment variable 'PATH':

````
$ export PATH=$PATH:~/home/username/cmdline-course
````

### Reflection

This module gave me a better understanding of my own operating system and how to navigate it. I also learned how to make my experience on the command-line more personalised, which is nice. Installing packages will definitely be useful in the future when executing tasks.

## Module 4

The fourth and the last module discussed remote servers and their utility for working on projects. However, the main part of this module was version control with Git and GitHub. This knowledge was put into use by getting to create an own webpage using GitHub.

### Contents
* Remote servers
    * Connecting and exiting
    * Copying files from a server
* Version control
    * What is it and what is it used for?
    * GitHub
        * Creating and cloning a repository
        * Working locally on your own command-line
        * Adding files to a repository
        * Commiting changes and pushing them to the global repository in GitHub
        * Undoing changes
        * Handling branches

Process of transferring changes made locally into the global repository in GitHub:

1. Add already made changes and modifications to the staging area with
2. Check the staging area status
3. Commit the changes
4. Push the changes from the staging area to the global repository in GitHub

````
1. $ git add nameofthemodifiedfile.md
2. $ git status
3. $ git commit -m 'comment on the changes made'
4. git push
````

### Reflection

I think this last module was my favorite since I got to put all the knowledge acquired throughout this course into practical use. I really enjoyed creating my own webpage on GitHub and learning about version control.



![alt text](https://i.programmerhumor.io/2022/11/programmerhumor-io-linux-memes-programming-memes-5ac17db28234935.png "Command-line Meme")
