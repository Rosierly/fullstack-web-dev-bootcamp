# Section 4: Multi-Page Websites

## Key Points / What I Learned

- **File Paths** (lead to a file or folder)
    ```html
    <!-- Root = Hard drive -->
    <!-- C: drive for Windows & Macintosh HD for Mac  -->
    📁 root 
    ├─ 📄 essay.docx
    └─ 📁 project
        ├─ 📄 index.html
        └─ 📁 images
            └─ 📄 cat.png
    ```

    - **Absolute** File Path
        ```html
        C:/Project/Images/cat.png <!-- for Windows -->
        /Project/Images/cat.png <!-- for Mac -->
        ```

    - **Relative** File Path
        ```html
        Images/cat.png <!-- if our code it's inside index.html-->
        ```

- **Special Characters**
  - Two double dots (..) --> go up a level
    ```html
    ../essay.docx  <!-- from inside project folder -->
    ```

  - Single dot (.) --> stay within the current directory
    ```html
    ./dog.png <!-- from inside index.html -->
    ```

- **Webpages**
    ```html
    📁 project 
    ├─ 📄 index.html
    ├─ 📄 about.html
    └─ 📁assets
        └─ 📁 images
            └─ 📄 cat.png

    <!-- Anchor Element for the About Page -->
    <a href="./about.html">About Page</a>
    ```

- **Wrapping Elements (Nesting)**
    ```html
    <a href="about.html">
        <img src="images/cat.png" alt="cat" />
    </a>
    <!-- Clicking the image will transfer you to another webpage -->
    ```

- **The HMTL Boilerplate**
    ```html
    <!DOCTYPE html>  <!-- the version of HTML the code was written in -->
    <html lang="en">  <!-- root of the document (the attribute lang stands for language) -->

        <head>
            <meta charset="UTF-8"> <!-- meta tag for the character set encoding of the webpage -->
            <title>My Website</title>
        </head>

        <body> <!-- all the content of our website goes inside the body element -->
            <h1>Hello World</h1>
        </body>
        
    </html>
    ```

    - **Shortcut for Boilerplate in VS Code**  
    Type "`!`" and hit `Enter` on the first selection


## Hosting Your Website with GitHub
1) New repo → `yourusername.github.io` (public)  
2) Upload files (`index.html` + assets)  
3) Go to Settings → Pages  
4) Source: `main` branch → `/root`  
5) Save & keep refreshing until you see the link  
6) Open: `https://yourusername.github.io`
    
- [Documentation about configuring a publishing source for your GitHub pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## Footer Element
- [MDN Web Docs – The Footer Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/footer)

---

## Project : Portfolio Project 
A simple website to showcase my projects so far, including links to a movie ranking page and a birthday invite project page.

<img src="./4.3 HTML Porfolio Project/goal.png" alt="Project Goal" width="600" height="auto">

## Capstone Project 1: Online Resume


<img src="./Capstone Project 1 - Online Resume/final_result.png" alt="Final Resutl" width="600" height="auto">