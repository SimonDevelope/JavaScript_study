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
