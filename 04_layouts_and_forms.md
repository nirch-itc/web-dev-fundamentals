# HTML and CSS: Layouts and Forms  

Welcome to the fourth lesson! In this lesson, you learn the basics of **layouts and forms**. A webpage's layout is how you organize the HTML elements on the screen. Based on which HTML tag types you write in your code and the order of them, your page will have a default layout. In other words, when you load the page in the browser, the HTML elements will organize themselves based on the tag type and order written in your file.

Using various collections of CSS style properties, you can override the default layout. In this lesson, you learn about **three different collections of style properties** that help you customize your page layout. Specifically, you learn how to position a single HTML element, align multiple HTML elements in a row **or** column, and align multiple HTML elements in rows **and** columns.  

After learning about layouts, you will learn about **HTML forms**. A form is a collection of HTML elements that allow a user to input and submit information. A form has one or more inputs and can also have one or more buttons. A form usually submits the information to a server. In this lesson, you learn about the different parts of HTML forms and how to customize them for your needs. If you enroll in [ITC's fullstack program](htps://www.itc.tech), you can learn how to send the information from a form to a server.

At the end of this lesson, you see a live coding example for creating a page layout and adding a form to your page. The live coding session reinforces what you learn in the lesson. This lesson also helps prepare you for making your personal portfolio site. The code from the session is included in this repository. You can use it however you like, but as with any code you get from someone else, make sure you understand it well enough to explain it to someone before putting it in your own projects.  

In this lesson, you learn:  

- Hour 1: [Position and Flexbox](#position-and-flexbox)    
- Hour 2: [Grid and Forms](#grid-and-forms)   
- Hour 3: [HTML and CSS Live Coding](#html-and-css-live-coding)  

The topics below outline what you learn in the live session. After the live session, you can use this material as a resource for guided self-learning. This document will serve you as a roadmap for gaining repetition with the material that you learned during the live session.   

## [Position and Flexbox](#position-and-flexbox)   

### Position  
 
- HTML elements, by default, have a collection of positioning properties  
- The positioning properties are `position`, `top`, `right`, `bottom`, `left`, `clip`, and `z-index`  
- Read about them at the bottom of the page about [positioning properties](https://www.w3schools.com/css/css_positioning.asp)  
- An HTML element's default value for `position` is `static`  
- `static` results in an HTML element rending on the screen in the order written in your document  
- By setting the `position` value to something other than `static`, you can change the type of positioning method for that element  
- The `position` values available are `static`, `relative`, `absolute`, `fixed`, `sticky`  
- Each [positioning method has its own behavior](https://www.w3schools.com/cssref/pr_class_position.asp)  
- Understand [how the positioning methods differ](https://css-tricks.com/absolute-relative-fixed-positioining-how-do-they-differ/)  
- Get [detailed definitions and see examples](https://developer.mozilla.org/en-US/docs/Web/CSS/position)  
- One key concept to understand is [how to wrap an element inside a *positioned* ancestor](https://stackoverflow.com/a/4457821)  
- Use [`top`, `right` `bottom`, and `left`](https://css-tricks.com/almanac/properties/t/top-right-bottom-left/) to place an element somewhere other than in its default location    
- Use the [`z-index`](https://css-tricks.com/almanac/properties/z/z-index/) to control the order elements appear on the z-axis (i.e., the axis perpendicular to the plane of your screen)   
- `top`, `right` `bottom`,`left` and `z-index` only impact *positioned* elements  
- For more on `clip`, see [this description on W3Schools](https://www.w3schools.com/cssref/pr_pos_clip.asp)  

### Flexbox

  - Flexbox is a collection of CSS properties for aligning items in a row **or** column   
  - When using Flexbox, you need to turn an HTML element into a [flex container](https://www.w3schools.com/css/css3_flexbox.asp) by setting its `display` property to `flex`  
  - By defining an HTML element as `flex`, you activate a collection of [flex properties](https://www.w3schools.com/css/css3_flexbox_container.asp) that control how it aligns the elements inside it  
  - An element nested *directly* inside a flex container is a flex child    
  - A flex child exhibits the flex behavior defined by the flex container  
  - You can override the default flex child behavior by setting [flex properties for the child](https://www.w3schools.com/css/css3_flexbox_items.asp)  
  - [See how Flexbox works](https://codepen.io/enxaneta/full/adLPwv) on CodePen      
  - Common [use cases for using Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Typical_Use_Cases_of_Flexbox)  
  - Example of [centering items inside a flex container](https://codepen.io/danielwarren/pen/WzqBOZ)
  - Elements nested inside a flex child are not influenced by the flex container  
  - To learn about the flex properties and see examples, visit [CSS Trick's Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)  
  - Reinforce the [basics for Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)  
  - Level up your understanding of flex child properties by [learning to control ratios of flex children on the main axis](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Controlling_Ratios_of_Flex_Items_Along_the_Main_Ax)  
  - Learn about [wrapping flex children](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Mastering_Wrapping_of_Flex_Items)  
  
## [Grid and Forms](#grid-and-forms)   

### Grid
 - CSS Grid Layout is a collection of CSS properties for aligning items in rows **and** columns  
 - When using Grid, you need to turn an HTML element into a [grid container](https://www.w3schools.com/css/css_grid.asp) by setting its `display` property to `grid` 
 - By defining an HTML element as `grid`, you activate a collection of [grid properties](https://www.w3schools.com/css/css_grid_container.asp) that define the columns and rows inside it and also control how it aligns the elements inside it  
 - An element nested *directly* inside a grid container is a grid item    
 - By default, a grid container has one grid item per row in each column    
 - You can override the default grid item behavior by setting [grid properties for the item](https://www.w3schools.com/css/css_grid_item.asp)  
 - Detailed [explanation of Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Basic_Concepts_of_Grid_Layout)  
 - One [simple Grid example](https://codepen.io/simoneas02/pen/gmREyQ) and another [simple Grid example](https://codepen.io/mozilladevelopers/pen/Xejyed)  
 - For a comprehensive explanation of Grid, visit [CSS Trick's Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)  
 - Use Grid in combination with Flexbox and `position` to create intuitive and user-friendly layouts  
 - Read about the [relationship between Grid and other layout methods](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Relationship_of_Grid_Layout) 
 
### Forms  

- A form is used to collect input from users
- Using HTML, you can create a form on your webpage  
- You can use the HTML `form` tag to serve as a container for HTML form elements   
- A `form` tag comes with [form attributes](https://www.w3schools.com/html/html_forms_attributes.asp), like an attribute for what the form does when it's submitted, where to display the response it receives after submitting, and more     
- The HTML form elements that you can put inside a form include [labels, inputs, and buttons and more](https://www.w3schools.com/html/html_form_elements.asp)  
- HTML [inputs have attributes](https://www.w3schools.com/html/html_form_attributes.asp) that let you define and control your elements, for instance, by setting their value, making them read only, and more  
- See here for more about [form input attributes](https://www.w3schools.com/html/html_form_attributes_form.asp)  
- Here is a [comprehensive resource about `form` tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)  
- See an example of a [registration form](https://www.w3schools.com/howto/howto_css_register_form.asp)  
- Learn [how to disable spell checking](https://www.tutorialrepublic.com/faq/how-to-disable-spell-checking-in-html-forms.php) in your forms  


## [HTML and CSS Live Coding](#html-and-css-live-coding)  

The live coding session continues working on the live code from the previous lessons. Here are the tasks:

1. Add a new html file to your project; create a link in your index.html file that takes the user to your new html page; link your new HTML page to the same stylesheet as the index.html file. 
2. In your new html file, create three separate rows stacked vertically using Flexbox; style the rows so that you can see where one row starts and the other row ends  
3. In the top row, nest three HTML elements and align the items horizontally; style each nested element so that you can see its boundaries; make one of the elements grow twice as large as the others when extra space is available  
4. In the middle row, nest three HTML elements and align the items vertically; for the top nested item, put text in the upper left corner; for the middle nested item, put text in the center; for the bottom nested element, put text in the bottom right corner  
5. In the bottom row, add a form to your page and explicitly set three of its attributes  
6. Put four inputs in your form; two inputs must be text and the other two can be any input other than text (but not the same as each other)  
7. Explicitly set two attributes for each of your form inputs  
8. Add a custom CSS class to your form that includes at least 3 style properties  
9. Add a submit button to your form  
