# Frontend Development Journey

**Tech Stack:** HTML, CSS, Bootstrap, JavaScript (ES6+), and ReactJS.

## HTML(Hypertext Markup Language) Fundamentals

### 1. What is HTML?
HTML (Hypertext Markup Language) is the standard markup language for creating Web pages.
- It describes the structure of a Web page.
- It consists of HTML elements that tell the browser how to display the content.

### 2. What are HTML Elements?
HTML Elements are the building blocks of HTML that describe the structure and content of a web page.
- They generally consist of a start tag, content, and end tag.
  
**Syntax:**  `<tag>Content</tag>`

### 3. What is the structure of an HTML document?
**Syntax:**
```html
<!DOCTYPE html>
<html>
  <head>
    Metadata elements
  </head>
  <body>
    Document Content
  </body>
</html>
```
Note: The extension of an HTML file is .html


### 4. What is the use of the doctype?
The doctype declaration tells the type/version of the HTML document to the browser.  
This ensures that the HTML document is rendered in different browsers in the same and expected way.

### 5. What is the HTML head element and why do we use it?
The HTML head element is the container for the elements that provide extra information about the document (metadata).  
It describes the properties of the document such as title, character set, style sheets, scripts, etc.

### 6. What is meant by an HTML body element?
The HTML body element defines the main content of an HTML document that displays on the web page.  
It can contain text content, paragraphs, headings, images, tables, links, videos, etc.

### 7. What are the uses of HTML?
Some of the uses of HTML are:
- Structuring web pages: HTML elements define the headings, paragraphs, and other contents of a web page. Without HTML elements, the text on the webpage would all look the same.
- Creating Hyperlinks: With Hyperlinks, we can navigate within the HTML document, to other web pages, etc.
- Embedding images and videos: HTML elements, we can embed images and videos in the HTML document.

### 8. Can we design dynamic web pages using HTML?
No, HTML alone cannot design dynamic web pages.  
By combining HTML with JavaScript, we can create dynamic web pages.

### 9. What is the use of an HTML anchor element?
The HTML anchor element is used to navigate to other web resources or a specific HTML element within the HTML document.  

**Syntax:**  `<a href="URL">Content</a>`

### 10. What are the differences between HTML div and span elements?
div element:
- The HTML div element is a block-level element	
- It can be used to wrap around other HTML elements and apply CSS styles to many elements at once
  
span element:
- The HTML span element is an inline element
- It can be used to wrap a small portion of text, etc, and add CSS styles to it

### 11. What is an HTML script element?
- The HTML script element can be used to embed the JavaScript code.
- It can contain scripting statements, or it points to an external script file through the src attribute.
  
**Syntax:**
`<script src="counter.js"></script>`

### 12. How to display images on the web page?
We can display images on the web page using the HTML img element.
Generally, the HTML img element requires two main HTML attributes.
- src specifies the path to the image.
- alt specifies an alternate text for the image.
  
**Syntax:**
`<img src="IMAGE_URL" alt="image" />`

### 13. How to create a link in HTML, and what is the HTML target attribute?
- The HTML anchor element can be used to create links on a web page.
- It requires the HTML href attribute to specify the URL/ path of the page where the link goes to.

### HTML target attribute:
- The HTML target Attribute specifies where to open the linked web resource.
- It can have the following values:

### Value	Description
- _self	(Default value). It opens the document in the same window or tab as it was clicked.

- _blank	It opens the document in a new window or tab.

- _parent	It opens the document in a parent frame.

- _top	It opens the document in a full-body window.


### 14. What are the differences between the HTML ordered List and the HTML unordered List?
HTML ordered list	
- It is a collection of related items that follow some order or have a sequence	
- It is created using the ol element	
- By default, list items in the Ordered List are marked with numbers.
  
HTML unordered list:
- It is a collection of related items that have no special order or sequence
- It is created using the ul element- 
- By default, list items in the Unordered List are marked with bullets.

### 15. Explain the HTML block-level elements and inline elements.?
Block-level Elements:
- The HTML Block-level elements always start in a new line and take up the full width available. 
- So, an HTML Block-level element occupies the entire horizontal space of its parent element.
- Examples: HTML h1 element, HTML p element, HTML div element, etc.
  
Inline Elements:
- The HTML Inline elements do not start in a new line and take up the content width.
- Examples: HTML button element, HTML img element, HTML a element, etc.

### 16. Why are Meta elements used in HTML?
- Meta elements can contain information about character encoding, description, title of the document, etc.
- Meta elements are used to tell the browser about the page description, author of the template, character set, keywords, etc.
- Meta elements are used for search engine optimization to tell the search engine about the page's content.

#### 17. What is an HTML class Attribute?
- The class attribute in HTML is used to assign one or more class names to an element. CSS or JavaScript can then target these class names to style or manipulate elements.
  
**Syntax:**
`<tag class="class-name">Content</tag>`

### 18. Why Do We Use the HTML id Attribute?
- The id attribute in HTML is used to assign a unique identifier to an element. This ID must be unique within the entire HTML document.
- It can be used for styling an HTML element using CSS.
- It is also used by JavaScript to access and manipulate the HTML elements with the specific id.
  
**Syntax:** 
`<tag id="unique-id">Content</tag>`

### 19. What Are HTML Attributes?
- HTML attributes provide additional information about HTML elements. They are always specified in the opening tag and usually come in name/value pairs.
  
**Syntax:** 
`<tagname attribute="value">Content</tagname>`

### 20. Can we use the HTML p element inside an HTML span element?
- The HTML span element is an inline element, which should contain only other inline elements.
- So, as span is an inline element and p is a block-level element, we can't use the p element inside a span element.

❌ Invalid Example:
<span>
  <p>This is a paragraph inside a span. (Not allowed)</p>
</span>

✅ Valid Example:
<p><span>This is a span inside a paragraph. (Allowed)</span></p>

### 21. What Are Forms in HTML?
- Forms in HTML are used to collect user input. They are essential for things like login pages, registrations, searches, and feedback.
- How to Create a Form in HTML
You use the <form> element, which can contain input fields, buttons, labels, and more.
### Basic Form Syntax:
```html
<form action="/submit-url" method="POST">
     <!-- form fields go here -->
 </form>
 ```

### 🎯 Example: Simple Registration Form
```html
<form action="/submit" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required>
  <br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>
  <br><br>

  <input type="submit" value="Register">
</form>
```

### 22. What are the differences between the HTML checkbox and radio input elements?
HTML radio input element:
- It is used when only one option to be selected out of several available options.
- It is created by using an HTML input element with the type attribute value is set to radio.
  
HTML checkbox input element:
- It is used when more than one option to be selected out of several available options.
- It is also created by using the HTML input element with the type attribute value is set to checkbox.

### ✅ Checkbox Example:
```html
<h4>Select your hobbies:</h4>
<input type="checkbox" name="hobby" value="reading"> Reading
<input type="checkbox" name="hobby" value="music"> Music
<input type="checkbox" name="hobby" value="travel"> Travel
```

### ✅ Radio Button Example:
```html
<h4>Select your gender:</h4>
<input type="radio" name="gender" value="male"> Male
<input type="radio" name="gender" value="female"> Female
```

### 23. What are the different types of input elements available and their uses?

`type="text"`
- Used for single-line text input. Example: name, city, etc.
Syntax: 
`<input type="text">`

`type="password"`
- Hides the typed characters. Ideal for passwords.
Syntax:
`<input type="password">`

`type="email"`
- Accepts only valid email formats.
Syntax:
`<input type="email">`

`type="number"`
- Allows only numbers. You can set min, max, and step.
Syntax:
`<input type="number" min="1" max="100">`

`type="checkbox"`
- Let users select multiple options.
Syntax:
`<input type="checkbox" name="hobby" value="reading">`

`type="radio"`
- Let users select only one option in a group.
Syntax:
`<input type="radio" name="gender" value="male">`

`type="submit"`
- A button that submits the form data.
`<input type="submit" value="Submit">`

etc.

### 24. HTML Validation Attributes?
- required: Ensures the field isn't empty.
- minlength / maxlength: Sets character limits.
- type="email": Checks for a valid email format.
- type="number" with min/max: Ensures numerical limits.
- pattern: (not shown above) Allows regex-based validation for custom formats.

### 25. What Are Semantic Elements in HTML?
- Semantic HTML elements are tags that clearly describe their meaning and purpose in the structure of a webpage. These elements tell both the browser and developers what type of content they contain.

In short:
Semantic elements give meaning to your HTML.

Elements like ```html <header>, <main>, <nav>, <button>, and <label> ``` provide meaning and structure.

### ✅ Why Use Semantic HTML?
- Improves Accessibility
Screen readers understand the structure better.

- Better SEO
Search engines can understand content hierarchy and meaning.

- Improves Code Readability
Easier for developers to read and maintain.

- Future-Proof Code
Better compatibility with new devices, browsers, and tools.

### Semantic HTML Page Structure:
```html
<body>
  <header>
    <nav>
      <!-- Navigation links -->
    </nav>
  </header>

  <main>
    <section>
      <!-- Section content -->
    </section>

    <article>
      <!-- Article content -->
    </article>

    <aside>
      <!-- Sidebar content -->
    </aside>
  </main>

  <footer>
    <!-- Footer content -->
  </footer>
</body>
```
### 26. What is Accessibility in Web Development?
- Accessibility (often abbreviated as a11y) means designing websites and applications so that everyone, including people with disabilities, can perceive, understand, navigate, and interact with the web effectively.

### 27. What is an <iframe> in HTML?
An <iframe> (short for inline frame) is an HTML element used to embed another HTML document within the current document. It's like showing another website or webpage inside your current page.

**Syntax:**
```html
<iframe src="https://example.com" width="600" height="400"></iframe>
```

## CSS(Cascading Style Sheets) Fundamentals

### 1. What is CSS?
CSS stands for Cascading Style Sheets.
It is the stylesheet language that is used to define styles for the HTML documents, including the design, layout and variations in display for different devices and screen sizes.

### 2. How to link the CSS file to the HTML file?
- The HTML link element is used to link the CSS file to the HTML file. It should be placed in the HTML head element.
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Web Page</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <h1>Hello, world!</h1>
</body>
</html>
```
- The HTML rel attribute stands for a relationship of the linked document to the current document. In this case, it is a stylesheet.
- The HTML href attribute stands for the URL/path of the CSS file.


### 3. How to add CSS to the HTML document?
CSS can be added to HTML documents in 3 ways.

✅ 1. Inline CSS
- You add CSS directly to an HTML element using the style attribute.

✅ 2. Internal CSS
- In Internal CSS, CSS property-values are defined in the HTML style element inside the HTML head element.
- It is used to define the styles for a single HTML document.
  
✅ 3. External CSS (Best Practice)
- In External CSS, CSS property-values are defined in a separate .css file.
- It can be used to define the styles for many HTML documents.

### 4. What is a responsive web design?
Responsive web design:
- Responsive web design is an approach to making web pages give the best user experience on all devices.
- A responsive website will automatically adjust for different screen sizes and viewports.

### 5. What are the advantages and disadvantages of CSS?

✅ Advantages:
- Separation of content and design – Makes code cleaner and easier to manage.
- Reusability – One CSS file can style multiple HTML pages.
- Improved website performance – External stylesheets are cached by browsers.

❌ Disadvantages:
- Browser compatibility issues – Styles may render differently across browsers.
- Global scope in plain CSS – Styles can accidentally affect unintended elements.
- No logic or dynamic behavior – CSS can't handle conditions or interact dynamically without JavaScript.

### 6. What is meant by the CSS Selector and what are the different types of it?
The CSS Selectors are used to select the HTML elements that we want to style.

The different types of CSS Selectors are:

Simple Selectors
 - Class Selector
 - ID Selector
 - Type (tag name) Selector
 - Attribute Selector
 - Universal Selector
 - Pseudo-class

Compound Selectors, Complex Selectors and many more.

#### 7. What is the id attribute and how did you write in CSS?
The id attribute in HTML is used to uniquely identify an element on a webpage. Each id must be unique within a page, meaning no two elements should have the same id.

**Syntax in HTML**:
`<div id="main-content">Hello World</div>`
### How to write CSS using the id:
In CSS, you select an element with an id by using the hash symbol # followed by the id name.
```html
#main-content {
  color: blue;
  font-size: 20px;
}
```
This CSS rule will apply styling to the element with id="main-content".

### 8. What is CSS Specificity?

CSS Specificity is how browsers decide which CSS property values are the most relevant to an HTML element and apply those CSS property values to the HTML element.

In short:
- CSS Specificity is the priority system used to decide which CSS rule wins when multiple rules target the same element.###

### CSS specificity order from lowest to highest:

- Universal selector (*)

- Element/type selectors (div, p, etc.)

- Class selectors (.class), attribute selectors ([type="text"]), pseudo-classes (:hover)

- ID selectors (#id)

- Inline styles (style="...")

- !important (overrides all, not part of specificity but highest priority)

### 9. How to import font-family in CSS?
You can import a custom font in CSS using the @import rule or by linking it in HTML and then using it in your styles.

✅ Method 1: Using @import in CSS

```html
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

body {
  font-family: 'Roboto', sans-serif;
}
```
✅ Method 2: Using <link> in HTML
```html
<head>
  <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
</head>
```
Then in your CSS:
```html
body {
  font-family: 'Roboto', sans-serif;
}
```

### 10. What is the CSS border radius property?
The CSS border-radius property specifies the roundness of the four corners of an HTML element.

```html
.button {
  background-color: skyblue;
  border-radius: 20px;
}
```

### 11. What is the sequence of CSS margin properties?
- The sequence of CSS margin properties is margin-top, margin-right, margin-bottom, margin-left.

### 12. What is the CSS Box Model?

The CSS box model is essentially a box that wraps around every HTML element. It consists of margin, border, padding, and the actual content.

Each element is made up of four layers:

Content – The actual text or image inside the box

Padding – Space between the content and the border

Border – The edge around the padding (can be visible or invisible)

Margin – Space outside the border that separates the element from others

### 🧱 Visual Structure (from inside out):
```css
[ Margin ]
  [ Border ]
    [ Padding ]
      [ Content ]
```
### 13. Explain media queries and why are they used?
Media queries play a crucial part while developing Responsive Layouts.

Using Media queries, we can conditionally apply styles based on the device type (e.g. printers, TVs, etc.) and media features (e.g. viewport width, etc.).

**Syntax:**
```html
@media media-type and (media-feature-expression) {
  /* CSS rules go here */
}
```
Media Type: Media type describes the general category of devices. Possible types of media are screen, print, tv, all, etc.

Media Feature: Using Media Features, we can write Media Query for a specific feature. Examples: width, height, orientation, etc.

### 14. What is CSS Flexbox?
CSS Flexbox (short for Flexible Box Layout) is a CSS layout model that allows you to arrange elements in a one-dimensional row or column, and control how space is distributed among them even when their sizes are unknown or dynamic.

It simplifies layout design compared to floats or positioning.

### Flexbox Properties:

```html
display: flex;
flex-direction: row | column;
justify-content: flex-start | flex-end | center | space-between | space-around;
align-items: stretch | flex-start | flex-end | center;
```
### 15. What are the differences between display: none and visibility: hidden?

### display: none
1. It doesn't display the HTML element	
2. Space will not be allocated for an HTML element in the layout	

### visibility: hidden
1. It hides the HTML element (i.e cannot be seen in the layout/web page)
2. Space will be allocated for an HTML element in the layout

### 16. Explain CSS display property with the values inline and block?
The CSS display property with the value block converts an HTML element to a block-level element.
- The block-level element always starts on a new line.
- It always takes up the full width available
  
The CSS display property with the value inline converts an HTML element to an inline element.

- The inline element does not start on a new line.
- It only takes up as much width as necessary.

### 17. CSS Grid System 
CSS Grid is a two-dimensional layout system in CSS that allows web developers to create responsive layouts by organizing content into rows and columns using a grid-based structure.

```html
<div class="grid-container">
  <div>Box 1</div>
  <div>Box 2</div>
  <div>Box 3</div>
  <div>Box 4</div>
</div>

<style>
.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
}
.grid-container > div {
  background: #ddd;
  padding: 20px;
  text-align: center;
}
</style>
```


### 18. Bootstrap Grid System
Bootstrap uses a 12-column grid layout to create responsive page designs. It’s based on Flexbox and includes classes for different screen sizes:

**Basic Syntax:**
```html
<div class="container">
  <div class="row">
    <div class="col-md-4">Column 1</div>
    <div class="col-md-4">Column 2</div>
    <div class="col-md-4">Column 3</div>
  </div>
</div>
```

### esponsive Breakpoints:

`col- (extra small, <576px)`

`col-sm- (≥576px)`

`col-md- (≥768px)`

`col-lg- (≥992px)`

`col-xl- (≥1200px)`

`col-xxl- (≥1400px)`

### 19. Explain about positions in CSS?
CSS Position property determines how an HTML element is positioned in the document flow and how it behaves in relation to other elements.

The position property specifies the type of positioning method used for an element.

There are five different position values:

- static
- relative
- fixed
- absolute
- sticky

`Static`

- Default positioning.
- Element flows naturally in the page layout.
- It can't be moved with top, left, right, or bottom.

`Relative`
- Positioned relative to its original position.
- Can be moved using top, left, right, or bottom, but still takes up space in the flow.

`Absolute`
- Positioned relative to the nearest ancestor with a position other than static.
- Removed from the normal document flow (doesn’t affect the positioning of other elements).

`Fixed`
- Positioned relative to the viewport (browser window).
- Stays in the same spot even when you scroll.

`Sticky`
- Acts like relative at first.
- Becomes fixed when you scroll past a certain point.

### 20. Explain CSS Transitions
CSS Transitions allow you to smoothly change property values over a specified duration, making animations like fading, sliding, or resizing possible without JavaScript.

### Transition Properties:
- transition-property → What to animate (e.g., color, width)

- transition-duration → How long (e.g., 0.5s)

- transition-timing-function → The speed curve (ease, linear, ease-in, ease-out)

- transition-delay → Delay before it starts (e.g., 0.2s)

**Basic Syntax:**
```css
selector {
  transition: property duration timing-function delay;
}
```
### 21. Explain CSS Animations
CSS Animations allow you to create smooth, customizable animations directly in CSS without JavaScript. They are used to change property values over time (like color, size, position, etc.).

**Basic Structure**

🔹 Define Keyframes:
```css
@keyframes slideIn {
  from {
    transform: translateX(-100%);
  }
  to {
    transform: translateX(0);
  }
}
```
**Apply Animation:**
```css
.box {
  animation: slideIn 1s ease-in-out forwards;
}
```

## JavaScript Fundamental

### What is a Garbage Collector in JavaScript?

The garbage collector (GC) is an automatic memory management system in JavaScript that:

Finds and removes unused (unreachable) objects from memory so your app doesn't run out of memory.

Why is Garbage Collection needed?

- When you create variables, objects, or arrays in JS, they take up memory.

- If you don’t clean them up after you're done, memory keeps filling up — and your app may crash or slow down.

- JavaScript’s Garbage Collector does this cleanup automatically.

### difference between SSR (Server-Side Rendering) and CSR (Client-Side Rendering)?

both are ways to render content on websites, but they differ in when and where the HTML is generated.

### Server-Side Rendering (SSR)

Server-side rendering is the process of rendering(loading) the web pages on the server side and sending the fully rendered HTML to the client. In this, the server generates HTML dynamically based on the requested URL and data then sends it to the client.

### Client-Side Rendering (CSR)

Client side rendering is the process of rendering web pages on the client side using JavaScript after the initial HTML is loaded. In this, the browser loads a minimal HTML document then JavaScript retrieves data from the server and generates the HTML dynamically.

### What is difference between Call(), Apply(), Bind()? 

```
function cook(ing1,ing2,ing3){
    console.log(`${this.name} is having a meal with ${ing1}, ${ing2}, ${ing3}`)
}
const person = { name : "Jayaram"}
```

Call() -> Invokes the function immediately, with this set to thisArg, and accepts arguments one by one.

```// call()
cook.call(person,"rice",'beans',"water")
```

Apply() -> Invokes the function immediately, with this set to thisArg, but takes arguments as an array.

```// apply()
cook.apply(person,["rice",'beans',"water"])
```

Bind() -> Returns a new function, with this set to thisArg, and any present arguments, but doesn't invoke it immediately.

```// bind()
const cookForJayaram = cook.bind(person,"rice",'beans',"water")
cookForJayaram()
```












































