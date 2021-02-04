# Code Refactor Starter Code
Welcome to the Horiseon site, our focus when designinig this site is accesibility for all, including web devs!

## Accessibility features

This website has been re-styled keeping accesibility for all users as a top priority. The features explained below describe two of the main changes done to make the website more friendly towards users needing screen readers to navigate. Additionally, we have re-organazised the code in both the HTML and CSS files to make them more readabl; by grouping elements alike in a logical order and reducing symplifying their code.

### Adding `<Alt>` Atributes

Each one of the images in the document has a **`<alt>`** atribute attached to it to help screen readers interpret images for their users. A literal description of the images may take quite a lot of space, so instead we focused on describing the context where they take place.

### Adding HTML Semantics

We replaced most of the **`<div>`** tags in the original document and repaced them with easier to read tags that give the screen reader, and coders, a better idea of what area they are looking at.

####`<header>`

Here we have our **`<nav>`** element with each item in the menu linked to their correspondent content in the middle of the page.
    
As an additional feature we have added a *link* to the **`<H1>`** element so it redirects to the main page when clicked.

####`<sections>`

You will find 2 main sections in the document:

- **`<Hero>`**

        The main image in our site.

- **`<articles>`**
        
        Each of the 3 articles has been given a class called 'explanation' to enable CSS styling.

####`<aside>`

Our aside section is positioned on right column of our site. it currently doest not have any links attached to any of its elements.

####`<footer>`
        
The Footer has been modified to match the `<nav>` element's style. This makes the website looks a bit more cohesive, reinforcing our branding.

## CSS Tech 

In order to reduce the amount of code written, we decided to take an efficient approach when *floating* the elements found in the  `"main-content"` section.

Rather than *floating* each `<div>` and `<img>` for each of the 3 articles. We selected each of them and *floated* them in the same direction. Changed the % width values of each `<div>` and `<img>`, and gave the *parent* element the **`overlow:auto`** property, to keep the elements from going outside their containers.

Now, prior to this , our *grand-parent* element was given the **`display:inline-block`** property so each of our `<div>` and `<img>` elements can fit within the same line.  

-----

Thank you for visiting and happy coding!

-----


