# HTML Basics  

Welcome to the second lesson! In this lesson, you continue learning about HTML. You will learn about HTML's *tag syntax* by examining different tag types. By examining tag syntax, you will become familiar with which tags to use in which situation, how to fill tags with content, and how to use the inspector to assist you with writing HTML. You also learn about *HTML attributes*, which are properties of HTML tags that can help you define and control HTML elements. Finally, you can participate in a live coding session in which you will see how to start a project from scratch and add to it several different types of HTML tags.  

The live coding session reinforces what you learn in the lesson and to help prepare you for making your personal portfolio site. You can find the code for the session in this repository. You can use it however you like, but as with any code you get from someone else, make sure you understand it well enough to explain it to someone before putting it in your own projects.  

In this lesson, you learn:  

- Hour 1: [HTML Tag Types](#html-tag-types)    
- Hour 2: [HTML Attributes](#html-attributes)   
- Hour 3: [HTML Live Coding](#html-live-coding)  

The topics below outline what you learn in the live session. After the live session, you can use this material as a resource for guided self-learning. This document will serve you as a roadmap for gaining repetition with the material that you learned during the live session.   

Also included in this material is the code from the live coding session.  

## [HTML Tag Types](#html-tag-types)  
 - [Tag syntax](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)  
 - [Tag types](https://www.w3schools.com/tags/)  
 - Some HTML tags have specific use situations and the content-holding tags come with built-in styles; learn about them to know when to use which tag   
    -- [metadata](https://html.com/document/metadata/) don't appear on the screen but hold important information for your page   
    -- [`body` tags](https://www.w3schools.com/tags/tag_body.asp) hold all the page content and wraps the content-holding tags  
    -- [`div` tags](https://www.w3schools.com/tags/tag_div.asp) are very commonly used, hold text and other HTML elements, and have a built-in `display: block` style property  
    -- [`span` tags](https://www.w3schools.com/tags/tag_span.asp) are like `div` tags because the hold text and other HTML elements, but they have a built-in `display: inline` style property      
    -- [`h1` - `h6` tags](https://www.w3schools.com/tags/tag_hn.asp) hold text and other HTML elements and have built-in `font-size`    
    -- [`p` tags](https://www.w3schools.com/tags/tag_p.asp) hold text and appear as a paragraph       
    -- [`a` tags](https://www.w3schools.com/tags/tag_a.asp) create links to other webpages     
    -- [`img` tags](https://www.w3schools.com/tags/tag_img.asp) display an image on the page  
  - HTML5 may help  
    -- Modernized HTML tags designed for specific use cases  
    -- You may see [HTML5 tags](https://html.com/document/) online or in other people's code  
    -- It's okay to use HTML5 tags or not to use them; regardless, try to be consistent and predictable with your code  
    -- Among many benefits, HTML5 may make your code [easier for you and other developers to read and maintain](https://html.com/html5/)  
  - How to fill tags with content  
    -- An element with opening and closing tags holds content between those tags   
    -- Self-closing tags hold content in an attribute  
    -- Nesting elements inside other elements is a very common thing to do for purposes of layout and style  
  - Tips on working with images  
    -- [Web Images: Practical Tips Plus Code To Put Them To Best Use](https://html.com/images/)  
    -- [Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)    
  - How to use the inspector to assist you with writing HTML  
    -- Can you move the inspector to the right side of your browser?  
    -- Can you move the inspector to the bottom of your browser?  
    -- Look at the Elements tab and find the HTML elements  
    -- Where in the Elements tab do you see HTML content?  
    -- In the Elements tab, can you change the name of a tag?  
    -- Do you see any built-in styles for each HTML element?  
    -- How do you open HTML tags in the Elements tab so that you can see what's nested inside?  
    -- Find an img tag - do you see its source?   
    -- Copy and paste the source into a browser's url  
    -- Do you see any HTML5 tags on any websites?  

## [HTML Attributes](#html-attributes)   

  - You can use HTML attributes to define and control HTML elements  
  - An attribute is a property of an HTML element, and certain types of tags have certain kinds of attributes  
  - Many [HTML attributes](https://www.w3schools.com/tags/ref_attributes.asp) exist, and here are some you will use frequently:  
    -- `class` for applying one or more CSS classes to an element (tags: any)  
    -- `href` for setting a link's destination (tags: `a`, `area`, `base`, `link`)  
    -- `id` for giving an HTML element a unique identifier (tags: any)    
    -- `rel` for linking the current document to another document (tags: `a`, `area`, `form`, `link`)    
    -- `src` for setting the url of a media file (tags: `audio`, `embed`, `iframe`, `img`, `input`, `script`, `source`, `track`, `video`)    
    -- `type` for defining the type of element (tags: `a`, `button`, `embed`, `input`, `link`, `menu`, `object`, `script`, `source`, `style`)  
    -- `value` for setting an element's value (tags: `button`, `input`, `li`, `option`, `meter`, `progress`, `param`)    
  - Frequently, you write tags without explicitly declaring any attributes (e.g., `<div>Welcome to ITC!</div>`)  
  - When you do declare attributes, write them in:   
    -- The opening tag   
    -- [Key:value pairs where the value is a string](https://www.tutorialrepublic.com/html-tutorial/html-attributes.php) (text wrapped in quotes)    
    -- Example: `<a href="www.itc.tech">Enroll</a>`  
  - The `href` and `src` attributes    
    -- Can use absolute or relative path    
    -- Absolute path links to an external source    
    -- Relative path links to internal source    
    -- Use the `<a>` tag to [link to other HTML pages in your project](https://www.w3schools.com/html/html_links.asp) by setting the `src` attribute equal to the relative path  
  - You will see in code examples online use of the `style` attribute    
    -- The `style` attribute allows for setting an HTML element's style (called inline styling)    
    -- Do not use this as your primary way of styling your web applications because it can be difficult to maintain    
    -- It is okay to not even use the `style` property or to use it only in special situations    
    -- Instead of using `style`, use a stylesheet that you write or import from a CSS framework  
  - Some HTML attributes listen for events, and then trigger functionality when that event happens    
    -- Examples: `onchange`, `onclick`, `oncopy`, `ondrag`, `onsubmit`    
    -- When you learn JavaScript, it is better that you not use these    
    -- Instead, use JavaScript code to listen for events instead of an HTML attribute for code that is easier to read and maintain    
  - Examples of attributes use cases to get you thinking:  
    -- [Spell check in forms](https://www.tutorialrepublic.com/faq/how-to-disable-spell-checking-in-html-forms.php)  
    -- [How to make a `div` editable](https://www.tutorialrepublic.com/faq/how-to-make-a-div-element-editable-in-html.php)  
    -- [How to remove bullets from list](https://www.tutorialrepublic.com/faq/how-to-create-an-unordered-list-without-any-bullets-in-html.php)  
    -- [Placeholder in select dropdown](https://www.tutorialrepublic.com/faq/how-to-make-a-placeholder-for-a-select-box-in-html.php)  
    -- [How to disable a button](https://www.w3schools.com/tags/att_button_disabled.asp)  
  - You will use JavaScript to change attributes dynamically  
    
## [HTML Live Coding](#html-live-coding)  
 
With some knowledge and resources in hand, now you are ready for live coding. In the live coding session, apply what you learned above. As an extra challenge, the last task asks you to do something you haven't yet learned. The tasks are:  
 
 1. Create a project folder with an index.html skeleton file, a CSS subfolder, and a blank styles.css file  
 2. Add metadata elements to the head for title, description, [icon](https://stackoverflow.com/questions/4888377/how-to-add-a-browser-tab-icon-favicon-for-a-website), and stylesheet  
 3. Add elements for a title and subtitle such that the title has a larger font size than the subtitle  
 4. Below the subtitle, add three links; the links should be stacked vertically, not horizontally; each link should take the user to one of your favorite websites  
 5. Above the title, add two images side-by-side; one image should display content from an absolute path and the other a relative path  
 6. Add three elements that take in an input; one must be text and the other two some other input type but not the same as the others   
 7. Add two buttons below the input, one disabled and the other enabled   
 8. Add a map that displays your hometown 
 9. Add an element that wraps two other elements, and inside of each of those two elements are three elements (9 elements total)  
 10. Add a `div` element on the left side of your page that takes 100% of the page width and that is editable
 11. Add an [HTML comment](https://www.tutorialrepublic.com/faq/how-to-write-comments-in-html.php) that apologizes for the poor styling  
 12. Write two CSS classes, one for each button; when you apply them to the HTML buttons, one class should make the disable button look disabled and the other class make the enabled button look enabled  

