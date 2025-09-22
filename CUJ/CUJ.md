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
- **Role / Background:** Full-Stack Developer at Chatsimple; cloud & AI systems  
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
- **React** — Core library for reusable, interactive UIs  
- **VS Code** (+ **Prettier**) — Editor & formatting  
- **Google Search** — Tutorials, Q&A, troubleshooting  
- **React Documentation** — Concepts, APIs, patterns  
- **npm / yarn** — Dependency and script management  
- **React Developer Tools** (Chrome/Firefox) — Inspect component trees  
- **Material-UI** — Component library (initially used; styling conflicts)  
- **Tailwind CSS** — Utility-first styling (switched to Tailwind; faster and more consistent)  
- **GitHub** — Version control & collaboration  
- **Vercel** — Fast, seamless React deployment  

### Summary of findings
Working with React was both challenging and rewarding. Its component-based structure made building interactive interfaces intuitive, and after we understood props and state, development felt smoother. VS Code with Prettier kept our code clean, while React Documentation and Google Search together provided clarity when we faced challenges such as understanding hooks like useEffect, managing state across multiple components, and resolving dependency or version conflicts. This combination of official guidance and quick community solutions helped us overcome problems more effectively. npm/yarn worked smoothly most of the time, but version mismatches occasionally popped up and slowed us down. On the other hand, React Developer Tools did not always display state changes clearly in complex components, which sometimes made debugging harder than expected. Similarly, while Material-UI accelerated UI design, styling conflicts with custom CSS created extra work and confusion.(MUI不好用，改了tailwind

These moments of confusion were frustrating but ultimately taught us important lessons about optimization and dependency management. Overall, the combination of strong tools, reliable documentation, and community support helped us push through challenges and made the experience both productive and rewarding.


## 7. Recommendations

### Product Recommendations
- React versions and ecosystem are fragmented; beginners can get lost choosing tools.  
- Official docs + community tutorials are great for basics but thin for deep mastery; learning path can feel unclear.  
- Abstract concepts (hook lifecycles, reconciliation) lack comprehensive, cohesive resources for deep application.

### Recommendations for Future Users
- Explore the broader ecosystem first (routing, state, forms, styling) to choose the right tools.  
- Don’t reinvent the wheel—search for established community solutions before custom-building.  
- Maintain consistent coding standards (lint/format, folder structure) for readability and long-term maintainability.

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

- 