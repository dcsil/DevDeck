# Assignment 7 — Competitive CUJ
## 1. Assignment Information:
Competitive CUJ

## 2. Group Details:
- **Group Name** — DevDeck  
- **Ben Cheng** — 1007920341  
- **Brenden Yiping Wang** — 1007684828  
- **Chen Jiang** — 1007637167  
- **Zihao Wang** — 1008036698  

## 3. TL;DR (Summary of Findings - max 65 words):
ClickUp is an integrated work management platform for tasks, docs, dashboards, and automation. We set up a Space, explored views, statuses, dependencies, automations, and Brain AI. After encountering pain points, we simplified statuses, limited Slack to critical events, focused dashboards on what is due and blocked, and wrote detailed prompts and templates. This reduced noise, improved clarity and speed, and sped up adoption.

## 4. User Goal (max 2 sentences):
As a product manager, I want to describe my product requirements and deadlines to ClickUp’s built-in AI assistant, so that it can turn them into a structured project plan with realistic timelines, task dependencies, and assignments for each team member.

---

## 5. Detailed Summary of Findings (approx. 600 words):

User Persona:  
- Persona: Ben Cheng  
Role / Background: 4th-year Computer Science Specialist, experience in ML and optimization from Ericsson internship  
Experience Level: Comfortable with collaborative tooling and agile workflows, confident in setting up project structures and automations  
Familiarity with Platform: Previously used ClickUp in a project to manage sprints, build dashboards, and configure custom fields  

- Persona: Brenden Yiping Wang  
Role / Background: 4th-year CS Specialist, Full Stack Developer at Chatsimple, works with cloud and AI systems  
Experience Level: Advanced grasp of project management practices, quick to master new tools and workflows  
Familiarity with Platform: New to ClickUp, no direct workspace experience yet  

- Persona: Chen Jiang  
Role / Background: 4th-year CS Specialist, 12-month internship at Roadpost focusing on AWS + full-stack development  
Experience Level: Proficient with project management concepts, comfortable learning new tooling quickly  
Familiarity with Platform: New to ClickUp, exploring core features for the first time  

- Persona: Zihao Wang (Leon)  
Role / Background: 4th-year CS Specialist, backend developer at VirgoCX  
Experience Level:  Experienced with team workflows and documentation, moderate familiarity with task tracking tools  
Familiarity with Platform: New to ClickUp, no prior hands-on usage  

### Tools Used
- ClickUp – All-in-one work management platform for planning, tracking, and collaboration.  
- ClickUp official Guide&Demo – The official tutorials and demos help users quickly understand the different components and features within the workspace.  
- Google Search – A quick way of finding ClickUp tutorials, setup guides, and solutions when learning the platform.  
- ClickUp AI – ClickUp developed AI platform that supports conversational queries, note-taking, App management, and more. Beyond its own “Brain AI” model, it can switch to other LLMs such as GPT5 and GPTmini.  

We set up a Team Space named Devdeck, created a new Project, and added two Lists to learn the basics. In List view, adding tasks, assignees, due dates, and comments felt straightforward. We linked a small dependency chain and checked it in Gantt. Once the dependency toggle was on, the relationships were clear.

Statuses tripped us up first. We started with a long list and kept second-guessing which one to use. After a quick retro, we cut it down to three plain verb states. With status, both List and Board views became scan-friendly, and tasks flowed faster.

Brain AI was helpful for summaries and drafting tasks, but one pain point stood out. The auto-generate tasks feature was slow, averaging about 30 seconds and sometimes taking more than a minute, with results that were sometimes off target. After many trials, we found that longer, detail-rich prompts led to noticeably faster responses and better accuracy. Adding clear context like scope, owner, due date, acceptance criteria, and dependencies in the request improved the output and reduced revisions. 

Automations were powerful but noisy. It integrates with Slack and other enterprise communication platforms and sends timely alerts and comment notifications, but the default setting is noisy and spams Slack. After tuning the settings, we kept only high-value triggers and restricted Slack notifications to critical events. The noise dropped, and the setup worked great.

Our first dashboard tried to include every component and felt cluttered and slow. We rebuilt it around three essentials: what is due soon, what is blocked, and who is overloaded. After removing unnecessary widgets, the dashboard became lighter, more useful, and much faster to load.

**Key takeaways for DevDeck:**

- Reduce prompt burden. Provide structured input panels and auto context so users do not need long prompts to get quality output.
- Prioritize speed for AI actions. Use lightweight execution paths and incremental updates so task creation feels instant.
- Make automations quiet by default. Push high-priority notifications only and surface an easy-to-use noise control panel.
- Design focused dashboards. Start with the three essentials and let users add modules gradually, with performance guardrails.
- Keep AI chat in line on the same page as tasks and views to prevent context switching.


### Highlights and Lowlights Table:

| Type     | Area / Theme                    | Observation                                                                                                     | Severity |
|----------|---------------------------------|-----------------------------------------------------------------------------------------------------------------|----------|
| Highlight| Core project management features| Workspace structure, board views, and scheduling workflows are mature and predictable to use.                  | Great    |
| Highlight| AI entry point & visibility     | The AI assistant is easy to find and invoke as a visible chat panel inside the UI.                             | Great    |
| Lowlight | Integration into workflow       | AI feels bolted on as a separate chat box instead of a deeply integrated “productivity layer.”                 | Moderate |
| Lowlight | Onboarding & guidance           | There is little guidance on how to use AI effectively, so users must learn best-practice prompts by trial.     | Moderate |
| Lowlight | Prompt burden / cognitive load  | Vague or natural prompts often produce generic results, forcing users to craft very structured prompts.        | Severe   |
| Lowlight | Task creation latency           | Inserting AI-generated tasks into a board can take 5-30 seconds, breaking flow and discouraging reuse.         | Severe   |
| Lowlight | Limited workflow intelligence   | AI rarely infers intent or proactively suggests workflows; it waits for manual prompts like a basic chatbot.   | Severe   |

### Product Recommendations
ClickUp demonstrates a strong foundation for AI-driven workflow management, but its assistant can evolve from a reactive chatbot into a deeply integrated productivity partner. To achieve this, several key improvements are recommended:  

- **Make the AI More Context-Aware**  
 Rather than forcing users to type perfect prompts, the system should automatically understand what users are doing. For example, when someone creates or updates a task, the AI could proactively suggest subtasks, summaries, or follow-ups. This would make the assistant feel more natural and useful instead of just a chat box. 

- **Improve Response Speed with Lightweight Execution Paths**  
 The current 5–30 second delay in inserting generated tasks interrupts user flow. Implementing asynchronous background operations and incremental task rendering could preserve responsiveness while heavy processes complete in the background — ensuring AI actions feel immediate.

- **Offer a Guided “AI Onboarding Journey”**  
 A short, interactive onboarding tutorial could teach users how to phrase effective prompts, combine multiple actions, and review outputs — reducing the early learning curve. A “show me how” panel that demonstrates real examples within the user’s workspace would help users achieve value on day one.

---

## 6. Competitor Product Analysis

ClickUp positions itself as a comprehensive project and task management platform with embedded AI assistance. Its AI feature is presented as a chat-driven add-on, enabling users to request summaries, generate task descriptions, and retrieve project insights. For this CUJ, I explored how ClickUp AI assists with task planning and lightweight project organization.  

- **Strengths:** 
ClickUp’s core value lies in its mature project management foundation: robust workspace structure, board views, templates, and scheduling workflows. As expected, it provides predictable and stable task organization features. The AI is easy to notice and access, clearly embedded as a visible chat panel, reducing friction for users who specifically want to “invoke an AI assistant.” For simple queries (e.g., rewriting a task description or summarizing a short document), the outputs are fast and accurate. Its UI is polished, consistent, and well-supported by onboarding tutorials and tooltips. 

- **Weaknesses:** 
Despite its visibility, ClickUp AI feels bolted on rather than integrated. The assistant often behaves like a standard constrained chatbot: prompts must be explicitly typed, context isn’t deeply embedded, and the assistant rarely infers intent from workspace activity. Workflow intelligence is limited — suggestions are generic and occasionally repetitive, showing clear prompt engineering boundaries rather than adaptive understanding.  
Most importantly, task-level automation is slow and disconnected: when inserting generated tasks into a board, delays occur for 5-30 seconds in simple cases. The assistant does not yet feel proactive or ambient — it waits to be asked rather than executing automatic pipelines.  

- **Comparison to DevDeck:**
DevDeck aims to function as an embedded intelligence layer, not merely a chat helper. While ClickUp’s approach surfaces AI visibly, DevDeck’s vision is to make AI invisible and contextual, automating friction points in planning, execution tracking, and system-level developer workflows. We do not plan to compete on general team-task UI breadth; instead, DevDeck differentiates through developer-specific, context-aware assistance and automation depth, offering stronger integration with code, terminals, and project artifacts — delivering workflow lift rather than optional chatbot help.

---

## 7. CUJ Overview Table

| Task (overview)                                              | Time  | Switches |
| ------------------------------------------------------------ | ----- | -------- |
| Open ClickUp and navigate to **DevDeck → List**              | 2 min | 0        |
| Identify AI entry points (Ask AI, Brain, in-task AI)         | 2 min | 0        |
| Review AI capabilities (Google Search + in-app help search)  | 5 min | 2        |
| Use **Brain** to generate FE/BE onboarding tickets from a prompt | 3 min | 0        |
| Observe insertion latency and confirm items in List          | 1 min | 0        |
| Open generated task; use **in-task Ask AI** to enrich description/subtasks | 4 min | 0        |
| Assign owner, dates, priority; finalize statuses/tags        | 3 min | 0        |

**Total Time:** **20 minutes**
 **Total Context Switches:** **2**

------

## 8. Full CUJ Table (Step-by-Step Documentation)

**Total Time:** **20 minutes**  **Total Context Switches:** **2**

| Step                                                     | Notes (What + Why)                                           | Screenshot                                                   |
| -------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1. Sign in to ClickUp                                    | **What:** From landing page, clicked **Log in** and entered workspace. **Why:** Start point. | ![image-20251106013248092](https://p.ipic.vip/umitex.png)    |
| 2. Open **DevDeck → Board**                              | **What:** Navigated to the team board where tasks will be created/inserted. | ![image-20251106013506402](https://p.ipic.vip/hizwo1.png)    |
| 3. Identify AI entry points                              | **What:** Located three AI buttons (Brain sidebar, top-bar **Ask AI**, in-task **Ask AI**). **Struggle:** Ambiguity on which button actually **creates items**. **Insight:** Brain = best for space-level actions; in-task AI = contextual editing. | ![image-20251106013757884](https://p.ipic.vip/4cwjrl.png)    |
| 4. **(switch)** Google Search for capabilities           | **What:** Searched “ClickUp Brain create tasks” to confirm which surface can create items. **Why:** Reduce prompt trial-and-error before generating. | ![image-20251106013843442](https://p.ipic.vip/48mp8a.png)    |
| 5. **(switch)** Read through ClickUp Brain Documentation | **What:** Back in ClickUp Brain introduction page, read through the documentation.” **Why:** Check expected behavior and where items appear. | ![image-20251106014031128](https://p.ipic.vip/9e0dir.png)    |
| 6. Prompt Brain to create tickets                        | **What:** In **Brain**, entered: “We are going to build the user onboarding portal of our ticket board app, please create tickets for both frontend and backend developers.” **Why:** Turn requirement into structured work. | ![image (38)](https://p.ipic.vip/kk67n5.png)                 |
| 7. Generate & insert (latency)                           | **Observation:** ~20–30s delay before items materialize in List; brief flow break. **Insight:** Latency is noticeable when inserting AI-generated tasks. | <img src="https://p.ipic.vip/6b9mv9.png" alt="image-20251106014503597" style="zoom: 33%;" /> |
| 8. Enrich with in-task AI                                | **What:** Opened “Develop frontend for user onboarding portal” and used **Ask AI** inside the task to improve description and propose subtasks. **Why:** Make the ticket actionable without manual drafting. | ![image-20251106014744913](https://p.ipic.vip/kgekzs.png)    |
| 9. Assign & schedule                                     | **What:** Set assignee, due date, priority. **Insight:** AI didn’t auto-assign—next time include assignee names/roles directly in the initial prompt. | ![image-20251106014853898](https://p.ipic.vip/qn7zwq.png)    |
