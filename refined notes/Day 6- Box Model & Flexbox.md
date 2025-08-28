### **Fonts, Text, and Filters**
- **Font Properties:**
    
    - `font-family`: Specifies a prioritized list of fonts ("font stack").
        
    - `font-size`: Sets the size of the text.
        
    - `font-weight`: Sets the boldness (e.g., `normal`, `bold`, `400`, `700`).
        
    - `font-style`: Sets italics.
        
- **Text Properties:**
    
    - `text-align`: `left`, `right`, `center`, `justify`.
        
    - `text-decoration`: `underline`, `line-through`.
        
    - `text-transform`: `uppercase`, `lowercase`, `capitalize`.
        
- **Image Filters:** `filter: blur(5px);`, `filter: grayscale(100%);`, `filter: opacity(50%);`
    

### **The CSS Box Model**

Every HTML element is a rectangular box. The box model describes how this box is composed.

- **Content:** The innermost part, where your text or images appear.
    
- **Padding:** The transparent space between the content and the border.
    
    - **Syntax:** `padding: 10px;` (all sides), `padding: 10px 20px;` (top/bottom, left/right), `padding: 10px 20px 30px 40px;` (top, right, bottom, left).
        
- **Border:** A line that goes around the padding and content.
    
    - **Syntax:** `border: 2px solid black;` (shorthand for width, style, color).
        
- **Margin:** The transparent space _outside_ the border. It separates an element from its neighbors. Syntax is the same as padding.
    
- **Why is it needed?** The box model is the foundation of layout on the web. It defines how elements are sized and how they interact with each other in terms of spacing. Understanding it is critical for positioning elements correctly.
    

### **`box-sizing` Property**

This property defines how the `width` and `height` of an element are calculated.

1. **`content-box` (default):** The `width` and `height` properties apply _only_ to the content area. Padding and borders are added _on top of_ this width/height, making the element larger than you specified.
    
    - `Total Width = width + padding-left + padding-right + border-left + border-right`
        
2. **`border-box`:** The `width` and `height` properties apply to the area _up to and including the border_. Padding and borders are inside this defined width, so the element's rendered size is exactly what you set. **This is much more intuitive and is considered best practice.**
    

- **Universal Reset:** It's standard practice to set all elements to `border-box`.
    
    CSS
    
    ```
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    ```
    

### **Flexbox**

A one-dimensional layout model for arranging items in rows or columns.

- **Flex Container:** The parent element you apply `display: flex;` to.
    
- **Flex Items:** The direct children of the flex container.
    
- **Axis System:** Flexbox works along two axes.
    
    - **Main Axis:** The primary direction items are laid out in. By default, this is horizontal (left-to-right).
        
    - **Cross Axis:** Perpendicular to the main axis. By default, this is vertical (top-to-bottom).
        
    - `flex-direction: column;` swaps the axes: the main axis becomes vertical, and the cross axis becomes horizontal.
        
- **Key Properties (for the container):**
    
    - `display: flex;`: Enables flexbox.
        
    - `flex-direction`: `row` (default) or `column`.
        
    - `justify-content`: Aligns items along the **main axis**. (`flex-start`, `flex-end`, `center`, `space-between`).
        
    - `align-items`: Aligns items along the **cross axis**. (`flex-start`, `flex-end`, `center`, `stretch`).
        
- **How to Center a Div:** To perfectly center a child `div` inside a parent, make the parent a flex container and apply `center` to both axes.
    
    CSS
    
    ```
    .parent {
      display: flex;
      justify-content: center; /* Centers horizontally */
      align-items: center;     /* Centers vertically */
      height: 100vh;           /* Give parent a height to center within */
    }
    ```
    

---

## **Actionable Advice**

### **How to Implement & Remember**

1. **Build Small Projects:** Don't just read notes. After learning about forms, build a detailed registration form. After learning flexbox, build a navbar or a photo gallery. Practical application is the only way to make it stick.
    
2. **Use Browser DevTools:** Right-click on any website and "Inspect". The "Elements" panel shows you the HTML and CSS. The "Computed" tab is amazing for debugging the box model—it visually breaks down the content, padding, border, and margin of any element you select.
    
3. **Create a Portfolio:** Start building your portfolio _now_ using what you learn each day. It's the most important project you'll work on. Apply typography rules, use flexbox for layout, and build semantic forms.
    
4. **Post Your Work:** As your notes say, post consistently. Don't just post "I learned flexbox." Post a link to a CodePen or GitHub Pages site showing a layout you built _with_ flexbox. Show, don't just tell. This builds credibility and an online presence.