- `!important`: A keyword added to a CSS property to override _all_ other declarations, including inline styles. **Use as a last resort**, as it breaks the natural cascade and makes debugging difficult.
    - `p { color: red !important; }`
- **ID vs. Class:**
    
    - `#id`: Selects one unique element. An ID must be unique per page.
        
    - `.class`: Selects all elements with that class. Can be used on multiple elements.
        
- **DRY (Don't Repeat Yourself):** A principle of software development aimed at reducing repetition. In CSS, use classes to apply the same styles to multiple elements instead of writing the same rules over and over.
    
- **Combinator Selectors:**
    
    - **Adjacent Sibling (`+`):** Selects an element that is the _next_ sibling. (`h1 + p` selects the first `<p>` right after an `<h1>`).
        
    - **General Sibling (`~`):** Selects all siblings that come after an element. (`h1 ~ p` selects all `<p>` tags that follow an `<h1>`).
        
- **Pseudo-Selectors:**
    
    - **Pseudo-classes (`:`):** Style an element based on its state.
        
        - `:hover`: When the user mouses over an element.
            
        - `:nth-child(n)`: Selects a child based on its position (e.g., `:nth-child(2)`, `:nth-child(odd)`).
            
    - **Pseudo-elements (`::`):** Style a specific part of an element.
        
        - `::before` / `::after`: Create a "fake" element before or after the content of the selected element, which can be styled.
            
        - `::placeholder`: Styles the placeholder text in an input field.
            
