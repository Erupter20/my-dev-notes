### **Networking & Client-Server**

- **Client-Server Architecture:** A model where a **client** (e.g., your browser) requests resources from a **server** (a powerful computer hosting websites).
    
    - **Analogy:** Ordering a meal. You (client) order from a menu (make a request) to the waiter, who goes to the kitchen (server). The kitchen prepares the meal and the waiter brings it back (the response).
        
    - Every request gets a response. Even an error or timeout is a type of response.
        
- **Application Layers:**
    
    - **Client (Frontend):** What you see and interact with.
        
    - **API (Bridge):** The "waiter." An Application Programming Interface that lets the frontend and backend communicate using a set of rules.
        
    - **Backend (Server-side):** The "kitchen." Processes requests, runs logic, and interacts with the database.
        
    - **Database:** Where application data is stored.
        
- **Connection Protocols:**
    
    - **TCP (Transmission Control Protocol):** Reliable and connection-oriented. It sends acknowledgments for data packets, ensuring everything arrives in order. Think of it as a tracked courier service. Slower but secure.
        
    - **UDP (User Datagram Protocol):** Fast and connectionless. It sends packets without acknowledgment. Think of it as dropping a letter in a mailbox; it's fast, but delivery isn't guaranteed. Used for streaming or gaming where speed > perfect accuracy.
        

### **How Browsers Render a Page**

1. **Request & Response:** You type a URL, the browser (client) requests data from the server.
    
2. **Packets:** The server sends back the website's code (HTML, CSS, JS) in small pieces called packets.
    
3. **Parsing:** The browser reassembles these packets and uses **parsers** to read the code from top to bottom, left to right.
    
    - **Example:** The HTML parser reads the HTML file and builds a tree-like object called the **DOM** (Document Object Model). The CSS parser does the same for CSS, creating the **CSSOM** (CSS Object Model).
        
4. **Render Tree:** The browser combines the DOM and CSSOM to create the **Render Tree**. This tree only includes elements that will be visually displayed (e.g., `<head>` or elements with `display: none;` are excluded).
    
5. **Layout & Paint:** The browser calculates the exact size and position of everything in the Render Tree (**Layout**). Then, it draws the pixels on the screen (**Painting**). This entire process is called **rendering**.
    

### **The Problem React Solves**

- **Reconciliation:** The initial rendering of a page. If you change a small piece of data (e.g., updating your username on a page), traditional websites would have to re-render the _entire page_ just for that one change. This is slow and inefficient.
    
- **Virtual DOM:** React creates a lightweight copy of the real DOM in memory, called the **Virtual DOM**.
    
    1. When data changes, React updates the Virtual DOM first.
        
    2. It then uses a **diffing algorithm** to compare the updated Virtual DOM with a snapshot of the real DOM before the change.
        
    3. It calculates the most efficient way to make these changes and updates _only the changed nodes_ in the real DOM, instead of re-rendering everything.
        
- **Other React Benefits:**
    
    - **State Management:** Solved issues like Facebook's "ghost notification" bug, where the UI didn't accurately reflect the application's true state. React `useState` hook ensures the UI and data stay in sync.
        
    - **SPA (Single Page Application):** React allows you to build SPAs. A **bundler** (like Webpack) compiles all your components and code into a single, highly optimized file. This file is loaded once, and subsequent navigation just updates the view dynamically without full page reloads.
        
    - **JSX:** A syntax extension for JavaScript that looks like HTML. It's not readable by browsers, so a **transpiler** like **Babel** converts it into regular JavaScript.
        
    - **History:** Facebook created React and made it open-source in **2013**.
        

### **JavaScript & Versioning**

- **Prototypal Inheritance:** A core JS feature allowing objects to inherit properties directly from other objects. This flexibility is a key reason why JS can be used for everything from frontend (React) to backend (Node.js).
    
- **Semantic Versioning (`package.json`):** A system for versioning packages, formatted as `MAJOR.MINOR.PATCH`.
    
    - `PATCH` (e.g., 2.0.**7**): Backwards-compatible bug fixes.
        
    - `MINOR` (e.g., 2.**0**.7): Backwards-compatible new features.
        
    - `MAJOR` (e.g., **2**.0.7): Breaking changes that are not backwards-compatible.
        
    - `^` (Caret): Allows updates to any future **minor** and **patch** versions (e.g., `^2.0.7` can update to `2.1.0` but not `3.0.0`). This is the standard and safest option.
        
    - `*` (Asterisk): Allows any update, including major breaking changes. **Avoid using this.**