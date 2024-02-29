- HTML (HyperText Markup Language) -content

  - Element, Tag, Attribute 

  - *ELEMENT*

    - designators that define the structure and content of the objects within a page 
      - Headings, paragraphs, anchors, etc

  - *TAG*

    - Surround element `<a>...</a>`

  - *ATTRIBUTE*

    - Properties used to provide additional information about an element
    - ex/ `id`, `class`, `src`, `href`
    - Defined within the opening tag after the elements name
      - `<a href="http://shayhowe.com/">Shay Howe</a>`

  - HTML Documents

    - Plain text documents saved with `.html` file extension

    - Use BBEdit app

    - all require this structure: 

    - `<!DOCTYPE html>`, `<html>`, `<head>`, and `<body>`

    - ```html
      <!DOCTYPE html>
      <html lang="en">
        <head> #whats inside the header will only show up in the browser window, not the page
          <meta charset="utf-8">
          <title>Hello World</title>
        </head>
        <body> #Visible content
          <h1>Hello World</h1>
        </body>
      </html>
      ```

      - Self enclosing Elements

        - ```html
          <br> <embed> <hr> <img> <input> <link> <meta> <param> <source> <wbr>
          ```

          

- CSS (Cascading Style Sheets) -appearance of content

  - `selectors`, `properties`, `values`

  - *SELECTORS*

    - Designates exactly which element/s within HTML to target and apply styles

    - May include a combination of qualifiers to selevt unique elements

    - Generally target an attribute value such as an `id` or `class` value or target type of element `<h1>` or `<p>`

      - `p { ... }`

    - *Type Selectors*

      - Select target by their element type (`<div>`,`<p>`) 
      - will target all with this element type

    - *Class Selectors*

      - Select an element based on the element’s `class` attribute value. Class selectors are a little more specific than type selectors, as they select a particular group of elements rather than all elements of one type.

      - Class selectors allow us to apply the same styles to different elements at once by using the same `class` attribute value across multiple elements.

      - Within CSS, classes are denoted by a leading period, `.`, followed by the `class` attribute value. Here the class selector will select any element containing the `class` attribute value of `awesome`, including both division and paragraph elements.

        - `.awesome { ... }`

        - ```html
          <div class="awesome">...</div>
          <p class="awesome">...</p>
          ```

    - *ID Selectors*

      - *ID* selectors are even more precise than class selectors, as they target only one unique element at a time. Just as class selectors use an element’s `class` attribute value as the selector, ID selectors use an element’s `id` attribute value as a selector.

      - Regardless of which type of element they appear on, `id` attribute values can only be used once per page. If used they should be reserved for significant elements.

      - Within CSS, ID selectors are denoted by a leading hash sign, `#`, followed by the `id`attribute value. Here the ID selector will only select the element containing the `id`attribute value of `shayhowe`.

      - `#shayhowe { ... }`

      - ```html
        <div id="shayhowe">...</div>
        ```

        

  - *PROPERTIES*

    - Determines the styles that will be applied to that element

    - ex/ `background`, `color`, `font-size`, `height`, and `width`,

      - ```css
        p {
          color: ...;
          font-size: ...;
        }
        ```

  - *VALUES*

    - ```css
      p {
        color: orange;
        font-size: 16px;
      }
      
      ```

- Referencing CSS within HTML

  - Reference CSS file within HTML file
  - include all styles in a single external style sheet
    - We reference this from within the `<head>` element of our HTML document
    - Make a `.css` document using BBEdit



- Check HTML with https://validator.w3.org/#validate_by_input

Check CSS with https://jigsaw.w3.org/css-validator/#validate_by_input

**Linter**

check computer code for errors, misuse, and style issues. Style and usage vs confromance to standards. Failing to follow best practices.