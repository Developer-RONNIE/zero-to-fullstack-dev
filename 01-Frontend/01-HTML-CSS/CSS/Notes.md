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
### ⭐ Borders 
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