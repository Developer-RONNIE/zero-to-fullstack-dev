# <div align="center"> HTML </div>



### Introduction
**History:** HTML (HyperText Markup Language) was first created by Tim Berners-Lee in 1991 and is the standard language used to create and structure web pages.  
**Use:** It provides the *skeleton* of a webpage — defining headings, paragraphs, links, images, forms, and overall page structure.  


###  Live Server Extension 
Install the VS Code Live Server extension → Open your HTML file → Right-click → Select **"Open with Live Server"** → The page automatically opens in your default browser and refreshes whenever you save changes. Perfect for live preview while coding.  


### index.html
**Boilerplate:** The main file that contains the structure of your webpage.  
- `<!DOCTYPE html>` tells the browser this is an HTML5 document.  
- `<html>` is the root container for all content.  
- `<head>` stores metadata like title, stylesheets, and scripts (not directly visible on the page).  
- `<title>` defines the page title (shown in browser tab).  
- `<body>` holds everything that is visible on the webpage — text, images, buttons, etc.  



### HTML Basics  

- `<>` → Angle brackets used to write HTML tags which tell the browser what each piece of content means.  
- `<!DOCTYPE html>` → Ensures the browser renders the page using the latest HTML5 standards.  
- `<html>` → The outermost container for the webpage.  
- `<head>` → Contains meta info, links to CSS/JS, and SEO info — does not display on the page.  
- `<title>` → Sets the page title in the browser tab and is important for SEO.  
- `<body>` → Holds everything you actually see — text, headings, links, images, etc.  
- `<h1>`–`<h6>` → Heading tags, where `<h1>` is the largest/most important and `<h6>` is the smallest.  
- `<br>` → Adds a single line break — good for breaking lines inside a paragraph.  
- `<hr>` → Inserts a horizontal line — useful for separating sections.  
- `<p>` → Creates a paragraph of text with some space before/after.  
- `lorem` → VS Code shortcut (`lorem10`, `lorem30`) to generate dummy text for testing layouts.  
- `<pre>` → Displays preformatted text exactly as written (keeps spaces, tabs, line breaks).  
- `<!-- comment -->` → Notes for developers, ignored by the browser — great for leaving reminders.  

> 💡 **Refer this for better understanding:**  
> Check out [`index.html`](./index.html) for a practical example of all the above tags in action.



 
### 📂 Project : 
**Task:** Create a new HTML page called `lyrics.html` → Add a heading with the song title (`<h1>`), break lines (`<br>`) between verses, add a horizontal line (`<hr>`) between chorus and verses, and use comments to mark sections.  
This project will help practice real-world HTML structure and make you comfortable writing and formatting HTML.  

> 💡 **Refer this for better understanding:**  
> Check out [`lyrics.html`](./lyrics.html) 


### Hyperlinks
### Hyperlinks & Anchor Tag  

- `<a>` → The anchor tag is used to create hyperlinks to navigate to other pages, websites, or files.  
- `href` → Stands for **Hyperlink Reference** — specifies the destination URL or file path.  
- `target="_blank"` → Opens the link in a new browser tab (useful for external sites like YouTube).  
- `title` → Adds extra info about the link; when you hover over the link, the title text appears as a tooltip.  



### Absolute vs Relative URLs  

- **Absolute URL:** Full web address that includes protocol (`https://`), domain name, and file path.  
  - Example:  
    ```html
    <a href="https://www.youtube.com/watch?v=abcd1234">Watch on YouTube</a>
    ```
  - Always points to the same resource no matter where your HTML file is.  

- **Relative URL:** Path relative to the current HTML file’s location.  
  - Example:  
    ```html
    <a href="./lyrics.html">Lyrics Page</a>
    ```
  - Used for linking files within your own project (doesn’t include `https://`).  

### 📂 Project : 
 **Task:**  
 Under the singer’s name (inside your `lyrics.html`), add a YouTube link to the song using `<a>`, `href`, `target="_blank"`, and `title`.  

> 💡 **Refer this for better understanding:**  
> Check out [`lyrics.html`](./lyrics.html) 

### Images

### Audio

### Video

### Favicons

### Text Formatting

### Span & Div

### Lists

### Tables

### Buttons

### Forms

### Headers & Footers


