# Introduction to CSS (Cascading Style Sheets)

CSS, short for **Cascading Style Sheets**, is a fundamental web technology **used to define the presentation and layout of HTML documents**. It plays a crucial role in determining **how web pages look and feel, ensuring a visually appealing and consistent user experience across various devices and screen sizes.**

At its core, CSS allows web developers to apply styling to HTML elements, such as **fonts, colors, margins, padding, and positioning.** By separating the content (HTML) from the presentation (CSS), it **enables better organization and maintainability of web pages, making it easier to update styles without modifying the underlying content.**

## Without CSS
![](https://github.com/projectfinalaudio/CSS_FUNDAMENTALS/blob/master/images/without%20css.png?raw=true)

## With CSS
![](https://github.com/projectfinalaudio/CSS_FUNDAMENTALS/blob/master/images/with%20css.png?raw=true)

## Key Concepts of CSS:

**TIP**: The **CSS box model** is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below illustrates the box model:

![](https://github.com/projectfinalaudio/CSS_FUNDAMENTALS/blob/master/images/box%20model.png?raw=true)

**TIP**: The **box-sizing** property allows us to include the padding and border in an element's total width and height. If you set box-sizing: border-box; on an element, both the padding and border are included in the width and height:

![](https://github.com/projectfinalaudio/CSS_FUNDAMENTALS/blob/master/images/box%20sizing.png?raw=true)

1.  **Selectors**: Selectors target HTML elements and define which elements the styles should be applied to. They can target elements based on their **tag name, class, ID, attributes, or even their relationship with other elements**.
    ```css
    body {
        background: white;
    }

    #id {
        background: #242424;
    }

    .class {
        background: #eeee;
    }
    ```

    ```html
    <p data-attribute-name="value">This is HTML</p>
    ```

    ```css
    [data-attribute-name] {
        background: lime;
    }

    [data-attribute-name="value"] {
        background: #242424;
    }
    ```
2.  **Properties**: CSS properties dictate the appearance of the selected elements. Examples of properties include **"color" (for text color), "font-size" (for text size), "background-color" (for background color),** and many more.
    ```css
    body {
        background: white;
    }

    p {
        font-size: 12px;
        font-weight: 600;
        line-height: 1.2rem;
    }
    ```
3.  **Values**: Each CSS property is assigned a value that determines how the property should be applied. **For instance, the "color" property could have a value like "red," "#00ff00" (hexadecimal), or "rgb(255, 0, 0)" (RGB value)**. Useful resources: https://www.rapidtables.com/web/color/RGB_Color.html
     ```css
    body {
        background: white;
    }

    body {
        background: #eeee;
    }

    body {
        background: rgb(255, 255, 255);
    }

    body {
        hsl(0, 0%, 100%)
    } 

    p {
        font-size: 12px;
        font-weight: 600;
         letter-spacing: 1.2px;
        line-height: 1.2rem;
    }
    ```
4.  **Rules and Declarations**: CSS rules consist of a selector and a set of declarations enclosed in curly braces. Declarations are composed of a **property-value pair, separated by a colon and terminated with a semicolon.**
    
5.  **Stylesheet**: A CSS stylesheet is a file containing all the **CSS rules that style a web page**. It can be linked to an HTML document using the "link" element or included directly within the HTML file using the "style" element.
```html
<link rel="stylesheet" type="text/css" href="styles.css" />
```
6. The HREF in full stands for **Hypertext reference**. It represents a hyperlink from one web address to another.  The HREF property **specifies the hyperlink's destination.**
    
7.  **Cascading Order**: The "Cascading" in CSS refers to the process of determining which styles should be applied when multiple rules target the same element. The order of importance is generally based on specificity, origin, and order of appearance in the stylesheet.
    
## Getting Started:

To apply CSS styles to an HTML document, you can follow these steps:

1.  **Create an HTML file**: Start by creating a basic HTML file with the content you want to style.
    
2.  **Create a CSS file** (*preferred*): For larger projects or better organization, create a separate CSS file to hold all the styles.
    
3.  **Link CSS to HTML**: In the HTML file, use the "link" element in the "head" section to link to the CSS file. Alternatively, use the "style" element to include CSS directly within the HTML document.
    
4.  **Write CSS rules**: In the CSS file, or within the "style" element, write CSS rules by selecting HTML elements and applying properties with their respective values.
    
5.  **Save and view**: Save both the HTML and CSS files and open the HTML file in a web browser to see the styled content.
    
With these basic concepts, you can start experimenting with CSS to enhance the appearance of your web pages and create visually compelling designs. As you gain proficiency, you can explore more advanced features and techniques to build responsive and engaging user interfaces.
