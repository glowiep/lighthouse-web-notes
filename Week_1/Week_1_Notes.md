# Week 1 Notes
## Command Line Args
* Command-line arguments: to get user input in a program when an application is run through the CLI of an operating system.
* This is particularly useful if you want to perform large number configuration settings.
* In Node.js, alll command-line arguments received by the shell are given to the process in an array called argv (arguments-values).
  - process.argv array
<br>
<br>

Command line arguments looks like this:
```
$ [runtime] [script_name] [argument-1 argument-2 argument-3 ... argument-n]
```

### Using the process.argv Array
* This is a global object that you can use without importing any additional libraries to use it.
* 1st element - will always be a file system path pointing to the node executable. 
* 2nd element - name of the JavaScript file that is being executed. 
* 3rd element - first argument that was actually passed by the user.

<br>








# Other Notes
After forking and cloning a gist, to commit and push the edits made locally to the forked gist on remote:
* cd to the directory that contains the gist file(s)
* git add .
* git commit -m ""
* git push origin master
<br>

Note that you have a branch 'master' by default.
<br> remote: Gist does not support directories.


## Random notes
* Template literals are a time saver!