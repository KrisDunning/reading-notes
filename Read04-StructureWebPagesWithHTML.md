[Return to main page](https://KrisDunning.github.io/reading-notes/)
# Structure Webpages with HTML

## Wireframe Notes

- Wireframes are often a good first step to UX/UI design
- Pen and paper work well as they are easily modified versus a digital mockup
- Research: Know your audience use cases, customer requirements and best practices or trends
- Understand and map out user flow, and information architechture - the way information is presented to the user
- K.I.S.S principle. Just a skeleton of the future layout is needed. Not a final design or color scheme
- Once you are happy prototype it out on figma or sketch
- 3 principles: Clarity, User confidence, Simplicity

*****

## HTML Basics Notes

- Elements- are wrappers for content and exist between opening and closing tage
- Content- the stuff inbetween the element tags
- Attributes- Contain extra info about the elements that wont show in the content
- Empty Element- empty elements like the `<img>` tag dont wrap content, so no closing tag
- example of basic HTML page layout  
  - `<!DOCTYPE html>`  
        `<html>`  
        `<head>`  
        `<meta charset="utf-8">`  
        `<title>Page Title</title>`  
        `</head>`  
        `<body>`  
        `<img src="image.jpg" alt="image">`  
        `</body>`
        `</html>`  

- image links- see above example
- heading- `<h1>` - `<h6>`  only up to H6
- comments- `<!--` inside is commented out`-->`
- parapgraphs- `<p>` `</p>` are the paragraph tags  
- Lists- Lists in HTML can be ordered or unordered  
    - Ordered- `<ol>` `</ol>` numbered 1,2,3,4,5
    - Unordered- `<ul>` `</ul>` no numbers  
- List items- each item in a list uses its own tags `<li>``</li>`  
-Links- Links use an anchor tag and an href attribute
    - `<a href="https://website.web">Click here</a>`

*****

## Semantics

In programmin Semantics refers to the *meaning* of the code. So an h1 *means* that it is a top level heading. You could style a single sentence `<p>` to *look* like a h1 but it wouldnt have the same semantics.

There are roughly 100 semantic elements available. Some of those are:
    - `<article>`
    - `<aside>`
    - `<figure>`
    - `<main>`
    - `<nav>`
    - `<footer>`

*****

## Resources

For more information please use the following sources:  
    -   <a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics">MDN HTML Basics</a>  
    -   <a href="https://developer.mozilla.org/en-US/docs/Learn/Front-end_web_developer">MDN Front-End Developer Learning Path</a>  
    -   <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element">MDN HTML Elements Refernce</a>  
