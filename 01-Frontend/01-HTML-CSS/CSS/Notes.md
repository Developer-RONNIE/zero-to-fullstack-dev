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

Shadows in CSS add **depth and dimension** to text and elements, making them look elevated or highlighted.

#### Horizontal Offset:
Distance of the shadow along the X-axis.  
- Positive → shadow moves **right**  
- Negative → shadow moves **left**  

#### Vertical Offset:
Distance of the shadow along the Y-axis.  
- Positive → shadow moves **down**  
- Negative → shadow moves **up**  

#### Blur Effect:
Controls the **softness or spread** of the shadow edges.  
- Higher value → softer, more blurred  
- Lower value → sharper edges  

#### Text Shadow:
Adds shadow to **text content**.  
- Syntax: `text-shadow: horizontal-offset vertical-offset blur-radius color;`  
- Example: `text-shadow: 2px 2px 5px black;` → shadow shifted 2px right & down with 5px blur  

#### Box Shadow:
Adds shadow to **elements** like divs, buttons, images.  
- Syntax: `box-shadow: horizontal-offset vertical-offset blur-radius color;`  
- Example: `box-shadow: 4px 4px 10px rgba(0,0,0,0.5);` → semi-transparent shadow

> 💡 **Refer this for better understanding:**  
> Check out [`colors.html`](./shadow.html) & [`style.css`](./style.css)



### ⭐ Margins

Margins in CSS create **space around elements**, separating them from other elements and controlling layout.

#### Margin Properties:

- `margin-top` → sets space above the element
- `margin-right` → sets space to the right of the element
- `margin-bottom` → sets space below the element
- `margin-left` → sets space to the left of the element

#### Shorthand Property:

- `margin: top right bottom left;` → allows setting all four sides in one line
- Example: `margin: 10px 20px 15px 5px;` → top 10px, right 20px, bottom 15px, left 5px

#### Auto Margin:

- `margin: auto;` → centers block elements horizontally when width is set
- Can also use individually: `margin-left: auto; margin-right: auto;` → horizontal centering

#### Checking Margins in Browser:

- **Shortcut** → Right-click on the element → Inspect → Look in the **Styles or Computed** tab
- Computed tab shows exact **margin values** for top, right, bottom, left

#### Notes:

- Margins do **not affect the element’s size**, only the space around it
- Collapsing margins can occur when vertical margins of adjacent elements meet → the larger margin is used

> 💡 **Refer this for better understanding:**  
> Check out [`colors.html`](./margin.html) & [`style.css`](./style.css)

### ⭐ Float

Float in CSS is used to **position elements to the left or right** within their container, allowing other content to wrap around them.

#### Float Properties:

- `float: left;` → moves the element to the **left** of its container
- `float: right;` → moves the element to the **right** of its container
- `float: none;` → default, element stays in normal flow

#### Clearing Floats:

- `clear: left;` → element will not move next to floated elements on the left
- `clear: right;` → element will not move next to floated elements on the right
- `clear: both;` → element will not move next to floated elements on either side

#### Notes on Body / Root:

- Applying float directly to `body` or `:root` is **not recommended**; floats are meant for individual elements inside containers
- For layout purposes, **flexbox or grid** is preferred over floating body elements

#### Browser Tip:

- Inspect floated elements in browser → right-click → Inspect → see how text and elements wrap around the floated item

> 💡 **Refer this for better understanding:**  
> Check out [`colors.html`](./float.html) & [`style.css`](./style.css)


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