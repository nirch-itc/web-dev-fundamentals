# Getting Started  

Welcome to the first lesson! In this first lesson, you focus on getting started as a developer. Being a developer requires more than just writing code. You need to learn how the web works, where to write your code, how to organize your files, where to find answers, and so much more.

In this lesson, you learn:

- Hour 1: [Course Intro and How the Web Works](#course-intro-and-how-the-web-works)    
- Hour 2: [Code Editors and Project Folder Structure ](#code-editors-and-project-folder-structure)   
- Hour 3: [Intro to HTML](#intro-to-html)  

The topics below outline what you learn in the live session. After the live session, you can use this material as a resource for guided self-learning. This document will serve you as a roadmap for gaining repetition with the material that you learn during the live session. 

## [Course Intro and How the Web Works](#course-intro-and-how-the-web-works)  
  
### Course Intro (see course info repo)

In the Google Classroom, find the post containing the link to the course information. Please review the course information. It outlines the syllabus, and other necessary information.  
  
### How the Web Works

The following outline contains basic information and links about how the web works. Please do not feel any pressure to understand all the information in this section. It's a lot of information! The purpose isn't to overwhelm you. Instead, it's to expose you to the topics on how the web works. 

As the program progresses, you will focus on specific parts of these topics and gain repetition with them.  
  
  - Browser  
    -- Based on a domain name, displays information on a screen for easy viewing  
    -- Chrome, Firefox, and Safari are examples of browsers  
    -- [Domain name](https://en.wikipedia.org/wiki/Domain_name) is alphanumeric and goes in browser's URL  
    -- [IP Address](https://en.wikipedia.org/wiki/IP_address) corresponding to domain name is retrieved by browser from DNS Server   
    -- [DNS Server](https://en.wikipedia.org/wiki/Domain_Name_System) links domain name to IP Address from browser  
    -- Browser uses IP Address for domain to request files from hosting provider  
    -- [Hosting provider server](https://en.wikipedia.org/wiki/Web_hosting_service) provides browser with source code for IP Address  
    -- Source code instructs the browser on how to display the information     
    -- Source code for browsers is typically HTML, CSS, JavaScript  
    -- Look at the inspector in your browser to explore behind the scenes  
    -- In the ITC Fullstack bootcamp and also the Frontend Course, you learn advanced HTML, CSS, and JavaScript   
    -- In this program, you learn the basics of HTML, CSS, and JavaScript   
  - Server  
    -- Software that runs on a [machine](https://media.geeksforgeeks.org/wp-content/uploads/20200429161002/server-image-1.png) and listens for incoming requests   
    -- [Express.js](https://expressjs.com/en/starter/hello-world.html) is an example of a JavaScript-based server framework  
    -- A server communicates with browsers, other servers, and databases  
    -- Has [routes that receive requests and send responses](https://expressjs.com/en/starter/basic-routing.html)  
    -- A route is like a server address (is not the same as a domain name or url)  
    -- Browser [sends request](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) to server route (or one server sends request to another server)  
    -- Server route responds with a response  
    -- A route usually has some functionality associated with it in addition to sending a response, like calling a database and processing data  
    -- Browser [receives response](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch#checking_that_the_fetch_was_successful) and displays it to the user  
    -- In addition to communicating with browsers, server can also create, update, read, and delete data from databases  
    -- Servers are written in many languages (two common ones are Node.js and Python)  
    -- In the ITC Fullstack bootcamp, you build your own servers and communicate with third-party servers  
    -- In this program, you will interact with third-party servers when learning about asynchronous code  
  - Database  
    -- A database stores electronic information  
    -- Databases live on a machine  
    -- Many [types of databases](https://www.guru99.com/introduction-to-database-sql.html) exist  
    -- Databases communicate with servers  
    -- Then servers send the data to browsers or servers  
    -- A common sequence: Browser sends a request to the server, which triggers the server to request data from the database; upon receiving the data from the database, the server responds to the browser's request with the data   
    -- In the ITC Fullstack bootcamp, you work with relational databases (SQL) and NoSQL (MongoDB)  
    -- In this program, you will not work with databases directly  
  - HTTP  
    -- A protocol for sending and receiving messages over the web  
    -- [Request methods](https://www.w3schools.com/tags/ref_httpmethods.asp) distinguish between the type of request you are sending  
    -- [Response status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status) help you know the status of a response  
    -- [JSON](https://www.w3schools.com/whatis/whatis_json.asp) is the data format you use to send and receive data via HTTP  
    -- You will work with requests, responses, and JSON in this course and the ITC Fullstack Program and Frontend Course    
  
## [Code Editors and Project Folder Structure](#code-editors-and-project-folder-structure)  
  - Visual Studio Code (VS Code)  
    -- [Download it](https://code.visualstudio.com/)   
    -- [Practice using it](https://code.visualstudio.com/docs/introvideos/basics)  
    -- Open a project folder in VS Code  
    -- Create a new file in your root folder, subfolder in your root folder, and file in your subfolder  
    -- Practice renaming files and dragging from folder to folder  
    -- Explore the split screen, terminal, and settings  
    -- Search for files  
    -- Open HTML file in browser  
  - VS Code Extensions  
    -- You can install extensions to enhance your coding experience  
    -- One example: Prettier Code Formatter auto formats your code so that it's organized and easy to read   
    -- Install it  
    -- In VS Code settings, search for "format" and choose "format on save"  
  - Folder Structures and File Paths  
    -- Example of HTML, CSS, JS [folder structure](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/Dealing_with_files)  
    -- [File paths](https://www.w3schools.com/html/html_filepaths.asp)   

## [Intro to HTML](#intro-to-html)   
  - HTML is a document  
    -- Look at the [inspector](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools) in your web browser   
    -- What do you see in the elements tab?  
    -- Do you see HTML?  
    -- What happens if you change the text inside an HTML tag?  
    -- Can you find another tab in the inspector where the source code files are accessible?  
    -- Explore what else you see in the inspector  
  - HTML Tags Examples  
    -- Look at [W3 Schools HTML Introduction](https://www.w3schools.com/html/html_intro.asp) for an example of how an HTML page is organized  
    -- Learn about [HTML elements generally](https://www.w3schools.com/html/html_elements.asp)  
    -- Explore [basic element types](https://www.w3schools.com/html/html_basic.asp)  
    -- Here is a list of [HTML tags](https://www.w3schools.com/tags/default.asp)  
  - HTML is used in combination with CSS for style  
    -- Import stylesheets for CSS in the [HTML head tag](https://www.w3schools.com/html/html_head.asp)  
  - HTML is used in combination with JavaScript for functionality  
    -- Import scripts into your HTML using the [script tag](https://www.w3schools.com/html/html_scripts.asp) inside the HTML body at the bottom   

