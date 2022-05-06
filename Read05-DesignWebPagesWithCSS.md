[Return to Code 102 Notes Page](https://krisdunning.github.io/reading-notes/Code102Notes.html)

# Design Web Pages With CSS Notes

*****

CSS stand for cascading style sheets and allows the developer control over the style and layout of their sites. Css is a rule based language and you define the rules by specifying group of styles that apply to elements on the page. 

CSS rules open with a "selector" and inside have "declarations" which are property/value pairs.

>h1{ color: red;}

The selector (h1) declares the color(property) is red(value).  

For a list of CSS properties please see <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Reference">MDN CSS Reference</a>  

CSS can be applied in 3 different ways:

- External Style Sheet- file with .css extention that can be linked from the HTML document.  
- Internal CSS- Usually for a single HTML page. Defined inside the `<style> </style>` element in the head section  
- Inline CSS- Used to style a single element. Add a style attribute to the element. `<h1 style="color:red;">` This is the least reccommended way to style a web page.  

If their are conflicting styles for an element the last style to be read will be used.  

*****
