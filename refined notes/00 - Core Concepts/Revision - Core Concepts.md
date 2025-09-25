# Revision - Core Concepts
## 🌐 Networking & Client-Server
- Client = frontend, Server = backend, API = bridge, DB driver = DB link.    
- Analogy: Restaurant → you order (request), chef cooks (server), waiter serves (API).    
- TCP: reliable, acknowledged, ordered.    
- UDP: fast, no ack, can drop packets.   
---
## 🏗️ Browser Rendering Pipeline
- HTML → DOM, CSS → CSSOM, JS parsed → combined → Render Tree.    
- Render Tree → Layout → Paint → Composite.    
- Reflow = geometry change.    
- Repaint = visual change.    
- Optimize with `defer/async`, batch DOM changes, requestAnimationFrame.   
---
## ⚡ React Motivation
- Problem: whole page reloads/blinks for small updates (Reconciliation Problem). 
- Virtual DOM: JS copy of DOM, diffing → minimal updates.
- Ghost notifications at Facebook → inconsistent UI states → React introduced predictable state updates.
- SPA: single HTML shell, JSX → Babel → bundler → optimized single-page app.
- Open-sourced 2013 by Facebook.
---
## 🎯 Interview Triggers
> [!question] Walk me through what happens when you type a URL.  
> [!question] DOM vs CSSOM vs Render Tree.  
> [!question] TCP vs UDP.  
> [!question] Why React was created?  
> [!question] Real DOM vs Virtual DOM.
---
## ⚠️ Traps & Gotchas
> [!warning] Misconception: “JS is not parsed” → it is parsed, can block rendering.  
> [!warning] Large reflows (changing `<body>` font-size) → full layout recalculation.  
> [!warning] JSX is **not HTML**; requires Babel transpilation.