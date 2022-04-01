> Brace yourself for more rules.

- The firest character of a variable name must be a letter, underscore(\_), or a dollar sign($)(Subsequent characters can be letters, digits, underscorse, or dollar signs).
- The first character of a variable name can't be a number.
- Variable names can't include a mathematical or logical operator in their name. For instance, 2\*something or this + that'
- Variable names can't contain spaces.
- You're not allowed to use any special symbols, like my#num, num%, etc/
- JavaScript is a hyphen free zone. They're reserved for subtractions.

1. Strings
   > backslash '\' escape character.

| code | outputs         |
| ---- | --------------- |
| \'   | single quote    |
| \"   | double quote    |
| \\   | backslash       |
| \n   | new line        |
| \r   | carriage return |
| \t   | tab             |
| \b   | backspace       |
| \f   | form feed       |

2. Boolean

   > The Boolean value of 0 (zero), null, undefined, empty string is false. Everything with a "real" value is true.

3. Arithmetic Operators

| Operator | Description    | Example                     |
| -------- | -------------- | --------------------------- |
| +        | Addition       | 25 + 5 = 30                 |
| -        | Subtraction    | 25 - 5 = 20                 |
| x = \*   | Multiplication | 10 x 20 = 200               |
| /        | Division       | 20 / 2 = 10                 |
| %        | Modulus        | 56 % 3 = 2                  |
| ++       | Increment      | var a = 10; a++; Now a = 11 |
| --       | Decrement      | var a = 10; a--; Now a = 9  |

> 10 _ '5' or '10' _ '5' will give the same result. But trying to multiply a number with string values that aren't numbers, like 'sololearn' \* 5 will return NaN(Not a Number).

4. Assignment Operators

| Operator | Example | Is equivalent to |
| -------- | ------- | ---------------- |
| =        | x = y   | x = y            |
| +=       | x += y  | x = x + y        |
| -=       | x -= y  | x = x-y          |
| `*`=     | x `*`=y | x =x `*` y       |
| /=       | x /= y  | x = x / y        |
| %=       | x %= y  | x = x % y        |

> > You can use multiple assignment operators in one line, such as x -= y += 9.

5. Comparison Operators
   > You get either true or false. The equal to '==' operator checks whether the operands' values are equal.
   >
   > > You can compare all types of data with comparison operators, they'll always return true or false.

| Operator | Description                       | Example         |
| -------- | --------------------------------- | --------------- |
| ==       | Equal to                          | 5 == 10 false   |
| ===      | Identical(equal and of same type) | 5 === 10 false  |
| !=       | Not equal to                      | 5 != 10 true    |
| !==      | Not Identical                     | 10 !== 10 false |
| >        | Greater than                      | 10 > 5 true     |
| >=       | Greater than or equal to          | 10 >= 5 true    |
| <        | Less than                         | 10 < 5 false    |
| <=       | Less than or equal to             | 10 <= 5 false   |

6. Logical Operators

| Logical Operators |                                                                          |
| ----------------- | ------------------------------------------------------------------------ |
| &&, And           | Returns true, if both operands are true                                  |
| Or                | Returns true, if one of the operands is true                             |
| ! Not             | Returns true, if the operand is false, and false, if the operand is true |

> > You can check all types of data; comparison operators always return true or false

7. The For Loop

```js
for (statement1; statement2; statement3) {
   code block to be executed
}
```

| a          | b                                                                     |
| ---------- | --------------------------------------------------------------------- |
| statement1 | is excuted before the loop(the code block) starts                     |
| statement2 | defines the condition for running the loop(the code block)            |
| statement3 | is executed each time after the loop(the code block)has been executed |

8. Do While Loop

```js
var i = 20;
do {
  document.write(i + "<br/");
  i++;
} while (i <= 25);
```

> > Note the semicolon used at the end of the do...while loop. This is important.
> > The loop will always be excuted at least once, even if the condition is false, because the code block is excuted before the condition is tested.

9. Break
   > We've met the break statement earlier in this module, we use it to "jump out"of a loop and continue executing the code after the loop.

```js
for (i = 0; i <= 10; i++>) {
   if (i == 5) {
      break;
   }
   document.write(i + "<br/>")
}

// 0
// 1
// 2
// 3
// 4
```

> > You can use the return keyword to return some balue immediately from the loop inside of a function. This will also break the loop.

10. Continue.
    > We're nearly done with module3. One last thing to cover. Unlike the break statement, the continue statement breaks only one iteration in the loop, and continues with the next iteration.

```js
for (i = 0; i <= 10; i++) {
  if (i == 5) {
    continue;
  }
  document.write(i + "<br/>");
}
// 0
// 1
// 2
// 3
// 4
// 6
// 7
// 8
// 9
// 10
```

11. Defining a Function

    > To define a JavaScript function, use the function keyword, followed by a name, followed by a set of "parentheses()". The code to be executed by the function is placed inside curly brackets {}.
    >
    > > Function names can contain letters, digits, underscores, and dollar signs (same rules as variables.)

12. Calling a Function

    > To execute the function, you need to call it. To call a function, start with the name of the function, then follow it with the arguments in parentheses.
    >
    > > Always remember to end the statement with a semicolon after calling the function.

13. Calling Functions

    > Once the function is defined, JavaScript allows you to call it as many times as you want to.
    >
    > > You can also call a function using this syntax: myFunction.call(). The difference is that when calling in this way, you're passing the 'this' keyword to a function. You'll learn about it later.

14. Function Parameters

    > > As with variables, parameters should be given names, which are separated by commas within the parentheses.

15. Using parameters
    > After defining the parameters, you can use them inside the function.

```js
function sayHello(name) {
  alert("Hi," + name);
}

sayHello("David");
```

> > This function takes in one parameter, which is called name. When calling the function, provide the parameter's value (argument) inside the parentheses.

> > > Function arguments are the real values passed to (and received by) the function.

16. Function Parameters
    > You can define a single function, and pass different parameter values(arguments) to it.

```js
function sayHello(name) {
  alert("Hi," + name);
}
sayHello("David");
sayHello("Sarah");
sayHello("John");
```

> > This will execute the function's code each time for the provided argument.

17. Multiple Parameters
    > If you pass more arguments than are defined, they will be assigned to an array called arguments. They can be used like this: arguments[0], arguments[1], etc.

> > If a function is called with missing arguments (fewer than declared), the missing values are set to undefined, which indicates that a variable has not been assigned a value.

18. Function Return
    > A function can have an optional return statement. It is used to return a value from the function. This statement is useful when making calculations that require a result.

> When JavaScript reaches a return statement, the function stops executing.

> Use the return statement to return a value. For example, let's calculate the product of two numbers, and return the result.

```js
function myFunction(a, b) {
  return a * b;
}

var x = myFunction(5, 6);
// Return value will end up  in x
```

> > If you do not return anything from a function, it will return undefined.

19. Three types of popup box => Alert, Prompt, Confirm

- Alert: When an alert box pops up, the user music click OK to proceed. The alret function takes a single parameter, which is the text displayed in the popup box.

- Prompt: When a prompt box pops up, the user will have to click either OK or Cancel to proceed after entering the input value. If the user clicks OK, the box returns the input value. If the user clicks Cancel, the box returns null.

  > The prompt() method takes two parameters.

  - the first is the label, which you want to display in the text box.
  - The second is a default string to display in the text box(optional).
    > > Do not overuse this method, because it prevents the user from accessing other parts of the page until the box is closed.

- Confirm Box
  > A confirm box is often used to have the user verify or accept something. When a confirm box pops up, the user must click either OK or Cancel to proceed. If the user clicks OK, the box returns true. If the user clicks Cancel, the box returns false.

20. Object Properties
    > You can access object properties in two ways.

```js
objectName.propertyName;
// or
objectName["propertyName"];
```

```js
var person = {
  name: "John",
  age: 31,
  favColor: "green",
  height: 183,
};

var x = person.age;
var y = person["age"];

console.log(x);
console.log(y);

// 31
// 31
```

> > Objects are one of the core concepts in JavaScript.

21. The Object Constructor.
    > In the preivious lesson, we created an object using the object literal(or initializer) syntax.

```js
var person = {
  name: "John",
  age: 42,
  favColor: "green",
};
```

> This allows you to create only a single object. Sometimes, we need to set an "object type" that can be used to create a number of objects of a single type. The standard way to create an "object type" is to use an object constructor function.

```js
function person(name, age, color) {
  this.name = name;
  this.age = age;
  this.favColor = color;
}
```

> The above function (person) is an object constructor, which.takes parameters and assigns them to the object properties.

> > The this keyword refers to the current object. Note that this is not a variable. It is a keyword, and its value cannot be changed.

22. Creating Objects
    > Once you have an object constructor, you can use the new keyword to create new objects of the same type.

```js
var p1 = new person("John", 41, "green");
var p2 = new person("Amy", 21, "red");

console.log(p1.age); // outputs 41
console.log(p2.name); // outputs "Amy"
```

> > p1 and p2 are now objects of the person type. Their properties are assigned to the corresponding values.

23. Object Initialization
    > Use the object literal or initializer syntax t ocreate single objects.

```js
var John = { name: "John", age: 25 };
var James = { name: "james", age: 21 };
```

> > Objects consist of properties, which are used to describe an object. Values of object properties can either contain primitive data types or other objects.

24. Methods
    > Methods are functions that are stored as object properties. Use the following syntax to create an object method:

```js
methodName = function () {
  codeline;
};
```

> Access an object method using the following syntax:

```js
objectName.methodName();
```

> A method is a function, belonging to an object. It can be referenced using the this keyword. The this keyword is used as a reference to the current object, meaning that you can access the objects properties and methods using it. Defining methods is done inside the constructor function.

```js
function person (name, age) {
  this.name = name;
  this.age = age;
  this.changeName = fuinction (name) {
    this.name = name;
  }
}

var p = new person("David", 21);
p.changeName("John");
// Now p.name equals to "John"
```

> In the example above, we have defined a method named changeName for our person, which is a function, that takes a parameter name and assign it to the name property of the object. this.name refer to the name property of the object.

> > The changeName method changes the object's name property to its argument.

25. Methods
    > You can also define the function outside of the constructor function and associate it with the object.

```js
function person(naem, age) {
  this.name = name;
  this.age = age;
  this.yearOfBirth = bornYear;
}

function bornYear() {
  return 2016 - this.age;
}
```

> > As you can see, we have assigned the object's yearOfBirth property to the bornYear function. The this keyword is used to access the age property of the object, which is going to call the method.

> > Note that it's not necessary to write the function's parentheses when assigning it to an object.

```js
function person(name, age) {
  this.name = name;
  this.age = age;
  this.yearOfBirth = bornYear;
}
function bornYear() {
  return 2016 - this.age;
}

var p = new person("A", 22);
console.log(p.yearOfBirth());

// 1994
```

> > Call the method by the property name you specified in the constructor function, rather than the function name.

26. JavaSCript Arrays

    > Array store multiple values in a single variable. To store
    >
    > > Array and new keywords create an array

27. Accessing an Array
    > You refer to an array element by referring to the index number written in square brackets. This statement accesses the value of the first element in courses and changes the value of the second element.

```js
var courses = new Array("HTML", "CSS", "JS");
var course = courses[0]; // HTML
courses[1] = "C++"; // Changes the second element.
```

> > [0]is the first element in an array. [1] is the second. Array indexes start with 0

> Attempting to access an index outside of the array, returns the value undefined

```js
var course = new Array("HTML", "CSS", "JS");
console.log(course[10]);

// undefined
```

> > Our couse array has just 3 element, so the 10th index, which is the 11th element, does not exist(is undefined).

28. Creating Arrays
    > You can also declare an array, tell it the number of elements it will store, and add the elements later.

```js
var courses = new Array(3);
courses[0] = "HTML";
courses[1] = "CSS";
courses[2] = "JS";
```

> > An array is a special type of object. An array uses numbers to access its elements, and an object uses names to access its members.

> JavaScript arrays are dynamic, so you can declare an array and not pass any arguments with the Array() constructor. You can then add the elements dynamically.

> > You can add as many elements as you need to.

29. Array Literal
    > For greater simplicity, readability, and execution speed, you can also declare arrays using the array literal syntax.

```js
var courses = ["HTML", "CSS", "JS"];
```

> This result in the same array as the one created with the new Array() syntax.

> > You can access and modify the elements of the array using the index number, as you did before. The array literal syntax is the recommended way to declare arrays.

29. The Length Property
    > JavaScript arrays have useful built-in properties and methods. An array's length property returns the number of it's elements.

> > The length property is always one more than the highest array index. If the array is empty, the length property returns 0.

30. Combining Arrays
    > JavaScript's concat() method allows you to join arrays and create an entirely new array.

```js
var c1 = ["HTML", "CSS"];
var c2 = ["JS", "C++"];
var courses = c1.concat(c2);
console.log(courses);

// [ 'HTML', 'CSS', 'JS', 'C++' ]
```

> The courses array that results contains 4 elements(HTML, CSS, JS, C++)
>
> > The concat operation does not affect the c1 and c2 arrays -it returns the resulting concatenation as a new array.

31. Associative Arrays
    > While many programming languages support arrays with named indexes (text instead of numbers), called associative arrays JavaScript does not. However, you still can use the named array syntax, which will produce an object.

```js
var person = []; // empty array
person["name"] = "John";
person["age"] = 46;
console.log(person["age"]);

// 46
```

> Now, person is treated as an object, instead of being an array. The named indexes "name" and "age" become properties of the person object.

> > As the person array is treated as an object, the standard array methods and properties will produce incorrect results. For example, person.length will return 0.

> Remember that JavaScript does not support arrays with named indexes. In JavaScript, arrays always use numbered indexes. It is better to use an object when you want the index to be a string(text). Use an array when you want the index to be a number.
>
> > If you use a named index, JavaScript will redefined the array to a standard object.

32. The Math Object
    > The Math oject allows you to perform mathematical tasks, and includes several properties.

| Property | Description                            |
| -------- | -------------------------------------- |
| E        | Euler's constant                       |
| LN2      | Natural log of the value 2             |
| LN10     | Natural log of the value 10            |
| LOG2E    | The base 2 log of Euler's constant (E) |
| LOG10E   | The base 10 log of Euler's constant(E) |
| PI       | Returns the constant PI                |

```js
console.log(Math.PI);

// 3.141592653589793
```

> > Nath has no constructor. There's no need to create a Math object first.

33. Math Object Methods
    > The Math object contains a number of methods that are used for calculations:

| Method           | Description                                                                   |
| ---------------- | ----------------------------------------------------------------------------- |
| abs(x)           | REturn the absolute value of x                                                |
| acos(x)          | Return the arccosine of x, in radians                                         |
| asin(x)          | Returns the arccosine of x, in radians                                        |
| atan(x)          | Returns the arctangent of x as a numeric value between -PO/2 and PI/2 radians |
| atan2(y,x)       | Returns the arcangent of the quotient of its argumennts                       |
| ceil(x)          | Returns x, rounded upwards to the nearest integer                             |
| cos(x)           | Returns the cosine of x(x is in radians)                                      |
| exp(x)           | Returns the value of E^x                                                      |
| floor(x)         | Retruns x, rounded downwards to the nearest integer                           |
| log(x)           | Returns the natural logarithm (base E) of x                                   |
| max(x,y,x,...,n) | Returns the number with the heightest values                                  |
| min(x,y,z,...,n) | Returns the number with the lowest value                                      |
| pow(x,y)         | Returns the value of x to the power of y                                      |
| random()         | Returns a random number between 0 and 1                                       |
| round(x)         | Rounds x to the nearest integer                                               |
| sin(x)           | Returns the sine of x (x is in radians)                                       |
| sqrt(x)          | Returns the square root of x                                                  |
| tan(x)           | Returns the tangent of an angle                                               |

> > Toi get a random number between 1-10, use Math.random(), which gives you a number between 0-1. Then multiply the number by 10, and then take Math.ceil() from it: Math.ceil(Math.random() \* 10).
> > Math is a handy object. You can save a lot of time using Math, instead of writing your own functions every time.

34. Date Methods
    > when a Date object is created, a number of methods make it possible to perform perations on it.

| Method            | Description               |
| ----------------- | ------------------------- |
| getFullYear()     | get the years             |
| getMonth()        | gets the month            |
| getDate()         | gets the day of the month |
| getDay()          | gets the day of the week  |
| getHours()        | gets the hour             |
| getMinutes()      | gets the minutes          |
| getSeconds()      | get the seconds           |
| getMilliseconds() | get the milliseconds      |

35. The DOM
    > When you open any webpage in a browser, the HTML of the page is loaded and rendered visually on the screen. To accomplish that, the browser builds the Document Object Model of that page, which is an object oriented model of its logical structure. The Dom of an HTML document can be represented as a nested set of boxes.

[The DOM](./The_DOM.png)

> > JavaScript ca be used to manipulate the DOM of a page dynamically to add, delete and modify elements.

36. DOM Tree
    > The DOM represents a document as a tree structure. HTML elements become interrelated nodes in the tree. All those nodes in the tree have some kind of relations among each other. nodes can have child nodes. Nodes on the same tree level are called siblings. For example, consider the following structure.

<img href="./The_DOM.png">

> For the example above:

- html tag has two children (head tag, body tag);
- head tag has one child (title tag) and one parent (html tag);
- title tag has one parent (head tag) and no children;
- body tag has two children (h1 tag and a tag) and one parent (html tag);

> > It is important to understand the relationships between elements in an HTML document in order to manipulate them with JavaScript.

37. The document Object
    > There is a predefined document object in JavaScript, which can be used to access all elements on the DOM. In other words, the document object is the owner(or root) of all objects in your webpage. So, if you want to access objects in an HTML page, you always start with accessing the document object.

```js
document.body.innerHTML = "some text";
```

> As body is an element of the DOM, we can access it using the documents object and change the content of the innerHTML property.

> > The innerHTML property can be used on almost all HTML elements to change its content.

38. Selecting Elements
    > All HTML elements are objects. And as we know every object has properties and Methods. The document object has methods that allow you to select the desired HTML element. These three methods are the most commonly used for selecting HTML elements:

```js
// finds element by id
document.getElemenById(id);

//finds elements by class name
document.getElementsByClassName(name);

// finds elements by tag name
document.getElementsByTagName(name);
```

> Im the example below, the getElementById method is used to select the element with id="demo" and change its content:

```js
var elem = document.getElementById("demo");
elem.innerHTML = "Hello World!";
```

> > The example above assumes that the HTML contains an element with id="demo", for example '<div id="demo"></div>'

38. Selecting Elements
    > The getElementsByClassName() method returns a collection of all elements in the document with the specified class name. For example, if our HTML page contained three elements with class="demo", the following code would return all those elements as an array:

```js
var arr = document.getElementsByClassName("demo");
// accessing the second element
arr[1].innerHTML = "Hi";
```

> Similarly, the getElementsByTagName method returns all of the elements of the specified tag name as an array. The following example gets all paragraph elements of the page and changes their contetn:

```js
<p>hi</p>
<p>hello</p>
<p>hi</p>
<script>
var arr = document.getElementsByTagName("p");
for (var x = 0; x < arr.length; x++) {
  arr[x].innerHTML = "Hi there";
}
</script>
```

> The script will result in the following HTML:

```js
<p>Hi there</p>
<p>Hi there</p>
<p>Hi there</p>
```

> > we used the length property of the array to loop through all the selected elements in the above example.

39. Working with DOM
    > Each element in the DOM has a set of properties and methods that provide information about their relationships in the DOM:

- element.childNodes returns an array of an array of an element's child nodes.
- element.firstChild returns the first child node of an element.
- element.lastChild returns the last child node of an element.
- element.hasChildNodes returns true if an element has any child nodes, otherwise false.
- element.nextSibling retruns the next node at the same tree level.
- element.previousSibling returns the previous node at the same tree level.
- element.parentNode returns the parent node of an element.

> We can, for example, select all child nodes of an element and change their content:

```js
<html>
  <body>
    <div id = "demo">
      <p>some text</p>
      <p>some other text</p>
    </div>

    <script>
    var a = document.getElementById("demo");
    var arr = a.childNodes;
    for (var x = 0; x<arr.length; x++) {
      arr[x].innerHTML = "new text";
    }
    </script>
  </body>
</html>
```

> > The code above changes the text of both paragraphs to "new text".

40. Changing Attributes
    > Once you have selected the element(s) you want to work with, you can change their attributes. As we have seen in the previous lessons, we can change the text content of an element using the innerHTML property. Similarly, we can change the attributes of elements. For exampe, we can change the src attribute of an image:

```js
<img id="myimg" src="orange.png" alt="" />
<script>
var el = document.getElementById("myimg");
el.src = "apple.png"
</script>
```

> We can change the href attribute of a link:

```js
<a href="http://www.example.com"> Some link</a>
<script>
var el = document.getElementByTagName("a");
el[0].href = "http://www.sololearn.com";
</script>
```

> > Practically all attributes of an element can be changed using JavaScript.

41. Changing Style
    > The style of HTML elements can also be changed using JavaScript. All style attributes can be accessed using the style object of the element.

```js
<div id="demo" style="width:200px">some text</div>
<script>
var x = document.getElementById("demo");
x.style.color="6600FF";
x.style.width="100px";
</script>
```

> The code above changes the text color and width of the div element.

> > All CSS properties can be set and modified using JavaScript. Just remember, that you cannot use dashes (-) in the property names: these are replaced with camelCase versions, where the compound words begin with a capital letter. For example: the background-color property should be referred to as backgroundColor.

42. Creating Elements
    > Use the following methods to create new nodes: element.cloneNode() clones an element and returns the resulting node. document.createElement(element) creates a new element node. document.createTextNode(text) create a new text node.

```js
var node = document.createTextNode("Some new text");
```

> This will create a new text node, but it will not appear in the document until you append it to an existing element with one of the following methods: element.appendchild(newNode) add a new child node to an element as the last child node. element.insertBefore(node1, node2) inserts node1 as a child before node2.

```js
<div id ="demo">some content</div>

<script>
//creating a new paragraph
var p = document.createElement("p");
var node = docuemnt.createTextNode("Some new text");
//adding the paragraph to the div
div.appenChild(p);
</script>
```

> > This creates a new paragraph and adds it to the existing div element on the page.

43. Removing Elements
    > To remove an HTML element, you must select the parent of the element and use the removeChild(node) method.

```js
<div id="demo">
  <p id="p1">This is a paragraph</p>
  <p id="p2">This is another paragraph</p>
</div>

<script>
var parent = docuemnt.getElementById("demo");
var child = docuemnt.getElementById("p1");
parent.removeChild(child);
</script>
```

> This removes the paragraph with id="p1" from the page.

> > An alternative way of achieving the same result would be the use of the parentNode property to get the parent of the element we want to remove: var child = document.getElementById("p1"); child.parentNode.removeChild(child);

44. Replacing Elements
    > To replace an HTML element, the element.replaceChild(newNodes, oldNode) method is used.

```js
<div>
  <p id="p1">This is a paragraph.</p>
  <p id="p2">This is another paragraph</p>
</div>

<script>
var p = document.createElement("p");
var node = document.createTextNode("This is new");
p.appenChild(node);

var parent = document.getElementById("demo");
var child = document.getElementById("p1");
parent.replaceChild(p, child);
</script>
```

> > The code above creates a new paragraph element that replaces the existing p1 paragraph.

45. Handling Events
    > You can write JavaScript code that executes when an event occurs, such as when a user clicks an HTML element,. moves the mouse, or submits a form. when an event occurs on a target element, a handler function is executed. Common HTML events include:

| Event       | Description                                                                                  |
| ----------- | -------------------------------------------------------------------------------------------- |
| onclick     | occurs when the user clicks on an element                                                    |
| onload      | occurs when an object has loaded                                                             |
| onunload    | occurs once a page has unloaded                                                              |
| onchange    | occurs when the contetn of a form element, the selec-tion, or the checked state have changed |
| onmouseover | occurs when the pointer is moved onto an element, or onto one of its children                |
| onmouseout  | occurs when a user moves the mouse pointer out of an element, or out of one of its children  |
| onmousedown | occurs when the user presses a mouse button over an element                                  |
| onmouseup   | occurs when a user release a mouse button over an element                                    |
| onblur      | occurs when an element loses focus                                                           |
| onfocus     | occurs when an element gets focus                                                            |

> > Corresponding events can be added to HTML elements as attributes.

46. Handling Events
    > Let's display an alert popup when the user clicks a specified button:

```js
<button onclick="show()">Click Me</button>
<script>
function show() {
  alert("Hi there")
}
</script>
```

> Event handlers can be assigned to elements.

```js
var x = docuemnt.getElementById("demo");
x.onclick = function () {
  document.body.innerHTML = Date();
};
```

> > You can attach events to almost all HTML elements.

47. Event
    > The onload and onunload events are triggered when the user enters or leaves the page. These can be useful when performing actions after the page is loaded.

```js
<body onload="doSomething()">
```

> Similarly, the window.onload event can be used to run code after the whole page is loaded.

```js
window.onload = function () {
  // some code
};
```

> The onchange event is mostly used on textboxes. The event handler gets called when the text inside the textbox changes and focus is lost from the element.

```js
<input type="text" id ="name" onchange="change()">
<script>
function change() {
  var x = document.getElementById("name");
  x.value = x.value.toUpperCase();
}
</script>
```

> > It's important to understand events, because they are an essential part of dynamic web pages.

48. Event Listener
    > The addEventListener() method attaches an event handler to an element without overwriting existing event handlers. You can add many event handlers to one element. You can also add many event handlers of the same type to one element, i.e., two "click" events.

```js
element.addEventListener(event, function, useCapture);
```

> The first parameter is the event's type (like "click" or "mousedown"). The second parameter is the function we want to call when the event occurs. The third parameter is a Boolean value specifying whether to use event bubbling or event capturing. This parameter is optional, and will be described in the next lesson.

> > Note that you don't use the "on" prefix for this event; use "click" instead of "onclick".

```js
element.addEventListener("click", myFunction);
element.addEventListener("mouseover", myFunction);

function myFunction() {
  alert("Hellow World!");
}
```

> This adds two event listeners to the element. We can remove on of the listeners:

```js
element.removeEventListener("mouseover", myFunction);
```

> Let's create an event handler that removes itself after being executed:

```js
<button id="demo">Start</button>

<script>
var btn = document.getElementById("demo");
btn.addEventListener("click", myFunction);

function myFunction() {
  alert(Math.random());
  btn.removeEventListener("click", myFunction)
}
</script>
```

> After clicking the button, an alert with a random number displays and the event listener is removed.

> > Internet Explorer version 8 and lower do not support the addEventListener() and removeEventListener() methods. However, you can use the document.attachEvent() method to attach event handlers in Internet Explorer.

49. Event Propagation
    > There are two ways of event propagation in the HTML DOM: bubbling and capturing. Event propagation allows for the definition of the element order when an even occurs. If you have p tag element inside a div tag element, and the user clicks on the p tag element, which element's "click" event should be handled first?

> In bubbling, the innermost element;s event is handled first and then the outer element;s event is handled. The p tag element;s click event is handled first, followed by the div tag element's click event.

> In capturing, the outermost element's event is handled first and then the inner. The div tag element;s click event is handeld first, followed by the p tag element;s click event.

> > Capturing goes down the DOM. Bubbling goes up the DOM

50. Capturing vs Bubbling
    > The addEventListener() method allows you to specify the propagation type with the "useCapture" parameter.

```js
addEventListener(event, function, useCapture)
```

> The default value is false, which means the bubbling propagation is used; when the value is set to true, the event uses the capturing propagation.

```js
// Capturing propagation
elem1.addEventListener("click", myFunction, true);

// Bubbling propagation
elem2.addEventListener("click", myFunction, false);
```

> > This is particularly useful when you have the same event handled for multiple elements in the DOM hierarchy.

51. Image Slider
    > Now we can create a sample image slider project. the images will be changed using "Next" and "Prev" buttons. Now, let's create our HTML, which includes an image and the two navigation buttons:

```js
<div>
  <button> Prev </button>
  <img
    id="slider"
    src="http://www.example.com/uploads/slider/1.jpg"
    width="200px"
    height="100px"
  />
  <button> Next </button>
</div>
```

> Next, let's defined our sample images in an array:

```js
var images = [
  "http://www.example.com/uplaeds/slider/1.jpg"
  "http://www.example.com/uplaeds/slider/2.jpg"
  "http://www.example.com/uplaeds/slider/3.jpg"
]
```

> > We are going to use three sample images that we have uploadsed to our server. You can use any number of images.
