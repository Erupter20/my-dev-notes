## 🏗️ High-Level Flow
When you load a webpage:\
1. **Request sent** → DNS resolves → TCP/HTTPS handshake → server responds.
2. **Response received** → HTML, CSS, JS, images, data.
3. **Parsing & Tree Building:**
    - HTML → **DOM**
    - CSS → **CSSOM**        
    - JS → parsed & executed by JS engine        
4. **Combine DOM + CSSOM → Render Tree** (only visible nodes).    
5. **Layout (Reflow):** calculate positions & sizes.    
6. **Paint:** fill pixels.    
7. **Composite:** combine painted layers → display final page.  
---
## 🌳 The Trees Explained
- **DOM (Document Object Model):** structural representation of HTML.    
- **CSSOM (CSS Object Model):** parsed CSS rules, cascade applied.    
- **Render Tree:** DOM + CSSOM combined, only visible elements.    
- **Layout Tree:** computes exact geometry for each visible node.    
- **Paint:** assigns pixels, colors, borders, shadows.
---
## 🎨 Rendering Steps (Critical Path)
1. **Construct DOM** from HTML.    
2. **Construct CSSOM** from stylesheets.    
3. **Combine → Render Tree.**    
4. **Layout (Reflow):** dimensions, positions.    
5. **Paint:** draw fills, borders, text, shadows.    
6. **Composite:** assemble into final screen image.  
---
## 🔁 Reflow vs Repaint
- **Reflow (Layout):** triggered when geometry changes (adding/removing nodes, resizing).
- **Repaint:** triggered when visual styles change (color, background).    
- **Both are costly** → avoid frequent DOM writes.
---
## ⚡ Optimization Techniques
- Use **`defer`** / **`async`** for scripts to avoid blocking.    
- Batch DOM changes instead of line-by-line.    
- Minimize style recalculations (avoid inline styles when possible).    
- Use **requestAnimationFrame** for smooth animations.    
- Use **virtual DOM (React, Vue)** for efficient diffing.   
---
## 📝 Notes
- Browsers parse HTML **top-to-bottom, left-to-right**.
- Invisible nodes (like `display:none`) are in the DOM, not in the render tree.    
- CSS cascade: inline > ID > class > tag.
---
## 🎯 Interview Triggers

> [!question] Explain DOM, CSSOM, and Render Tree.  
> [!question] What is the difference between Reflow and Repaint?  
> [!question] How do `async` and `defer` affect rendering?
---

## ⚠️ Traps & Gotchas

> [!warning] Large reflows (like changing `font-size` on `<body>`) can trigger **full page re-layouts**.  
> [!warning] Avoid animating `width/height`; use `transform` (GPU-optimized).

---
