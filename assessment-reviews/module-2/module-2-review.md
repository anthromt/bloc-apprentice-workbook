# Module 2 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

*Note: any topics from the first assessment should be reviewed in addition to the questions below!*

## CSS

### Questions

1. What is the box model?

The box model is a layout in CSS that places HTML elements in "boxes" that can be manipulated in different ways (margin, border, etc.)

2. What is the difference between block and inline elements?

Block level elements are applied to an entire block of HTML within a body, while inline elements appear only in individual lines

3. What is responsive design?

Responsive design is the web design philosophy that says user behavior should drive the design of a web page

4. Which selector is more specific, a tag selector or class selector?

Class selector

5. What does `box-sizing` do?

Box sizing is an efficient way in CSS to maniupluate the size and shape of box elements including height, width, etc.

6. What's the difference between `relative` and `absolute` positioning?

Elements that have absolute positioning stay in place regardless of how the page is moved, and with regard to other elements around them, elements with relative positioning can change their location on the page with regards to other elements

### Exercises

1. Write a CSS rule to turn the background color of the link with the `.btn` class blue on hover:

  ```html
  <a href="#" class="btn">Learn more</a>
  ```

btn:hover { 
    background-color: blue;
}

2. Write a CSS rule to give the `.container` a maximum width of `980px` when the browser window is wider than `1200px`:

  ```html
  <div class="container">
    <h1>I'm a heading!</h1>
  </div>

.container {
    width: 980px;
    box-sizing: border-box;
///not sure about the browser window
}

3. Which text would be red in the following example?

  ```html
  <style>
    section p:last-child {
      color: red;
    }
  </style>

  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  ```
 
  Third Paragraph

4. Open this [JSBin](http://jsbin.com/qigiwuhepe/1/edit?html,css,output). Write a CSS rule using floats to make the HTML sample into a four column layout. Paste your udpated link below.

I can't get this bin to open

## JavaScript

### Questions

1. What is a callback?

A callback is a function that is passed into another function as variable

### Exercises

1. Write a function `filterLongWords()` that takes an array of words and an integer `num` and returns the array of words that are longer than `num`.


var filterLongWords = function(array, num){
  var length = array.length;
  var longestWords = [];
  for (i = 0; i < length; i++) {
    if (array[i].length > num) {
      longestWords[longestWords.length] = array[i];
    }
  }
  return longestWords;
}


2. Write a function `charFreq()` that takes a string and builds a frequency listing of the characters contained in it. Represent the frequency listing as a Javascript object. Try it with something like `charFreq("abbabcbdbabdbdbabababcbcbab")`.


var charFreq = function(string){
  var list = {};
  var length = string.length;
  for (var i = 0; i < length; i++) {  
  if 
  else 
    list;
  }
  return list;
}

## DOM Scripting

### Questions

1. What does DOM stand for and what is it?

The DOM stands for Document Object Model, and using JavaScript it can change all the elements of an HTML file

### Exercises

1. Write a JavaScript statement that finds the element with the ID, `next`, and saves it to a variable called `nextButton`:

  ```html
  <a href="#" id="next" class="btn">Next</a>
```
<script>
var nextButton = "next";
</script>

3. Write another line that adds a click event listener to `nextButton` so that when it's clicked the browser alerts `"Next image coming up."`.

document.getElementById("nextButton").addEventListener("click", "Next image coming up.");

## jQuery

### Questions

1. What is a JavaScript library and why do we use them?

A Javascript library is a pre-selected set of javascript code that's efficiently deployable in websites to create a large number of elements all at once without having to code each element individually

2. What is jQuery for?

JQuery is a javascript library, and it takes tasks that require a lot of JavaScript code to write, and puts them into methods that can be used just one line of code.



### Exercises

1. Write a statement to select all elements with the `.btn` class using a jQuery selector and save them to a variable called `buttons`:

  ```html
  <a href="#" id="next" class="btn">Next</a>
  <a href="#" id="beginning" class="btn">Beginning</a>
  <a href="#" id="previous" class="btn">Previous</a>
 
    $(".btn").var = buttons
    
2. Write another line that adds a click event to the buttons that logs `'click'` to the console when the button is clicked. Use the jQuery syntax.

    $(".btn").click(function(){
        $(".btn")."click"();
    });


## Angular

### Questions

1. How is a framework different than a library?
2. What is a controller?
3. What is a view?
4. What is a single page application?
5. What is a directive in Angular?

## Git

### Exercises

1. Write a command to create a new branch called `bug-fix`.

$git checkout -b bug-fix

2. If you're on the `master` branch, write a command to merge a branch called `bug-fix` into the `master` branch.

$git checkout master
$git merge bug-fix
