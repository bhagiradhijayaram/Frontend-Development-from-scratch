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

### 8. Can we design dynamic web pages using HTML?
- No, we can't design dynamic web pages with HTML alone.
- By combining HTML with JavaScript, we can create dynamic web pages.

### 9. What is the use of an HTML anchor element?
- We use the HTML anchor elements to navigate to other web resources or a specific HTML element within the HTML document. They are also called Hyperlinks/ Links.
  
**Syntax:**
`<a href="URL">Content</a>`

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

### CSS(Cascading Style Sheets) Fundamentals

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

✅ Advantages of CSS:

Separation of content and style
- HTML handles structure, CSS handles styling, making both easier to maintain.
  
Reusability
- One CSS file can style multiple HTML pages, reducing repetition.

Faster Page Loading
- External stylesheets are cached by the browser, improving performance.

Easier Maintenance
- Changes to a single CSS file affect all linked HTML pages instantly.

Consistent Design
- Ensures uniform look and feel across the entire website.

Responsive Design
- Enables websites to adapt across devices using media queries.

❌ Disadvantages of CSS:

Browser Compatibility Issues
- Some styles may behave differently in different browsers.

Complexity in Large Projects
- Without proper structure (like BEM, SCSS, or CSS Modules), CSS can become messy.

No Logic or Conditionals
- CSS lacks built-in logic, making dynamic styling limited without JS or preprocessors.

Global Scope (in plain CSS)
- Styles can unintentionally affect other elements unless scoped carefully.














