# Assignment 3 — CUJ Runthrough + Demo

## 1. Assignment Information
**Title:** CUJ Runthrough + Demo

## 2. Group Details
- **Ben Cheng** — 1007920341  
- **Brenden Yiping Wang** — 1007684828  
- **Chen Jiang** — 1007637167  
- **Zihao Wang** — 1008036698  

## 3. TL;DR (≤ 65 words)
React is a powerful JavaScript library that transforms how businesses build digital experiences. It delivers fast, scalable, and interactive user interfaces through reusable components and efficient updates. By reducing development time and enhancing performance, React helps startups launch products faster, improve customer engagement, and stay competitive in the marketplace.

## 4. User Goal (≤ 2 sentences)
As a frontend developer, I want to create an interactive, elegant, and well-readable interface with reusable React UI components, a huge ecosystem of libraries, and community support, so I can quickly iterate on modern designs and deliver a more tailored experience to users through our task board product.

## 5. User Persona

### Persona: Ben Cheng
- **Role / Background:** 4th-year Computer Science Specialist; ML & optimization experience from Ericsson internship  
- **Experience Level:** Strong in backend/algorithms; limited frontend frameworks  
- **Familiarity with Platform:** Used JavaScript before; first time building a full React app  

### Persona: Brenden Yiping Wang
- **Role / Background:** 4th-year CS Specialist; Full-Stack Developer at Chatsimple; cloud & AI systems
- **Experience Level:** Proficient full-stack; some modern frontend frameworks  
- **Familiarity with Platform:** Prior exposure to React; not expert-level  

### Persona: Chen Jiang
- **Role / Background:** 4th-year CS Specialist; 12-month internship at Roadpost (AWS + full-stack)  
- **Experience Level:** Experienced in full-stack & infra; moderate frontend skills  
- **Familiarity with Platform:** Some React; more backend-oriented  

### Persona: Zihao Wang (Leon)
- **Role / Background:** 4th-year CS Specialist; backend developer at VirgoCX  
- **Experience Level:** Strong backend (Java, Spring Boot, DBs); less frontend  
- **Familiarity with Platform:** Used Node.js; limited experience building full React apps  

## 6. Tools Used
- **React** – Core library for building reusable and interactive user interfaces.  
- **VS Code** – Primary code editor, enhanced with Prettier for clean, consistent code.  
- **Google Search** – A quick way to find answers, tutorials, and solutions when learning and developing.  
- **React Documentation** – Reliable source for understanding concepts, APIs, and recommended patterns.  
- **npm / yarn** – Package managers for installing, updating, and managing dependencies.  
- **React Developer Tools** (Chrome/Firefox Extension) – Specialized extension to inspect React component hierarchies directly in the browser.  
- **Material-UI** – Styling libraries to speed up UI design with ready-made, customizable components.  
- **Github** - Platform for version control and collaboration using Git.  
- **Taliwind** - Utility-first CSS framework for fast, customizable styling.  
- **Vercel** - Cloud platform for fast, seamless React app deployment.  

### Summary of findings
Working with React was both challenging and rewarding. Its component-based structure made building interactive interfaces intuitive, and after we understood props and state, development became even smoother. VS Code with Prettier kept our code clean, while React Documentation and Google Search together provided clarity when we faced challenges such as learning hooks, managing state across multiple components, and resolving dependency or version conflicts. 

We ran into several issues along the way. First, npm/yarn sometimes caused version mismatches, which slowed progress and forced us to spend more time on dependency management. Second, React Developer Tools struggled to display state changes in complex components, making debugging a pain point. Third, while Material-UI initially accelerated UI development, styling conflicts with custom CSS made it frustrating to maintain, which eventually led us to switch to Tailwind for faster and more flexible design.

These moments of confusion were frustrating but ultimately turned into valuable insights. We learned the importance of locking package versions to avoid build breaks, gained a deeper understanding of how React’s re-rendering works by debugging without over-relying on tools, and discovered that Tailwind’s utility-first approach gave us cleaner, more consistent styling compared to Material-UI. Overall, the strong ecosystem, reliable documentation, and community support helped us push through challenges and made the experience both productive and rewarding.



## 7. Recommendations

### Product Recommendations
React versions and component ecosystem are overly fragmented, making it easy for beginners to get lost when choosing tools; the official documentation and community tutorials are insufficient for complete mastery, leaving the learning path unclear; and some abstract design concepts (such as hooks lifecycle and reconciliation) lack comprehensive resources, making it difficult for developers to deeply understand and apply them correctly.  


### Recommendations for Future Users
It is recommended to spend time exploring the broader React ecosystem to understand the variety of available components and libraries; when encountering a new requirement, avoid reinventing the wheel and first search for established community solutions; and throughout development, maintain consistent coding practices to ensure readability and long-term maintainability of the project.


## 8. Highlights & Lowlights

| Task                      | Severity | Notes                                                                 |
|---------------------------|:--------:|-----------------------------------------------------------------------|
| Component-based structure |  Great   | Reusable, interactive UI felt intuitive once props/state were clear.  |
| Official documentation    | Moderate | Helpful, but light on advanced hooks lifecycle & reconciliation.      |
| State management          | Severe   | Cross-component state was confusing and caused early bugs.            |
| React DevTools            | Severe   | State changes not always obvious in complex component trees.          |
| Tailwind integration      |  Great   | Faster, consistent styling vs. MUI; boosted productivity.             |
| Quick deployments         |  Great   | Vercel deployed in minutes with simple config.                        |
| Context switching         | Moderate | Frequent hops between docs, tutorials, and error triage.              |

## 9. CUJ Overview Table (General Developer Flow with React)

| Task                                    | Time  | Switches |
| --------------------------------------- | ----- | -------- |
| Open IDE (VS Code) and project          | 2:00  | 1        |
| Google React packages/styling options   | 10:00 | 2        |
| Add styling and React packages          | 2:00  | 3        |
| Build reusable React components         | 12:00 | 3        |
| Assemble React interface (board layout) | 10:00 | 3        |
| Test React app locally                  | 8:00  | 2        |
| Deploy React app to Vercel              | 6:00  | 3        |
| Validate production deployment          | 4:00  | 2        |

**Total Time:** ~54:00  
**Total Switches:** ~19  

---



## 10. End-to-End User Journey Documentation (General Developer Flow with React)

**Total Time:** ~54:00  
**Total Switches:** ~19  

| Step                               | Notes (what + why )                                          | Screenshot                                                |
| ---------------------------------- | ------------------------------------------------------------ | --------------------------------------------------------- |
| 1. Open IDE & project              | **What:** Launched VS Code and opened the React repo. <br>**Why:** To access the project code and begin development. | ![image-20250921015432656](https://p.ipic.vip/rxgx3j.png) |
| 2. Google React packages/styling   | **What:** Searched for React-compatible UI libraries and styling tools. <br>**Why:** To choose reliable packages with strong community support. <br>**Struggle:** Too many options (MUI, Chakra, Tailwind). Decided on Tailwind for readability + ecosystem. | ![image-20250921015557740](https://p.ipic.vip/oyj06p.png) |
| 3. Add styling & React packages    | **What:** Installed TailwindCSS and React component libraries. <br>**Why:** To apply consistent styling and speed up UI building. <br> | ![image-20250921015837011](https://p.ipic.vip/0ez1xb.png) |
| 4. Build reusable React components | **What:** Created TicketCard, Form, and Button components in React. <br>**Why:** To make UI modular and maintainable. <br>**Struggle:** Props became messy. Grouped related props into objects for clarity. | ![i96eix](https://p.ipic.vip/0fmh4m.png)                  |
| 5. Assemble React interface        | **What:** Composed components into a board layout with columns. <br>**Why:** To provide a clear interface for ticket management. <br>**Struggle:** Column alignment broke on first render. Fixed by adjusting flex/grid CSS. | ![image-20250921020357510](https://p.ipic.vip/wu0aw2.png) |
| 6. Test locally                    | **What:** Ran React dev server; tested component rendering and flows. <br>**Why:** To ensure the app worked before deploying. <br> | ![image-20250921020505066](https://p.ipic.vip/w4f751.png) |
| 7. Deploy React app                | **What:** Pushed repo to GitHub, it will trigger a GitHub action to deploy on Vercel automatically <br>**Why:** To host the app for customer use. <br> | ![image-20250921020730072](https://p.ipic.vip/pgb9t1.png) |
| 8. Validate production             | **What:** Opened live React app on the browser, tested flows. <br>**Why:** To confirm production matched local behaviour. <br> | ![image-20250921021031041](https://p.ipic.vip/zo8eot.png) |
