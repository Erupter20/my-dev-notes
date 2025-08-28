### **Core Concepts**
- **CSS (Cascading Style Sheets):** A language used to style the visual presentation of a document written in HTML.
- **Cascading:** The process of combining different stylesheets and resolving conflicts between CSS rules. The last defined rule wins.
- **Inline vs. Block Elements:**
    
    - **Block:** Starts on a new line and takes up the full width available (e.g., `<div>`, `<p>`, `<h1>`).
        
    - **Inline:** Does not start on a new line and only takes up as much width as necessary (e.g., `<span>`, `<a>`, `<img>`).
        
- **ARIA (Accessible Rich Internet Applications):** Attributes like `aria-label` help screen readers understand the purpose of an element, improving accessibility.
    

### **Applying CSS**

1. **External:** In a separate `.css` file. **Best practice.** Linked via `<link rel="stylesheet" href="styles.css">` in the `<head>`.
    
2. **Internal:** Inside a `<style>` tag within the HTML `<head>`. Useful for single-page styling.
    
3. **Inline:** As a `style` attribute directly on an HTML element (`<p style="color: blue;">`). **Avoid this** as it's hard to maintain.
    

### **Selectors & Specificity**

The browser uses specificity to decide which CSS rule applies if multiple rules point to the same element. **Priority Order (Highest to Lowest):**

1. **Inline styles** (e.g., `style="..."`)
    
2. **ID** (e.g., `#header`)
    
3. **Class, Attribute, Pseudo-class** (e.g., `.container`, `[type="text"]`, `:hover`)
    
4. **Tag/Element** (e.g., `h1`, `div`)
    

### **Units**

- **Absolute:** `px` (pixels). Fixed size. Not ideal for responsive design.
    
- **Relative:**
    
    - `%`: Relative to the parent element's size.
        
    - `em`: Relative to the font-size of the _parent_ element. Can be tricky due to nesting.
        
    - `rem` (root em): Relative to the font-size of the _root_ (`<html>`) element. **Highly recommended for responsive typography.**
        
    - `vh` / `vw`: 1/100th of the viewport's height or width.