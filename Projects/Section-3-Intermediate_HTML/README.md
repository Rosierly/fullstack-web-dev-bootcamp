# Section 3: Intermediate HTML

## Key Points / What I Learned

- The List Elements
  - **Unordered List `<ul>`**: Bullet points
    ```html
    <ul>
      <li>...</li> <!-- list item -->
      <li>...</li>
      <li>...</li>
    </ul>
    ```
  - **Ordered List `<ol>`**: Numbered List
    ```html
    <ol>
      <li>...</li> <!-- list item -->
      <li>...</li>
      <li>...</li>
    </ol>
    ```

- **Nesting and Indentation** (for readability): nested lists

- **The Anchor Element `<a>`**
  ```html
  <a href="http://google.com">This is a link</a>
  ```

- **HTML Attributes**
  ```html
  <tag attribute=value>Content</tag>
  <!-- Separate attributes with a space -->
  <tag attribute=value another_attribute=value>Content</tag>
  ```
  - **Global Attributes of HTML Elements**
    ```html
    <!-- Example: draggable -->
    <a draggable=true>This is a link</a>
    ```

- **The Image Element**: self-closing tag (void element)
  ```html
  <img src="url" />
  ```
  
  - **The Alt Attribute** (Alternative Text Description)
    ```html
    <img src="https://picsum.photos/200" alt="forest at sunset"/>
    <!-- The number 200 at the end of the URL sets the image size (square: 200x200) -->
    ```


## Reference Documentation
- [MDN Web Docs – The Anchor Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/a)  

## Placeholder Image Resource
- [Picsum](https://picsum.photos)  

## Screen Reader Simulator - Chrome Browser Extension
- [Silktide](https://silktide.com/toolbar/screen-reader-simulator/) 

---

## Project : Birthday Invite 
A retro 90s-style website designed to help you invite guests to your next party.

<img src="3.4 Birthday Invite Project/goal.png" alt="Project Goal" width="500" height="auto">
