# <div align="center"> CSS </div>

### ⭐ Introduction to CSS 

> 🧠 ** Prerequisites**  
> Check out [`./01-Frontend/01-HTML-CSS/HTML`](./01-Frontend/01-HTML-CSS/HTML) first ! 

- **Full Form:** Cascading Style Sheets.  
- **History:** CSS was created by **Håkon Wium Lie** in **1994** while working at **CERN**, the same research center where the World Wide Web was born.  
- **Purpose:** It was introduced to separate content (HTML) from presentation (design) — allowing developers to style web pages with colors, fonts, layouts, and spacing.  
- **First Used:** Officially adopted as a web standard by the **W3C (World Wide Web Consortium)** in **1996**.  


#### Ways to Apply CSS  

1. **Inline CSS**  
   - Written directly inside an HTML tag using the `style` attribute.  
   - Example: `<p style="color: blue;">Hello</p>`  
   - ✅ Quick styling, ❌ Not reusable or clean.  

2. **Internal CSS**  
   - Written inside the `<style>` tag within the `<head>` section of HTML.  
   - Example:  
     ```html
     <style>
       p { color: green; }
     </style>
     ```  
   - ✅ Useful for single-page styling.  

3. **External CSS**  
   - Written in a separate `.css` file and linked using `<link rel="stylesheet" href="style.css">`.  
   - ✅ **Advantages:**  
     - Code **reusability** — same CSS used for multiple pages.  
     - **Cleaner structure** — separates content (HTML) and design (CSS).  
     - Easier to **maintain and update** across large projects.  

> 💡 **Refer this for better understanding:**  
> Check out [`index.html`](./index.html) & [`style.css`](./style.css)

### ⭐ Colors 

CSS allows you to set colors using different formats.  

- **Color Names:**  
  Use predefined color names like `red`, `blue`, `green`, `yellow`, etc.  
  Example: `color: red;`  

- **RGB Values:**  
  Use the **Red, Green, Blue** color model.  
  Syntax: `rgb(255, 0, 0)` → Red color.  
  Each value ranges from **0 to 255**.  

- **Hexadecimal Values:**  
  Use a **6-digit** or **3-digit** hex code.  
  Syntax: `#RRGGBB` → e.g., `#ff0000` (Red), `#00ff00` (Green).  

- **HSL Values:**  
  Use **Hue, Saturation, Lightness**.  
  Syntax: `hsl(0, 100%, 50%)` → Red color.  
  - **Hue:** Base color (0–360° on color wheel)  
  - **Saturation:** Color intensity (0%–100%)  
  - **Lightness:** Brightness (0%–100%)  

> 💡 **Refer this for better understanding:**  
> Check out [`colors.html`](./colors.html) & [`style.css`](./style.css)

📘 **[Refer color docs](https://developer.mozilla.org/en-US/docs/Web/CSS/named-color)** – Complete list of all CSS named colors.


### ⭐ Fonts 

Fonts control how text looks on a webpage — its style, size, and weight.  

- **Fallback Fonts / Web-Safe Fonts:**  
  These are common fonts (like Arial, Verdana, Times New Roman) that are available on most devices.  
  - Example: `font-family: 'Poppins', Arial, sans-serif;`  
  - If the first font isn’t available, the browser uses the next one.  

- **Using ID in CSS:**  
  Each HTML element can have a unique `id`.  
  - In CSS, we target it using `#idName`.  
  - Example:  
    ```css
    #heading {
      font-size: 20px;
      color: navy;
    }
    ```  

- **Font Size (`font-size`):**  
  - Defines how big the text appears.  
  - Common units:  
    - `px` → fixed size (e.g., `16px`)  
    - `em` → relative to parent element’s size (e.g., `1em`, `1.5em`)  

- **Font Weight (`font-weight`):**  
  - Controls text thickness (e.g., `normal`, `bold`, `100–900`).  

- **Font Style (`font-style`):**  
  - Controls slant of text — values: `normal`, `italic`, `oblique`.  

---

#### Using Google Fonts  

- **Via API (Link):**  
  - Add a `<link>` tag from [Google Fonts](https://fonts.google.com) inside your HTML `<head>`.  
  - Example:  
    ```html
    <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
    ```  
  - Then use in CSS:  
    ```css
    body {
      font-family: 'Poppins', sans-serif;
    }
    ```  

- **Using Google Fonts Locally:**  
  - You can **download font files** and keep them inside a `fonts/` folder in your project.  
  - Then import using `@font-face`:  
    ```css
    @font-face {
      font-family: 'MyFont';
      src: url('fonts/MyFont.ttf');
    }
    ```  
  - ✅ Good for **offline use** and **faster loading** when hosting fonts locally.  

> 💡 **Refer this for better understanding:**  
> Check out [`colors.html`](./fonts.html) & [`style.css`](./style.css)


📘 **[Refer color docs](https://fonts.google.com/)** – Complete list of all Google Fonts.

### ⭐ Borders  

Borders in CSS are used to define the outline of an element — they create visible boundaries around boxes like divs, buttons, images, etc. You can control a border’s style, width, color, and radius to match your design.

#### Border Style:
The `border-style` property defines the type of border.  
Common values are:
- `solid` — A single solid line.  
- `dashed` — A line made of dashes.  
- `dotted` — A line made of dots.  
- `double` — Two solid lines.  
- `groove` — Gives a 3D grooved effect.  
- `ridge` — Opposite of groove; appears raised.  
- `inset` — Makes the element appear embedded.  
- `outset` — Makes the element appear pushed out.  
- `none` — Removes any border.

#### Border Width:
Specifies the thickness of the border.  
Example:  
`border-width: 2px;`

#### Border Color:
Defines the color of the border.  
Example:  
`border-color: red;`

#### Border Radius:
Used to make rounded corners.  
Example:  
`border-radius: 10px;`

#### Shorthand Syntax:
You can combine border properties into one line:  
`border: 2px solid red;`  
Here:
- `2px` → border width  
- `solid` → border style  
- `red` → border color  

#### Border Sides:
CSS lets you style each side of a border individually:  
- `border-top: 2px solid blue;` → applies only to the top edge.  
- `border-right: 2px dashed green;` → applies only to the right edge.  
- `border-bottom: 3px dotted red;` → applies only to the bottom edge.  
- `border-left: 1px double black;` → applies only to the left edge.  

This gives full control over how each side looks — useful when designing unique boxes, underlines, or separators.


> 💡 **Refer this for better understanding:**  
> Check out [`colors.html`](./border.html) & [`style.css`](./style.css)




### ⭐ Shadows 
### ⭐ Margins 
### ⭐ Float 
### ⭐ Overflow 
### ⭐ Display Property 
### ⭐ Height and Width 
### ⭐ Positions 
### ⭐ Background Images 
### ⭐ Combinators 
### ⭐ Pseudo-classes 
### ⭐ Pseudo-elements 
### ⭐ Pagination 
### ⭐ Dropdown Menus 
### ⭐ Navigation Bar 
### ⭐ Website Layout 
### ⭐ Image Gallery 
### ⭐ Icons 
### ⭐ Flexbox 
### ⭐ Transformations 
### ⭐ Animations 