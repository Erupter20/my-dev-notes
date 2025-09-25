## 🌐 Networking & Client-Server
- **Networking:** exchange of data between devices using protocols.    
- **Client-Server Model:**
    - **Client:** frontend (browser/app).
    - **Server:** backend that processes requests, fetches from DB, returns responses.
    - **API:** bridge between client & server.        
    - **DB Driver/ORM:** connects backend to database.

**Analogy – Ordering Food:**
- You (client) order → waiter (API) → chef (server) → kitchen storage (database) → response is food.
- Even silence (timeout) is a response.
---
## 🔒 TCP vs UDP
- **TCP:** connection-oriented, reliable, ordered, acknowledged. Used for websites, APIs.
- **UDP:** connectionless, fast, no acknowledgement, can drop packets. Used for games, streaming.   
---
## 📦 Request & Response
1. Client makes request → packets sent over internet.
2. Response = HTML, CSS, JS, images, data.
3. Packets reassembled by browser. 
---
## 🖥️ Browser Parsing Basics
- **HTML Parser:** builds **DOM (Document Object Model)** tree.
- **CSS Parser:** builds **CSSOM (CSS Object Model)**.    
- **JavaScript:** parsed & executed by JS engine (though it can block rendering unless `async`/`defer`).  
**Key Trees:**
- DOM + CSSOM → **Render Tree** (only visible elements).
- Render Tree → **Layout** (positions & sizes).
- Layout → **Paint** (pixels drawn).
- Paint → **Composite** (final page).
> [!example] Parser Example  
> HTML: `<div><p>Hi</p></div>` → DOM: `div → p → "Hi"`.
- ## ⚡ Rendering Cycle
- **First Paint:** first visible render (blink).
- **Reflow:** recalculating layout when DOM changes.
- **Repaint:** redrawing pixels when style changes.    
- **Re-rendering/Reconciliation:** repeated updates cause performance issues.   
---
## 📝 Notes
- **JS Original Name:** Mocha → LiveScript → JavaScript.
- **Garbage Collection:** Mark & Sweep algorithm.
- **Prototypal Inheritance:** objects inherit via prototype chain.
---
## 🎯 Interview Triggers
> [!question] What’s the difference between TCP and UDP?  
> [!question] Walk me through what happens when you type a URL in the browser.  
> [!question] Explain DOM, CSSOM, Render Tree.

---
## ⚠️ Traps & Gotchas
> [!warning] Misconception: "JS is not parsed" → It **is parsed**; parsing can block rendering unless managed with `defer/async`.  
> [!warning] Spread operator (`...`) ≠ setter → it’s for shallow copying/merging.

