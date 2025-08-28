### **More HTML Tags**

- **Definition List:** Used for key-value pairs.
    
    - `<dl>`: The list itself.
        
    - `<dt>`: Definition term (the key).
        
    - `<dd>`: Definition description (the value).
        
- **Formatting Tags:**
    
    - `<strong>`, `<b>`: Bold text (strong has semantic meaning).
        
    - `<em>`, `<i>`: Italicized text (em has semantic meaning).
        
    - `<u>`: Underlined.
        
    - `<s>`: Strikethrough.
        
- **Tables:** For displaying tabular data.
    
    - `<table>`: The table container.
        
    - `<thead>`, `<tbody>`, `<tfoot>`: Sections for header, body, and footer rows.
        
    - `<tr>`: A table row.
        
    - `<th>`: A table header cell (bold and centered).
        
    - `<td>`: A table data cell.
        
- **Semantic vs. Non-Semantic Tags:**
    
    - **Semantic:** Clearly describes its meaning to both the browser and developer (e.g., `<nav>`, `<article>`, `<footer>`). Good for SEO and accessibility.
        
    - **Non-Semantic:** Tells nothing about its content (e.g., `<div>`, `<span>`).
        

### **Forms & Input**

- **`<form>`:** A container for collecting user input.
    
    - `action`: The URL where the form data is sent upon submission.
        
    - `method`: The HTTP method to use.
        
        - `GET`: Appends form data to the URL. Visible, book-markable, and has a length limit. **Default method.** Good for search queries.
            
        - `POST`: Sends form data in the HTTP request body. Not visible in the URL. More secure for sensitive information like passwords.
            
- **`<input>`:** The most common form element. The `type` attribute defines its behavior.
    
    - `type="text"`: A single-line text field.
        
    - `type="password"`: A password field (masks input).
        
    - `type="email"`: Field for an email address.
        
    - `type="submit"`: A button that submits the form.
        
- **Other Form Elements:**
    
    - `<select>`: A dropdown list.
        
    - `<option>`: An item within a `<select>` list.