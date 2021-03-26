# Custom Functions 

Welcome to the eighth lesson! In this lesson, you learn how to write your own functions. Functions are blocks of code that perform one or more tasks. They're critical for adding functionality to your webpages. You will study the syntax of how to write a function and learn how functions work. Then, you will see several examples of how you can use functions to enhance your projects.

The purpose of showing you examples of how you can use functions is because many different types of situations require you to use a function, and not in all situations are you going to use functions in the same way. For instance, you can use a function to perform a task and `return` a value. Or, instead of returning a value, you may want the function to manipulate the DOM, update a database, or perform some other tasks without returning a value. 

Plus, while practicing writing functions, you can weave together what you learned in previous chapters. For instance, you can write functions containing conditional statements, operators, and expressions. In addition, in your functions, you can get elements by the `id`, tag type, and `class` and do other DOM manipulations. 

At the end of this lesson, you see a live coding example. The live coding session reinforces what you learn in the lesson. This lesson also helps prepare you for making your personal portfolio site. The code from this session is included in this repository. You can use it however you like, but as with any code you get from someone else, make sure you understand it well enough to explain it to someone before putting it in your own projects.  

In this lesson, you learn:  

- Hour 1: [How to Write a Function](#how-to-write-a-function)     
- Hour 2: [Examples of Functions](#examples-of-functions)   
- Hour 3: [Live Coding](#live-coding)   

The topics below outline what you learn in the live session. After the live session, you can use this material as a resource for guided self-learning. This document will serve you as a roadmap for gaining repetition with the material that you learned during the live session.   

## [How to Write a Function](#how-to-write-a-function)       

- Two keys concepts for understanding functions:  
  -- You have to define your function  
  -- Once defined, you have to invoke the function for the code in the definition to actually run      
  
### Function Definitions  

- You have to define a function before you can use it  
- Function definitions are blocks of code that contain instructions for what the function does when you invoke it; note that the function definition code isn't run unless and until you invoke it (invoking a function is also known as calling a function)    
  -- Examples of tasks a function can do are perform math and return a number, manipulate the DOM, communicate with other applications like browsers, servers and databases, and so much more   
- You can define functions in the global scope, inside other functional blocks of code, and inside objects; where you define your function impacts which other blocks of code in which you can invoke that function   
  -- Once you define a function, you can invoke (or call) it multiple times  
- The modern syntax for writing functions is the [arrow syntax](https://www.w3schools.com/js/js_arrow_function.asp)  
- You should know about the [older syntax](https://www.w3schools.com/js/js_function_definition.asp) too because you will see it online; although you will see it online, practice using the arrow syntax in your code (except inside of the global scope or inside objects), as its the more modern approach; this [StackOverflow post has some tips](https://stackoverflow.com/a/23045200) on when to use which type of syntax and why   
- The differences between arrow syntax and older syntax are more than just the syntax; they have slightly different behavior, which mostly deals with scope and is beyond what you learn in this lesson  
- A function defined inside an object is called a method  
- Regardless of which syntax you use or where your function is defined, you can 
  1. Save a function as a named variable, 
  2. Define parameters (like inputs) required by the function in order to invoke it,  
  3. Give the function an explicit `return` statement; 
- Each of these are optional and can be used alone or in combination with one another  
- You can read about saving a function as a named variable here in this section and can read about parameters and the `return` statement in the sub section below this one  
- Function definitions that are not saved as a named variable are known as anonymous functions    
- You should get in the habit of saving your function definitions as named variables because this makes your functions re-usable throughout your code  
- Here is an example of an arrow function named `greetUser` saved to variable that console logs a welcome message with a `username`:  
  ```javascript
  const greetUser = (username) => {
    console.log("Welcome to ITC, " + username);
    }
  ```
- In the example, the `username` is a parameter required by the function definition    
- Your function definitions are not required to include parameters; however, if you do include one or more parameters, they go inside the parenthesis in the function definition    
- By including parameters in your function definition, that means you need to give those parameters values when you invoke the function  
- You can [give parameters default values](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Default_parameters) in your function definition or you can pass arguments into the function when you invoke it (or both, in which case your argument trumps the default value)  
- Here is an example definition with a default value for the `username` parameter:  
  ```javascript
  const greetUser = (username="Jack") => {
    console.log("Welcome to ITC, " + username);
    }
   ```
### Invoking a Function    
 - Invoking a function causes the code inside the function definition to run   
 - To invoke a function, you use the name of the function followed by `()`, and you put inside the `()` arguments for any of the parameters required by the function definition   
  -- For instance, `greetUser("Jill")`  
  -- The value "Jill" is an argument for the `username` parameter   
  -- If the function doesn't require any arguments, for instance, because no parameters exist in the definition or the definition has parameters with default values that you want to use, then you call the function using empty parenthesis (e.g., `greetUser()`). 
 - The difference between an argument and parameter is that a **parameter** appears in the **function definition** and is like a property of the function (typically because the function requires that parameter to have a value for the function to work properly) and an **argument** is a **value** that you pass in for each parameter **when you invoke the function**  
 - If the function definition has a default value for the parameter, calling the function without an argument results in the function using the default value  
 - If a default value exists **and** you pass an argument for the parameter, the argument overrides the default value  
 - When you call a function, by default, [arguments are matched to parameters when read from left to right](https://stackoverflow.com/a/8406177)  
 - Here is one technique some people like: some function definitions have the parameter expect [an object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide) so that you can [pass an object as the argument](https://stackoverflow.com/a/7764557); instead of having to match your arguments to parameters inside the function call, you just pass one object as an argument, and inside the argument object you match the keys and values; this means you do not worry about whether the order of your arguments match the parameters; you just pass in the function one object as the argument, and that object has all the values your function needs     
 - Switching the discussion from function inputs to function outputs . . .  
 - All functions return a value    
 - By default, a function returns the value `undefined`; therefore, if you don't explicitly include a `return` statement or if you `return` nothing, then the function's `return` value is `undefined`  
 - You can override that default value by explicitly returning a value, like so:  
  
  ```javascript
  const greetUser = (username) => {
    const message = "Welcome to ITC, " + username
    return message
    }
  ```
 - A `return` statement makes the `return` value available outside the scope of the function definition  
 - Oftentimes when you return a value, you **will** want to save that value to a variable to capture that value for later use  
 - To capture the `return` value when you invoke a function, set the function call equal to a variable  
 - For instance, you can do this: `const userGreeting = greetUser("Jill")`  
  -- Here, `userGreeteing` is equal to the function call (`greetUser("Jill")`), and the function call is equal to the value "Welcome to ITC, Jill" because that is the value the function returns (i.e., the value that the function makes available when it's done running the code in the function definition)    
 - Naming is important! Use good naming so that your code **tells a story to your reader** and therefore makes your code easier to understand;  
  -- For instance, notice the function returns a greeting message to a user; a message is a noun, so you should name the message using a descriptive noun, like `userGreeting`   
  -- For another example, the function definition performs an action, which is to greet the user; so the function definition should have a descriptive verb as the name, like `greetUser`  
 - A `return` statement ends that block of code, which means that the browser does not read any code appearing inside of the function definition but after a `return` statement    
  
 ### This is just the tip of the iceberg for function  
 
 - You can do very powerful things with a basic understanding of functions  
 - Once you feel comfortable with the basics, continue to explore what else you can do with functions  

## [Examples of Functions](#examples-of-functions)    

 - You should be able to explain the parts of the following functions and how they work:  
 
### Basic arrow function definitions 
 ```javascript
const sendMessage = () => {
  const message = "Hello World";
  console.log(message);
  return message;
}

const helloMessage = sendMessage()
```

```javascript
const sendMessageToUser = (username) => {
  const message = "Hello, " + username;
  console.log(message);
  return message;
}

const helloUserMessage = sendMessageToUser("Jack")
```
### Basic function definition using old syntax   

```javascript
 const sendMessage = function() {
  const message = "Hello World";
  console.log(message);
  return message;
}

const helloMessage = sendMessage("Jack")
```

### Using operators in functions  

```javascript
const calculateSquare = (number) => {
  return number * number;
}

const numberSquared = calculateSquare(9)
```

```javascript
const raiseToThePowerOf = (number, power) => {
  return number ** power;
}

const exponentialResult = raiseToThePowerOf(3, 10)
```

```javascript
const updateLoaderStatus = (isLoading) => {
  loader = document.getElementById("loader");
  
  if (isLoading === true) {
      loader.classList.add("show-loader")
      loader.classList.remove("hide-loader")
  } else {
      loader.classList.remove("show-loader")
      loader.classList.add("hide-loader")
  }
}


updateLoaderStatus(true)
```

### Using conditional statements in functions    

```javascript
const determineOddOrEven = (number) => {
  if (number % 2 == 0) {
    return true
  } else {
    return false
  }
}

const isOdd = determineOddOrEven(9)
const isEven = determineOddOrEven(10)
```

```javascript
const raiseToThePowerOf = (number, power) => {
  return number ** power;
}

const exponentialResult = raiseToThePowerOf(3, 10)
```

### Performing multiple tasks using ES6 Built-in functions

Reverse a string using ES6 (see [this article](https://www.freecodecamp.org/news/how-to-reverse-a-string-in-javascript-in-3-different-ways-75e4763c68cb/) for more information)  

```javascript
const reverseString = (str) => {
    // Step 1. Use the split() method to return a new array
    const splitString = str.split(""); // var splitString = "hello".split("");
    // ["h", "e", "l", "l", "o"]
 
    // Step 2. Use the reverse() method to reverse the new created array
    const reverseArray = splitString.reverse(); // var reverseArray = ["h", "e", "l", "l", "o"].reverse();
    // ["o", "l", "l", "e", "h"]
 
    // Step 3. Use the join() method to join all elements of the array into a string
    const joinArray = reverseArray.join(""); // var joinArray = ["o", "l", "l", "e", "h"].join("");
    // "olleh"
    
    //Step 4. Return the reversed string
    return joinArray; // "olleh"
}
 
reverseString("hello");
```

### Manipulating the DOM  

Check out this [MDN Example](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals#else_if); here is the code from that example, but click on the link to see it in action    

```html
<label for="weather">Select the weather type today: </label>
<select id="weather">
  <option value="">--Make a choice--</option>
  <option value="sunny">Sunny</option>
  <option value="rainy">Rainy</option>
  <option value="snowing">Snowing</option>
  <option value="overcast">Overcast</option>
</select>

<p></p>
```

```javascript
const select = document.querySelector('select');
const para = document.querySelector('p');

select.addEventListener('change', setWeather);

const setWeather = () => {
  const choice = select.value;

  if (choice === 'sunny') {
    para.textContent = 'It is nice and sunny outside today. Wear shorts! Go to the beach, or the park, and get an ice cream.';
  } else if (choice === 'rainy') {
    para.textContent = 'Rain is falling outside; take a rain coat and an umbrella, and don\'t stay out for too long.';
  } else if (choice === 'snowing') {
    para.textContent = 'The snow is coming down — it is freezing! Best to stay in with a cup of hot chocolate, or go build a snowman.';
  } else if (choice === 'overcast') {
    para.textContent = 'It isn\'t raining, but the sky is grey and gloomy; it could turn any minute, so take a rain coat just in case.';
  } else {
    para.textContent = '';
  }
}
```

## [Live Coding](#live-coding)   

The live coding session continues working on the live code from the previous lessons. Here are the tasks:  

1. Write a function that gets the title from your webpage and counts the number of vowels and the number of consonants in your title; use a regular `for` loop, not a built-in JavaScript loop; show the numbers for vowels and consonants on the webpage  

2. Write a function that takes in an array containing at least three strings, one of which is not the word "or", and uses the strings in the array to build a sentence that starts with "When I'm really hungry, I like to eat " and is followed by the items in your array where the second-to-last and last item in the sentence are separated by the word "or"; the function should return the sentence (e.g., "When I'm really hungry, I like to eat pasta, pizza, or chocolate ice cream."  
