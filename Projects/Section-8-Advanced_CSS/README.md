# Section 8: Advanced CSS

## Project : Web Design Agency Project 
A simple responsive agency website that adapts to desktop and mobile screens.


<div style="display: flex; align-items: flex-start; gap: 10px;">
  <img src="./8.4 Web Design Agency Project/assets/images/goal_desktop_version.png" 
       alt="Project Goal - Desktop Version" 
       width="570">
  <img src="./8.4 Web Design Agency Project/assets/images/goal_mobile_version.png" 
       alt="Project Goal - Mobile Version" 
       width="200">
</div>


## Key Points / What I Learned

- **CSS Display Property**  
    - **Block** - (default for most elements)
        ```css
        /* Full width, new line */
        h2 {display: block;}
        ```
    - **Inline**
        ```css
        /* Same line, size = content (cannot change width and height) */
        h2 {display: inline;}
        ```
    - **Inline-Block**
        ```css
        /* Same line + can set width/height */
        h2 {display: inline-block;}
        ```
    - **None**
        ```css
        /* Hides element (removed from layout) */
        h2 {display: none;}
        ```

- **Span Element**  
    It's a small inline container used to style part of text.
    ```html
    <p>Hello <span>Beautiful</span> World</p>
    ```
    ```css
    /* span element: by default has an inline display property */
    span {display: inline;}
    ```

- **CSS Float Property**  
    Positions an element to the left or right, allowing surrounding content to wrap around it.
    ```html
    <img ... />
    <p>text... </p>
    ```
    ```css
    img {float: left;}  /* our text wraps around the image */
    ```
    - **Clearing Floats** - How to avoid wrapping around unwanted elements (e.g. footer)?
        ```html
        <img ... />
        <p>text... </p>
        <footer>Copyright App Brewery</footer>
        ```
        ```css
        img {float: left;}
        /* stops elements from wrapping around floated items */
        footer {clear: left;} /* Possible values: left, right, both */
        ```

- **Responsive Websites**  
    Making layouts adapt to different screen sizes. Common approaches:
    1) **Media Queries**  
        Apply different styles depending on screen width, height, or other device features.
        ```css
        /* Default styling */
        div {
            background-color: blue;
            height: 200px;
            width: 200px;
        }

        /* Screens ≤ 600px */
        @media (max-width: 600px) {
            /* CSS for screens below or equal to 600px wide (breakpoint) */
            div {
                height: 100px;
                width: 100px;
            }
        }

        /* Screens ≥ 600px */
        @media (min-width: 600px) {
            /* Styles for larger screens */
        }

        /* Combine Breakpoints (600px ≤ width ≤ 900px) */
        @media (min-width: 600px) and (max-width: 900px) {
            /* Styles for screens between 600px and 900px */
        }
        ```
        ```css
        /* For screens in landscape mode */
        @media screen and (orientation: landscape) {
            /* Styles for landscape orientation */
        }

        /* Shorter (commonly used), you often don’t need the keyword screen */
        @media (orientation: landscape) {
            /* Styles for landscape orientation */
        }

        /* For printing */
        @media print {
            /* Styles for print (e.g., remove colors, adjust layout) */
        }
        ```
    2) **CSS Grid**  
        A layout system for creating flexible, two-dimensional layouts (rows + columns).
    3) **CSS Flexbox**  
        A one-dimensional layout system for aligning and distributing elements in a row or column.
    4) **External Frameworks e.g. Bootstrap**  
        Pre-built CSS/JS libraries with responsive components to speed up design.

- **Check Responsiveness on Chrome**
1) Go to `Developer Tools`
2) Click the `Toggle Device Toolbar(📱 icon)` or `Ctrl + Shift + M`
3) Choose a device (e.g., iPhone, iPad) or set custom width/height
4) Resize the screen to test breakpoints


## Using Media Queries
- [MDN Docs - Media Query](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Media_queries/Using)

## Object-Fit CSS Property
- [MDN Docs - object-fit](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/object-fit)
