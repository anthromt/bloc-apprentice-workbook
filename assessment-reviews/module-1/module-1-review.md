# Module 1 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

## HTML

### Questions

1. What is HTML and what is it used for?

HTML stands for "hypertext markup language" and is used to format text styles and functionality in websites

2. What is the difference between an ID and a class?

In HTML ID applies an identity to an individual element only, while a class identity can be used for multiple elements

3. What does it mean to write "semantic" HTML?

Writing semantic HTML means using tags that describe exactly what the browser will display for the user.

### Exercises

1. Write a paragraph tag with a class of "highlight" and content "Watch out!".

<p class="highlighted"> Watch out!</p>

2. Write an HTML image tag to show an image called `profile-picture.jpg`.

<img src="profile-picture.jpg">

3. Write a link tag that links to http://google.com.

<a href="http://google.com">Google</a>

5. Write an complete standard HTML document outline (including a DOCTYPE, and `<html>`, `<head>`, and `<body>` tags).

<!DOCTYPE HTML>
<HTML>
   <HEAD>
      <TITLE>This is a webpage</TITLE>
   </HEAD>
   <BODY></BODY>
</HTML>

6. Inside of the code for the previous exercise, write the appropriate tag to link to a script file called `main.js`.

<!DOCTYPE HTML>
<HTML>
   <HEAD>
      <TITLE>This is a webpage</TITLE>
   </HEAD>
   <BODY>
    <script src="main.js"></script>
   </BODY>
</HTML>

7. Inside of the code for the previous exercise, write the appropriate tag to link to a stylesheet file called `main.css`.

<!DOCTYPE HTML>
<HTML>
   <HEAD>
      <TITLE>This is a webpage</TITLE>
        <link rel="stylesheet" href="main.css">
   </HEAD>
   <BODY>
      <script src="main.js"></script>
   </BODY>
</HTML>

8. Write a numbered list in HTML and list three of your favorite books.

<ol>
  <li>Desert Solitaire</li>
  <li>The Plague</li>
  <li>Devil in the White City</li>
</ol>

9. Fix the indentation of the following HTML sample:

  ```html
  <div>
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>
  </div>
  ```

## CSS

### Questions

1. What is CSS and what is it used for?

CSS stands for Cascading Style Sheet and it used as a tool to display html elements in a browser. 

2. What is the CSS box model?

Boxes in CSS are a way to display html elements by including them within a box that can maniuplated for color, padding, margins, etc.

3. What's the difference between margin and padding?

The margin is the area outside the box described in CSS, and padding is the area between the html elements and the inside of the box.

### Exercises

1. Write a CSS rule to make the text of all `h1` tags red.

h1 {
    color: blue;
}

2. Write a CSS rule to make the background color of the link with `class="btn"` blue:

a:link {
    background-color: blue;
}

  ```html
  <a href="#" class="btn">Learn more</a>
  ```

3. Write a CSS rule to give the first paragraph in the following HTML a font size of `20px`, but not the second paragraph

  ```html
  <header class="jumbotron">
    <style>
      p {
        font-size: 20px;
      } 
    </style>
    <p>Hello, World!</p>
  </header>

  <p>Welcome to this awesome website!</p>
  ```

## JavaScript

### Questions

1. What is a function? What are they used for?

A function in JavaScript is a bounded block of code that performs a particular task. They are used to take advantage of the structure of computers to perform many tasks at once or the same task many times.

2. What is the difference between `==` and `===`?

== describes equality of value between to variables, === describes equality of both value and type

3. What is the difference between global and local scope variables?

Global variables are variables defined in code outside of particular funcitons, they can apply to all the funcitons within the page. Local variables are variables defined only for a single function.

4. What is a boolean value?

A boolean value is a variable that can only take true or false as its value.

5. What is an array?

An array is a tool in Javascript that can contain multiple values within one variable.

### Exercises

1. Write a line that declares a variable called `myName` and set its value to your name.

var myName = "Steve";

2. Write a loop that logs the numbers 1 through 10 to the console.
 
var x;

for (var x = 1; x <= 10; x++) {
    console.log(x);
}

3. Translate the following pseudocode into JavaScript: if `score` is greater than `3` and `lives` is greater than `0`, alert "You win!".

var score;
var lives;

if (score > 3 && lives > 0) {
  alert = "You win!"};

4. Write a function `sayHello` that takes one argument, a name, and logs "Hello, <name>!" to the console. Then, call the function below the function definition and pass in your name as the argument.

function sayHello (name) {
  return "Hello," + name + "!";
  }

sayHello(Steve);

5. What would the following script log to the console?

  ```javascript
  var currentSong = "Call Me Maybe";

  function setSong(song) {
    currentSong = song;
  }

  setSong("Friday, Friday");

  console.log(currentSong);
  ```
  
"Call Me Maybe"


6. What would the following script log to the console?

  ```javascript
  var add = function(a, b) {
    return a + b;
  }

  var result = add(3, 7);

  console.log(result);

  ```
10

7. What would the following script log to the console?

  ```javascript
  var helloGoodbye = function(name) {
    return sayHello(name) + " " + sayGoodbye(name);
  }

  var sayHello = function(name) {
    return "Hello " + name " !";
  }

  var sayGoodbye = function(name) {
    return "Goodbye " + name " !";
  }

  console.log(helloGoodbye("Sarah"));
 
  ```
  Hello Sarah! Goodbye Sarah!

8. Write a function `findLongestWord()` that takes an array of words and returns the length of the longest one.

var findLongestWord = function(array) {
  var words = array.length;
  var number = 0;
  for (x = 0; x < words; x++) {
    if (array[x].length > number) 
      number = array[x].length;
  }
  return number;
}

9. Define a function `sum()` that sums all the numbers in an array of numbers. For example, `sum([1,2,3,4])` should return 10.

var sum = function(array) {
  var length = array.length;
  var total = 0;
  for (x = 0; x < length; x++) {
    total += array[x];
  }
  return total;
};

10. Write a function that takes a character (i.e. a string of length 1) and returns true if it is a vowel, false otherwise.
11. Write the correct line to make `"Woof!"` show up in the console based on this script:

  ```javascript
  var pet = {
    name: "Charles",
    goodDog: true,
    speak: function() {
      console.log("Woof!");
    }
  };
  ```

12. Using the same script as above, write the correct line to log the dog's name to the console.

## Command Line

### Questions

1. What is the command line and what is it used for?

The command line is the tool on a computer that allows the use to manipulate files on a computer

2. What does the command `ls` do?

ls lists files 

3. What does the command `pwd` do?

names the current directory

4. What does the following command do: `cd my-cool-project`

changes the location to the directory named "my-cool-project"

### Exercises

1. Write the command to make a new directory called "my-cool-project".

mkdir my-cool-project

2. Write the command to create a file called "index.html".

touch index.html

3. Write the command to delete a file called "main.css".

rm main.css

## Git

### Questions

1. What is Git and what is it used for?

Git is a collaborative work tool that allows developers to share and work together on common files and projects

2. What's the difference between a local repository and a remote repository?

The local repository are the files that a single user is working on located only on his or her computer, the remote repository is where users who are working in common 'push' or 'pull' common files for all to access

### Exercises

1. Write the command that you would use to create a new local Git repository.

git init

2. Write the command to stage a file called `index.html` to be committed.

git commit -m 

3. Write the command to view the current status of the git repository.

git checkout
