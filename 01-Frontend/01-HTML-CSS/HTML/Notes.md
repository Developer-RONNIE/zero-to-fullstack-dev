# <div align="center"> HTML </div>



### ⭐Introduction
**History:** HTML (HyperText Markup Language) was first created by Tim Berners-Lee in 1991 and is the standard language used to create and structure web pages.  
**Use:** It provides the *skeleton* of a webpage — defining headings, paragraphs, links, images, forms, and overall page structure.  


###  ⭐Live Server Extension 
Install the VS Code Live Server extension → Open your HTML file → Right-click → Select **"Open with Live Server"** → The page automatically opens in your default browser and refreshes whenever you save changes. Perfect for live preview while coding.  


### ⭐index.html
**Boilerplate:** The main file that contains the structure of your webpage.  
- `<!DOCTYPE html>` tells the browser this is an HTML5 document.  
- `<html>` is the root container for all content.  
- `<head>` stores metadata like title, stylesheets, and scripts (not directly visible on the page).  
- `<title>` defines the page title (shown in browser tab).  
- `<body>` holds everything that is visible on the webpage — text, images, buttons, etc.  



### ⭐HTML Basics  
### Tags & Attributes  

- **Tags:** Define the structure of a webpage.  
  - Most tags have an opening `<tag>` and closing `</tag>` (e.g., `<p>...</p>`).  
  - Some are self-closing (e.g., `<br>`, `<img>`).  

- **Attributes:** Add extra information to a tag, written inside the opening tag as `name="value"`.  
  - Example: `<img src="album.jpg" alt="Album Cover">`  
  - `src` tells where the image is, `alt` describes it. 

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


### ⭐Hyperlinks
#### Hyperlinks & Anchor Tag  

- `<a>` → The anchor tag is used to create hyperlinks to navigate to other pages, websites, or files.  
- `href` → Stands for **Hyperlink Reference** — specifies the destination URL or file path.  
- `target="_blank"` → Opens the link in a new browser tab (useful for external sites like YouTube).  
- `title` → Adds extra info about the link; when you hover over the link, the title text appears as a tooltip.  



#### Absolute vs Relative URLs  

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

### ⭐Images  
- `<img>` → Used to display images on a webpage. It is a **self-closing tag** (no `</img>` needed).  
- `src` → Stands for **Source** — specifies the path (URL or relative path) of the image.  
- `alt` → Alternative text shown if the image cannot load; also improves SEO and accessibility for screen readers.  
- `height` / `width` → Set the size of the image. Can be in `px` (pixels) or `%` (percentage of the container).  
- **Images as hyperlinks:** You can wrap an `<img>` tag inside an `<a>` tag to make the image clickable.  
  ```html
  <a href="https://example.com" target="_blank">
    <img src="./album.jpg" alt="Album Cover" width="300">
  </a>
  ```

### 📂 Project : 
 **Task:**
Under the singer’s name (inside your lyrics.html), add the album cover as an image with alt text.

> 💡 **Refer this for better understanding:**  
> Check out [`lyrics.html`](./lyrics.html) 


### ⭐Audio  

- `<audio>` → Used to embed audio files in a webpage. Can have controls or play automatically.  
- `controls` → Displays built-in audio controls (play, pause, volume).  
- `autoplay` → Plays the audio automatically when the page loads *(often combined with `muted` due to browser restrictions)*.  
- `muted` → Starts the audio with sound off (required for autoplay to work on most browsers).  
- `loop` → Plays the audio file in an infinite loop.  
- `<source>` → Nested inside `<audio>`, specifies the audio file and its format.  
- `src` (inside `<source>`) → Path to the audio file.  
- `type` → Defines the MIME type of the file (so the browser knows how to play it).  
  - Common types:  
    - `audio/mpeg` → For `.mp3` files  
    - `audio/wav` → For `.wav` files  
    - `audio/ogg` → For `.ogg` files  

**Example:**  
```html
<audio controls autoplay muted loop>
  <source src="./song.mp3" type="audio/mpeg">
  <source src="./song.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>
```

> 💡 **Refer this for better understanding:**  
> Check out [`index.html`](./index.html) 


### ⭐Video
### Video  

- `<video>` → Used to embed videos on a webpage. Can display controls, autoplay, and loop just like `<audio>`.  
- `controls` → Adds built-in video controls (play, pause, volume, fullscreen).  
- `autoplay` → Plays the video automatically when the page loads *(must be combined with `muted` to work on most browsers)*.  
- `muted` → Starts the video with sound off (needed for autoplay to work).  
- `loop` → Repeats the video infinitely after it ends.  
- `width` / `height` → Sets the display size of the video in pixels.  
- `<source>` → Nested inside `<video>`, specifies the video file and format.  
- `src` (inside `<source>`) → Path to the video file.  
- `type` → Specifies the video format (MIME type) for better browser support.  

**Common Video Formats:**  
- `.mp4` → Most widely supported (MIME type: `video/mp4`).  
- `.webm` → High-quality, open format supported by most modern browsers (MIME type: `video/webm`).  
- `.ogg` → Open format, good for fallback support (MIME type: `video/ogg`).  

**Example:**  
```html
<video controls width="640" height="360" autoplay muted loop>
  <source src="./sample-video.mp4" type="video/mp4">
  <source src="./sample-video.webm" type="video/webm">
  <source src="./sample-video.ogv" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

> 💡 **Refer this for better understanding:**  
> Check out [`index.html`](./index.html) 



### ⭐Favicons 

- **What is a Favicon?**  
  - A favicon (short for "favorite icon") is the small icon that appears in the browser tab, bookmarks, and search results.  
  - It helps users quickly recognize your site.  

- **Why it is used:**  
  - Improves branding & professionalism.  
  - Makes your site easily identifiable in multiple open tabs.  
  - Appears in browser bookmarks, history, and search previews.  

- **Supported Formats:**  
  - `.ico` → Most common format (best compatibility across browsers).  
  - `.png` → High-quality transparent icon (commonly used).  
  - `.gif` → Animated favicon (rarely used, can be distracting).  
  - `.jpg` → Works, but no transparency support.  
  - `.svg` → Scalable vector favicon (modern, but not supported by all browsers).  

- **Attributes in `<link>` tag:**  
  - `rel` → Relationship attribute, set to `"icon"` (or `"shortcut icon"` for legacy browsers).  
  - `type` → Specifies the MIME type (`image/x-icon`, `image/png`, etc.).  
  - `href` → Path to your favicon file.  

**Example:**  
```html
<head>
  <link rel="icon" type="image/x-icon" href="./favicon.ico">
</head>
``` 

> 💡 **Refer this for better understanding:**  
> Check out [`index.html`](./index.html) for a practical example of all the above tags in action.



### ⭐Text Formatting
 
- `<b>` → **Bold** text (for styling, not importance).  
- `<strong>` → **Bold** text (adds semantic importance, better for SEO & screen readers).  
- `<i>` → *Italic* text (for styling).  
- `<em>` → *Italic* text (adds emphasis semantically).  
- `<u>` → Underlined text.  
- `<del>` → ~~Deleted~~ text (shows strike-through).  
- `<big>` → Makes text slightly larger.  
- `<small>` → Makes text smaller.  
- `<sub>` → Subscript text (e.g., H<sub>2</sub>O).  
- `<sup>` → Superscript text (e.g., X<sup>2</sup>).  
- `<code>` → Monospaced text (used to display code snippets).  
- `<mark>` → <mark>Highlighted</mark> text.  



### ⭐Span & Div
- **`<div>`** → Block-level container.  
  - Used to group larger sections of HTML.  
  - Starts on a new line and takes full width.  
  - Often used with CSS for layout.  

- **`<span>`** → Inline container.  
  - Used to style or group small parts of text inside a line.  
  - Does NOT break the line.  

✅ **Key Difference:**  
- `<div>` → big container, affects layout.  
- `<span>` → small container, affects part of text.  

### ⭐Lists


### ⭐Tables

### ⭐Buttons

### ⭐Forms

### ⭐Headers & Footers


