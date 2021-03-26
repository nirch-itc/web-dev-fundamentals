# Working With The DOM

Welcome to the sixth lesson! In this lesson, you learn about the Document Object Model, commonly known as **The DOM**. Using the DOM, you can interact with your HTML document using JavaScript. With JavaScript, you can access, modify, and otherwise interact with your HTML document and the elements inside it.

In this lesson, first you learn about what the DOM is. Next, you will look under the hood to learn about the properties and methods available for the HTML document itself and for the elements within it. Using these methods and properties, you can add functionality to your web pages. For instance, you can change the text, add and remove styles, capture user input, and so much more.  

At the end of this lesson, you see a live coding example. The live coding session reinforces what you learn in the lesson. This lesson also helps prepare you for making your personal portfolio site. The code from the session is included in this repository. You can use it however you like, but as with any code you get from someone else, make sure you understand it well enough to explain it to someone before putting it in your own projects.  

In this lesson, you learn:  

- Hour 1: [What is the DOM](#what-is-the-dom)     
- Hour 2: [JavaScript Builtin Functions](#javascript-builtin-functions)   
- Hour 3: [Live Coding](#live-coding)  

The topics below outline what you learn in the live session. After the live session, you can use this material as a resource for guided self-learning. This document will serve you as a roadmap for gaining repetition with the material that you learned during the live session.   

## [What is the DOM](#what-is-the-dom)    

- The [DOM](https://www.w3schools.com/js/js_htmldom.asp) is an object-oriented representation of an HTML document 
- When a webpage loads, the browser converts the HTML into a DOM  
- Every element in an HTML document is part of the document object model for that document. For instance:  
    -- The `document` itself  
    -- The `head`  
    -- The `body`  
    -- The elements inside the body, like `div`, `h1`, `p`  
- You saw a [visual representation of the DOM](https://css-tricks.com/dom/) when you looked at the Elements tab in the inspector  
- You can modify the DOM [using a scripting language such as JavaScript](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction#dom_and_javascript)  
- You can access the DOM in your JavaScript code by creating a `script` inside your HTML document    
  -- It can be a `script` that links to an external JavaScript file or any other type of `script`   
  -- You can immediately begin accessing the DOM and modifying HTML elements  
  -- As you learned in the variables lesson, once you access an HTML element, you can **save it as a variable** and **access its attributes**    
- The DOM has various [built-in data types](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction#important_data_types)    
  -- Pay special attention to the built-in [data type named `document`](https://developer.mozilla.org/en-US/docs/Web/API/Document)  
  -- The `document` is an object that represents the HTML document as loaded in the browser  
  -- It serves as an entry point for JavaScript into the web page's content    
  -- It provides [global functionality](https://developer.mozilla.org/en-US/docs/Web/API/Document#properties), like accessing the page's URL or adding new elements, through its built-in methods     
- Modifying the DOM is modifying the HTML document  
- The DOM organizes into objects the properties, methods, and events available for modifying and creating HTML elements       
- By defining the HTML elements as objects, JavaScript can do things like:  
  -- Get an existing HTML element and read its attributes  
  -- Change an existing HTML element's attributes    
  -- Add a new HTML element and set its attributes   
  -- Remove an existing HTML element or any of its attributes    
  -- Create and execute new HTML events    
  -- An example using document's built-in method for getting an HTML element by its `id` attribute: `const submitButton = document.getElementById("submitButton")`  
## [JavaScript Builtin Functions](#javascript-builtin-functions)    

### DOM Methods    

- A document object has many [properties and methods](https://www.w3schools.com/jsref/dom_obj_document.asp)  
- Commonly used **methods** for the **document** include:    
  -- [`getElementById`](https://www.w3schools.com/jsref/met_document_getelementbyid.asp)    
  -- [`createElement`](https://www.w3schools.com/jsref/met_document_createelement.asp)    
  -- [`getElementsByClassName`](https://www.w3schools.com/jsref/met_document_getelementsbyclassname.asp)    
  -- [`addEventListener`](https://www.w3schools.com/jsref/met_document_addeventlistener.asp)    
- Element objects also have [properties and methods](https://www.w3schools.com/jsref/dom_obj_all.asp)     
- Commonly used **methods** for **elements** include:    
  -- [`appendChild`](https://www.w3schools.com/jsref/met_node_appendchild.asp)    
  -- [`removeChild`](w3schools.com/jsref/met_node_removechild.asp)    
  -- [`addEventListener`](https://www.w3schools.com/jsref/met_element_addeventlistener.asp)    
  -- [`getElementsByTagName`](https://www.w3schools.com/jsref/met_element_getelementsbytagname.asp)    
- Commonly used **properties** for **elements** include:    
 -- [`id`](https://www.w3schools.com/jsref/prop_html_id.asp)    
 -- [`classList`](https://www.w3schools.com/jsref/prop_element_classlist.asp)    
 -- [`textContent`](https://www.w3schools.com/jsref/prop_node_textcontent.asp)    
 -- You will see online the use of `innerText` and `innerHTML` instead of `textContent` and you should know [the differences](https://developer.mozilla.org/en-US/docs/Web/API/Node/textContent)    

### DOM Events    

- The [`addEventListener` method](https://www.w3schools.com/js/js_htmldom_eventlistener.asp) lets you turn a DOM element into an element that listens for an event to happen    
- An event can be when a user clicks, types into an input, moves their mouse over an element, and much more    
- To turn a DOM object into a listener, access it `getElementById` or create it using `createElement` and then call the `addEventListener` method; [don't use HTML attributes to listen for events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events#what_mechanism_should_i_use)     
- When calling the `addEventListener` method, you need to pass to it two arguments:  
    -- The [name of the type of event](https://www.w3schools.com/jsref/dom_obj_event.asp) to listen for    
    -- A function that will be triggered when the event happens    
- When passing the function in as an argument, it's good practice to pass in the name of the function instead of the entire function definition    
  -- Example: `submitButton.addEventListener('click', sendFormInfo)`   
  -- Assume that `sendFormInfo` is the name of a function   
  -- Notice that you don't include `()` on the end of `sendFormInfo` because you don't want to call the function now; only pass a reference to it    
  -- This makes your code more reusable and easier to read and maintain than defining the function inside the `addEventListener` method    
- Inside the listener's function, you can access the [event object](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events#event_objects)     
- The event object makes available to you the details of the event, such as the type of event, the HTML element it happened on, all the attributes of that HTML elements, and more    
- You will commonly use the event object to get and modify the attributes of an HTML element, like its text content, styles, and more    
- The event object is automatically passed to event handlers and is the first argument in your function definition    
- In examples online, you will see the event object represented in code usually as `event`, `e`, or `evt`  
- For instance:    

```javascript
const getClickEvent = (e) => {
  console.log(e.target.value);
  console.log(e.target.classList);
}

submitButton.addEventListener('click', getClickEvent);
```

## [Live Coding](#live-coding)   

The live coding session continues working on the live code from the previous lessons. Here are the tasks:  

1.  You should already have four inputs in your form; add an event listener to each input in form; the listeners should listen for a change in value; when a change in value occurs, console log the value  
2. Console log the id attribute when a change in value occurs to that input in your form       
3. Add a click event listener to your submit button; when a user clicks the button, console log the text content and class list for the button    
4. You should have two images on your home page, a big one and a small one; for the big one:    
    a. Add two buttons below it called previous and next; review [this link](https://frontendmasters.github.io/bootcamp/interactive) for inspiration  
    b. Use an array to store the photo names and the index position of the photo to set the src attribute of the img tag    
    c. You must have a minimum of three photos     
    d. When a user is on the first photo in the array, the previous button should be hidden and disabled    
    e. When a user is on the last photo in the array, the next button should be hidden and disabled    
5. For the small button, make it so that the small image changes the photo that it displays when a user clicks it; similar concept as the previous task, but this time without buttons      
    a. Use the same array as above    
    b. When a user clicks on the photo, it should display the next photo in the array    
    c. When a user clicks on the last photo, it should display the first photo     
