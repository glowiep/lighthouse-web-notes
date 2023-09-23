# Week 1 Notes
<details>
<summary>Command Line Args</summary>

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
</details>

<details>
<summary> Using the process.argv Array </summary>

* This is a global object that you can use without importing any additional libraries to use it.
* 1st element - will always be a file system path pointing to the node executable. 
* 2nd element - name of the JavaScript file that is being executed. 
* 3rd element - first argument that was actually passed by the user.

<br>

</details>

<details>
<summary>Do you get the Gist of it?</summary>

After forking and cloning a gist, to commit and push the edits made locally to the forked gist on remote:
* cd to the directory that contains the gist file(s)
* git add .
* git commit -m ""
* git push origin master
<br>

Note that you have a branch 'master' by default.
<br> remote: Gist does not support directories.

</details>

<details>
<summary>Falsey</summary>

All of the following are inherently falsey:
* False
* 0
* "" - an empty string is falsey
* null - a null or empty value is falsey
* undefined
* NaN - Not a number is falsey

Interesting cases:
```
false == undefined  // false
false == null       // false
NaN === NaN         //false

null == undefined   // true
' \t\r\n ' == 0     // true
0 === -0            // true
```
</details>

<details>
<summary>Functions</summary>

* Variables and constants declared with let or const are not hoisted the same way var is. 
* Let or const variables are not initialized until their definition is evaluated. Accessing them before the initialization results in a ReferenceError. 

### Global
Function *declarations* are hoisted, and that's why even though the function declaration is defined after the loop, it can be called from within the loop without any issues.
The example uses a function declaration:
```
function translateToPigLatin(word) {
  return word.slice(2, word.length) + word[0] + "ay";
}
```
### Local - Only valid after defined
Function *expressions* in JavaScript are not hoisted, which means if you try to call the function before a function expression you get an error. 
*  Function expressions oly start existing after the JavaScript interpreter reaches the line where it is defined, so they are only available after being defined.

</details>


<details>
<summary>Data Types Matter!</summary>

### What is the difference between using the for loop to push elements to a new array, versus using arr.toString().split(",")?

1. <b>For loop and push</b>: This method allows more control over the data as you are iterating over each element individually. You can make changes or apply conditions to the values before pushing them into the new array. This approach keeps the data types intact.
```

```

2. <b>toString and split</b>: This method converts every element of the array to a String using the toString() method, then separates the array into a new array where each element is split using a comma as a separator. 
* It's a quicker way to create a new array, but compared to a for loop, it provides less flexibility in terms of controlling individual element processing. 
* Also, as it converts everything to strings, you'll lose the original data type. 
* If your array contains non-string data types, like Numbers, Boolean, Objects, etc., and you want to preserve these, the toString().split(',') method is not the best choice.

```
const flatten = function(arr) {
  let newArr = arr.toString().split(",");
  return newArr;
};
```
</details>


<details>
<summary>Functions</summary>

## Growing Functions - Eloquent JavaScript
(function within a function)

## Functions & Side Effects - Eloquent JavaScript
* A pure function is a specific kind of value-producing function that not only has no side effects but also doesn’t rely on side effects from other code.
* Does not read global bindings whose value might change.
* When called with the same arguments, it always produces the same value (and doesn’t do anything else). 

## Rules to Naming Functions
* Avoid generic names like 'data', or 'run'.
* Use precise verb/action based names.
* Be consistent with naming conventions.
* Adapt existing conventions.
* Use camelCased Names.
* Properly indent code.
* Functions should focus on a single task: *returning a value* or *causing a side effect*. 

</details>

<details>
<summary></summary>
</details>


<details>
<summary></summary>
</details>


## Other notes
* Template literals are a time saver!

<center>
<img src="https://media.giphy.com/media/gbmWwWm4sGMQvAYm1G/giphy.gif" width="200">
</center>
