# JavaScript Logic  

Welcome to the seventh lesson! In this lesson, you learn about JavaScript logic. Adding logic to your JavaScript code will give your webpage functionality. You can add logic to your code using loops, conditionals, operators, and expressions. 

First, you will learn about loops. You use loops to run the same block of code multiple times but on a different value each time. Typically, you loop through arrays and strings. Next, you will learn about conditionals, operators, and expressions. Conditional statements let you add control to your code by telling it to run certain blocks under certain circumstances. Operators allow you to compare, combine, and otherwise interact with data to modify data or make decisions. Expressions are blocks of code that return a value. For instance, a function always returns a value (by default, it returns `undefined`) and is therefore an expression. 

Using these tools alone and in combination with one another will give your application the ability to make decisions based on circumstances. 

At the end of this lesson, you see a live coding example. The live coding session reinforces what you learn in the lesson. This lesson also helps prepare you for making your personal portfolio site. The code from this session is included in this repository. You can use it however you like, but as with any code you get from someone else, make sure you understand it well enough to explain it to someone before putting it in your own projects.  

In this lesson, you learn:  

- Hour 1: [Loops and Iterable Data Types](#loops-and-iterable-data-types)     
- Hour 2: [Conditionals, Operators, and Expressions](#conditionals-operators-and-expressions)   
- Hour 3: [Live Coding](#live-coding)  

The topics below outline what you learn in the live session. After the live session, you can use this material as a resource for guided self-learning. This document will serve you as a roadmap for gaining repetition with the material that you learned during the live session.   

## [Loops and Iterable Data Types](#loops-and-iterable-data-types)   

- A loop is a block of code that repeats itself  
- Typically has a [counter, condition, and iterator](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code#keep_me_in_the_loop) in addition to whatever code is inside the loop  
- Loops are most useful when you want to run the same block of code on multiple values  
- Loops, therefore, are a great tool to use with [iterable data types](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Iteration_protocols#iterable_examples)  
- The iterable data types you should know of are strings and arrays  
- The types of loops for you to know about are `for` loops, `while` loops, and `for/in` loops    
- A `for` loop repeats a block of code **for** a predefined number of times
- A `while` loop repeats a block of code **while** a condition is true and therefore the number of times it runs is not necessarily pre-defined    
- A `for/in` loop is like a `for` loop but it's for looping through an object of key:value pairs, not for strings and arrays  
- Here is [an example](https://www.w3schools.com/js/js_loop_for.asp) of how a `for` loop can transform your code  
- Walk through a `for` loop step-by-step explaining what happens and how the syntax works   
  -- Focus on using the index position to move through the array  
  -- Having a solid understanding of [index positions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Indexed_collections#referring_to_array_elements) is critical   
  -- ES6 has [built-in methods for looping](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Indexed_collections#array_methods) that you should know  
- Here are [examples](https://www.w3schools.com/js/js_loop_while.asp) of how a `while` loop works with some explanation  
- Walk through a `for` loop step-by-step explaining what happens and how the syntax works  
- Here is [an example and description](https://www.w3schools.com/js/js_loop_forin.asp) of how a `for in` loop works  
- [MDN's in-depth discussion](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration) is a good resource to learn more advanced ways of working with loops, like using `break` and `continue`    

## [Conditionals, Operators, and Expressions](#conditionals-operators-and-expressions)    

- You oftentimes will use conditional statements, operators, and expressions inside loops  
- You oftentimes will use loops inside a conditional statement or in combination with operators and expressions  
- You should have a good understanding of [Booleans](https://www.w3schools.com/js/js_booleans.asp) given that conditionals and operators check whether a certain condition is true or false  

### Conditionals  

- Conditional statements let you control when to perform certain actions  
- In other words, you can check whether a condition exists before running a block of code  
- To write conditional statements, you need to use `if` alone or in combination with `else` and/or `else if`  
- An `if` statement must be written with a condition and block of code following it  
- If the condition is true, then the browser runs the corresponding block of code  
- Here is [an example](https://www.w3schools.com/js/js_if_else.asp) of an `if` statement  
- In combination with `if`, you can use `else` and/or `else if`  by chaining them to `if` or one another  
- `else if` requires a condition like `if` does, but `else` does not require a condition; both require a corresponding block of code  
- Here are [examples](https://www.w3schools.com/js/js_if_else.asp) of `else` and `else if` in conditional statements  

### Operators  

- **Comparison** operators let you compare values to check, for instance, whether they are equal to one another, whether one is greater than or equal to the other, and more  
- Look here for [syntax and examples](https://www.w3schools.com/js/js_comparisons.asp)  
- **Logical** operators let you check whether something **and** something are true, something **or** something is true, or whether something is **not** true  
- Look here for [syntax and examples](https://www.w3schools.com/js/js_comparisons.asp)  
- You also can use **assignment** operators, **arithmetic** operators, and **string** operators to add logic to your code  
- Look here for [syntax and examples](https://www.w3schools.com/js/js_operators.asp)  
- [MDN's in-depth discussion](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators) is a great resource for learning about operators and its [list of operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators) also is good  

### Expressions  

- An expression is [any block of code that results in a value](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#expressions)  
- An expression is different from other statements because not all blocks of code result in a value 
- Instead, some blocks of code perform certain tasks but do not result in returning a value; those are not expressions  
- An `if` block is an example of a statement  
- A function with an explicit `return` statement is an example of an [expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions#returning_a_formatted_number)  
 -- [Important Sidenote](https://stackoverflow.com/a/20915524): functions, by default, return the value `undefined` but you can override that value by explicitly declaring a `return` value; therefore, every function is technically an expression  
- The value that an expression returns depends upon your circumstances  
- Use conditionals and operators in combination with one another and in combination with data types to write blocks of code that return a value  
- You will see more of this when you learn about functions in detail later  
- This StackOverflow post has a good explanation of expressions vs statements](https://stackoverflow.com/questions/46351924/javascript-declarations-vs-expressions-vs-statements)
- Here is a good article [explaining expressions](https://masteringjs.io/tutorials/fundamentals/expressions)  

## [Live Coding](#live-coding)   

The live coding session continues working on the live code from the previous lessons. Here are the tasks:  

1. Find the form on your page and add a button to it  
2. To the button, add a click event listener, and inside the corresponding function, console log the values for your four inputs when the user presses the button  
3. Inside that function, write an `if` statement that checks whether all four inputs have values  
4. If all four inputs have values, console log the phrase "Your form is complete" and also console log the values    
5. Add an `else if` statement that checks whether at least one input has a value  
6. If at least one input (but not all) has a value, console log the phrase "Your form needs more information" and also console log the names of the tags for which you need more information      
7. Add an `else` statement  
8. Console log in the `else` statement the phrase "Your form is empty"    
9. Inside the `if` block, in addition to the console log, add a custom CSS class to the small image on the screen that changes the style of that image when you click the button    
