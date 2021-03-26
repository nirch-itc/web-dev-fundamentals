# CSS Basics  

Welcome to the third lesson! In this lesson, you learn the basics of CSS. You start with an introduction to CSS in which you learn about CSS syntax, basic style properties, and how to connect your HTML and CSS. Next, you learn how to write your own custom CSS classes by exploring CSS selectors, pseudo classes, pseudo elements, and animations. Finally, you see a live coding example of using CSS to style a webpage. The live coding session reinforces what you learn in the lesson. 

This lesson also helps prepare you for making your personal portfolio site. The code from the session is included in this repository. You can use it however you like, but as with any code you get from someone else, make sure you understand it well enough to explain it to someone before putting it in your own projects.  

In this lesson, you learn:  

- Hour 1: [Intro to CSS](#intro-to-css)    
- Hour 2: [Writing Custom CSS Classes](#writing-custom-css-classes)   
- Hour 3: [CSS Live Coding](#css-live-coding)  

The topics below outline what you learn in the live session. After the live session, you can use this material as a resource for guided self-learning. This document will serve you as a roadmap for gaining repetition with the material that you learn during the live session.   

## [Intro to CSS](#intro-to-css)  

  ### CSS Getting Started
  
  - CSS is the language for adding style to webpages  
  - Use styles to control properties of your HTML elements, like color, height, width, layout, font type, and more
  - Here is a [list of CSS properties](https://www.w3schools.com/cssref/)  
  - Write CSS code in a .css file or in your HTML file using the `style` attribute or `script` tags  
  - Recommended to use a .css file instead of the other options because it is easier to maintain  
  - Whichever style approach you use, be consistent, intuitive, and predictable so that reading and maintaining your code is easy  
  - When using a .css file, import it inside your HTML file in the `head` tag using a link tag having its `src` set to the .css file's relative path  
  
  ### Syntax
  
  - In your .css file, use the following syntax:
  
  ```css
  div {
      border-radius: 5px;
      color: orange;
      font-size: 18px;
      padding: 10px;
      margin: 10px;
  }
  
  .name-of-your-class {
      background-color: blue;
      font-size: 24px;
      padding: 10px;
    }
  ```
  
  - If writing a class for a tag type, you use the tag name: `p { . . .}` and the class applies to all tags of that type
  - The class name starts with `.` for custom classes followed by a name you give it; set any HTML element's `class` attribute to that name to give it that class's style     
  
  - In your HTML file, apply the class to HTML elements like this:
  
  ```html
    <div class="name-of-your-class">Welcome to ITC!</div>
  ```
  
  - You can apply a CSS class to as many HTML elements as you want  
  - For custom names, use names that describes the HTML element 
  - Make your custom CSS names nouns because your classes apply to objects, not functions  
  - Good names help bring your code to life when someone reads it!  
  - After the tag type or name is an object `{ }` comprised of key:value pairs separated by a semi-colon   
  - Each key is the name of a CSS property and each value defines that property for the class you're writing. 
  
  - When using the `style` attribute, you set an HTML element's style attribute to a string (not an object) containing key:value pairs separated by a semi-colon  
  - Like in a .css file, each key is the name of a CSS property and each value defines that property for the class you're writing  
  - Here is an example inside an HTML file:
  
  ```html
      <p style="color: gray; margin: 10px; padding: 20px; width: 50%;">
        This is text inside a paragraph tag.
      </p>
  ```
   
  ### Examples of CSS Style Properties for Design  
  - [margin](https://www.w3schools.com/css/css_margin.asp)  
  - [padding](w3schools.com/css/css_padding.asp)  
  - [height and width](w3schools.com/css/css_dimension.asp)  
  - [colors](https://www.w3schools.com/css/css_colors.asp)  
  - [links](https://www.w3schools.com/css/css_link.asp)  

  ### Examples of CSS Style Properties for Layout  
  - [`position` style property and its cousins top, right, bottom, left](https://www.w3schools.com/css/css_positioning.asp)  
  - [Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)  
  - [Grid Layout](https://css-tricks.com/snippets/css/complete-guide-grid/)  

## [Writing Custom CSS Classes](#writing-custom-css-classes)   
  
  ### Selectors
  - CSS selectors give you versatility when selecting HTML elements for style  
  - You saw an example of a selector above (i.e., `.name-of-your-class` is a `.class` selector)  
  - Look at this list of other [CSS selectors](https://www.w3schools.com/cssref/css_selectors.asp)  
  - When first learning, it's okay to keep things simple by using just the `.class` selector  
  
  ### Pseudo    
  - [Pseudo classes](https://www.w3schools.com/css/css_pseudo_classes.asp) define a special state of an element (e.g., hover)    
  - [Pseudo elements](https://www.w3schools.com/css/css_pseudo_elements.asp) style specific parts of an element (e.g., first letter of a div)  
  
  ### Animations  
  - Change property values gradually over a given time using [transitions](https://www.w3schools.com/css/css3_transitions.asp) or [keyframes](https://www.w3schools.com/css/css3_animations.asp) in combination with pseudo classes  
  - Learn more about [transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions) 
  - Examples of [simple animations](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/)  
    
## [CSS Live Coding](#css-live-coding)  

The live coding session continues working on the live code from the previous lesson. Here are the tasks:

 1. Style your title and subtitle by overriding their default font-size, color, and font-family
 2. Style the three links to remove the text-decoration, add some padding and margin, add a border and border-radius, add a cursor, align them horizontally, not vertically
 3. Add a side bar to your page that goes from the top to the bottom of your page on the right side and make it 200px wide; add other style to make it look professional; delete the div on the left side of your page from the previous lesson     
 4. Make the images circles and put one image in the sidebar and the other on the main part of the page; make the sidebar image small and the main image large; add one word of text below the small image  
 5. Add a placeholder to your text input, remove the border, and make the background color change when in focus 
 6. Add custom styles to each of your other two inputs  
 7. Add a card to your page that is the shape of a rectangle and put inside the card the title and subtitle  
 8. Use the `position` property to position the 6 inner-most elements in unique places within the 2 middle divs (hint: use position absolute with top, right, bottom, or left on an element nested inside a positioned element)    
 9. Add an animation that increases the scale of the enabled button when you hover over it 
 10. Add an animation that moves the disabled button left when you hover over it  
