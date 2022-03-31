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
