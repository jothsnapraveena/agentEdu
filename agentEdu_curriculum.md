# Agentic AI: A 6-Week Course for High Schoolers
### A Free Curriculum by AgentEdu · Created by Jothsna Praveena Pendyala

---

**Course Description**
This 6-week course introduces high school students to agentic AI — systems that can reason, plan, use tools, and adapt to achieve goals. Students progress from understanding what an AI agent is, to building and demoing their own working agent using free no-code tools. No prior coding experience required.

**Target Audience:** Grades 9–12 · AP CS Principles · Introduction to AI · Elective tech courses  
**Time Commitment:** ~60–90 minutes per week  
**Prerequisites:** None. Curiosity required.  
**Standards Alignment:** CSTA K-12 CS Standards · AI4K12 Big Ideas 1, 3, 4 · ISTE Student Standards  

---

## How to Use This Curriculum

Each week includes:
- **Learning objectives** — what students will be able to do
- **Key concepts** — terms and ideas to cover
- **Lesson outline** — timing guide for a 75-minute class
- **Discussion questions** — open-ended prompts for class conversation
- **Student activity** — hands-on assignment (worksheet or project)
- **Teacher notes** — facilitation tips and common student questions

Weeks 1–4 are concept-building. Week 5 is full hands-on build. Week 6 is reflection and future-thinking. You can run all 6 weeks or pick individual weeks as standalone modules.

---

## Week 1 — What Is an AI Agent?

### Learning Objectives
By the end of this lesson, students will be able to:
- Define an AI agent and distinguish it from a simple AI tool
- Identify the three stages of the agent reasoning loop: Think → Act → Observe
- Give 3 real-world examples of AI agents and explain what makes them "agentic"

### Key Concepts
| Term | Definition |
|---|---|
| AI Agent | A software system that perceives its environment, reasons about a goal, takes actions, and adapts based on feedback |
| Agentic AI | AI that has autonomy — it can plan and act without a human directing every step |
| The Reasoning Loop | Think (reason about the goal) → Act (do something) → Observe (see what happened) → repeat |
| LLM | Large Language Model — the "brain" that powers modern AI agents |
| Prompt | The instructions or question given to an AI |

### Lesson Outline (75 min)
- **0:00–0:10** — Hook: Show a 2-minute demo of a real AI agent (suggested: a coding assistant solving a bug, or a research agent finding information). Ask: "What did the AI just do that a basic chatbot couldn't?"
- **0:10–0:25** — Lecture: What makes AI "agentic"? The Think → Act → Observe loop explained with a simple diagram. Compare: calculator (not agentic) vs. AI research assistant (agentic).
- **0:25–0:40** — Group exploration: Show 3 real-world agents (customer service bot, coding assistant, content writer). Small groups identify what tools each agent uses and when it makes decisions.
- **0:40–0:65** — Student Activity (below)
- **0:65–0:75** — Share-out and wrap-up

### Discussion Questions
1. What's the difference between asking ChatGPT a question and giving an AI agent a task to complete on your behalf?
2. What would have to be true for an AI agent to be trustworthy enough to act without asking you first?
3. Can you think of a situation where an AI agent acting autonomously could go wrong?

### Student Activity — The Agent Hunt
Students choose a technology they use regularly (a recommendation engine, a voice assistant, an autocomplete tool, etc.) and fill in the Agent Profile worksheet:

```
Agent Name: _______________
What goal does it pursue? _______________
THINK: What does it reason about? _______________
ACT: What action does it take? _______________
OBSERVE: How does it learn from what happened? _______________
Is it fully autonomous or does a human stay in the loop? _______________
One way it could fail or make a mistake: _______________
```

### Teacher Notes
- Students often conflate "AI agent" with "chatbot." Emphasize that the key differentiator is autonomy — agents take sequences of actions to reach a goal, not just answer one question.
- If students struggle to identify agents, prompt: "Does it keep doing things after the first response, or does it stop?"

---

## Week 2 — The Brain Behind the Agent

### Learning Objectives
By the end of this lesson, students will be able to:
- Explain how a Large Language Model works at a conceptual level (next-token prediction)
- Write an effective prompt using at least 3 prompting techniques
- Identify when an AI response is confidently wrong (hallucination) and explain why it happens

### Key Concepts
| Term | Definition |
|---|---|
| Large Language Model (LLM) | A neural network trained on vast text data to predict what words come next |
| Token | The basic unit an LLM processes — roughly a word or part of a word |
| Hallucination | When an AI confidently states something false because it generates plausible-sounding text, not factual text |
| Chain-of-thought | Prompting an AI to "think step by step" before answering, which improves accuracy |
| System prompt | Background instructions given to an AI before the user interacts with it |
| Zero-shot vs few-shot | Zero-shot: no examples given. Few-shot: examples included in the prompt to guide the response. |

### Lesson Outline (75 min)
- **0:00–0:10** — Hook: Ask an AI a question it gets confidently wrong (try a recent event or a trick math problem). Discuss: why did it fail?
- **0:10–0:30** — Lecture: How LLMs work — explain next-token prediction with a simple analogy (autocomplete on your phone, scaled to billions of parameters). Why hallucination is a structural problem, not a bug.
- **0:30–0:50** — Live demo and practice: Show the difference between a vague prompt and a well-structured one. Introduce 4 techniques: (1) role assignment, (2) step-by-step instruction, (3) output format specification, (4) few-shot examples.
- **0:50–0:70** — Student Activity (below)
- **0:70–0:75** — Reflection and debrief

### Discussion Questions
1. If an LLM is essentially "predicting the next word," why does it seem to understand what we mean?
2. How is hallucination different from a human making a mistake? Is it more dangerous, or less?
3. If you were building an AI agent for something important (medical advice, legal documents), what safeguards would you add?

### Student Activity — The Prompt Engineering Challenge
Students compete to get the best output from an AI using only prompt engineering (no code). Three rounds:

**Round 1 — The Explainer:** Get the AI to explain quantum computing to a 10-year-old in exactly 5 sentences.  
**Round 2 — The Debugger:** Paste a broken piece of simple code. Get the AI to find the bug and explain why it's wrong.  
**Round 3 — The Planner:** Get the AI to create a complete study plan for an upcoming exam, including specific time blocks.

Students compare outputs and vote on the best prompt for each round. Debrief: what made the winning prompts work?

### Teacher Notes
- LLM mechanics can be simplified: "It's an extremely sophisticated autocomplete that learned patterns from most of the internet. It generates what sounds right — which is usually correct, but not always."
- Hallucination is a great teachable moment: AI is not a search engine. It generates, not retrieves.

---

## Week 3 — Tools & Memory

### Learning Objectives
By the end of this lesson, students will be able to:
- Explain why an LLM alone is limited and what tools add to agent capability
- Distinguish between short-term (in-context) and long-term (persistent) memory
- Describe at a high level how RAG (Retrieval-Augmented Generation) works

### Key Concepts
| Term | Definition |
|---|---|
| Tool calling | The ability of an AI agent to invoke an external function (search, calculator, code runner, database query) and use the result in its response |
| Context window | The amount of text an LLM can "see" at once — its short-term working memory |
| RAG | Retrieval-Augmented Generation — fetching relevant documents and giving them to the LLM so it answers from real information, not just training data |
| Vector database | A specialized database that stores information as mathematical representations (embeddings), enabling similarity-based retrieval |
| Persistent memory | Information stored outside the LLM and retrieved across multiple conversations |

### Lesson Outline (75 min)
- **0:00–0:10** — Hook: Ask an AI agent what happened in the news yesterday. Watch it fail or make things up. Then show it using a web search tool to answer correctly. Discussion: what changed?
- **0:10–0:30** — Lecture: The limitations of a bare LLM (no real-time data, no persistent memory, no ability to compute). How tools solve each limitation. Introduction to the tool-calling loop.
- **0:30–0:45** — Concept: RAG explained with a physical analogy. "Imagine taking an open-book test — RAG is giving the AI the right pages from the textbook before it answers."
- **0:45–0:70** — Student Activity (below)
- **0:70–0:75** — Debrief

### Discussion Questions
1. What kinds of tasks would you NOT trust an AI agent without tools to do? What about with tools?
2. If an AI can search the internet in real time, does that solve the hallucination problem? Why or why not?
3. What personal information would you be comfortable storing in an AI's long-term memory about you? Where's your limit?

### Student Activity — Build a Memory Bot
Using a free no-code platform (e.g., Claude.ai, ChatGPT with memory, or Zapier AI), students:
1. Start a conversation about a topic they care about (a hobby, a sports team, a show)
2. Give the AI specific facts to remember (their preferences, opinions, background)
3. End the conversation, start a new one
4. Test: does the AI remember what it was told?

Then students document: What did it remember? What did it forget? What would make this more useful in a real product?

### Teacher Notes
- RAG is the most practically important concept in this week. The analogy of "open-book test" lands well with students.
- Context window limits are easy to demonstrate live: paste a very long document and ask the AI about the beginning after it has processed the end.

---

## Week 4 — Multi-Agent Systems

### Learning Objectives
By the end of this lesson, students will be able to:
- Explain why multi-agent systems exist and when a single agent is insufficient
- Distinguish between an orchestrator agent and a worker agent
- Design a simple multi-agent pipeline for a specific task

### Key Concepts
| Term | Definition |
|---|---|
| Multi-agent system | A network of AI agents that collaborate to complete complex tasks |
| Orchestrator | The "manager" agent that breaks down a task and assigns subtasks to other agents |
| Worker/specialist agent | An agent with a specific skill (coding, writing, research, verification) |
| Handoff | The passing of information or control from one agent to another |
| Guardrails | Rules or checks that prevent an agent from taking harmful or unauthorized actions |
| Human-in-the-loop | A design pattern where humans review or approve agent actions before they execute |

### Lesson Outline (75 min)
- **0:00–0:10** — Hook: "Why do companies have departments instead of one all-knowing employee?" Draw the parallel to AI agent teams.
- **0:10–0:30** — Lecture: Real enterprise multi-agent examples. Show a diagram of how a research pipeline works: Orchestrator → Research Agent → Summarization Agent → Fact-Check Agent → Delivery Agent.
- **0:30–0:50** — Discussion: What can go wrong when agents hand off to each other? What happens when one agent makes an error that compounds through the chain?
- **0:50–0:70** — Student Activity (below)
- **0:70–0:75** — Gallery walk and debrief

### Discussion Questions
1. If you had a team of AI agents doing your homework, what would you want each one to specialize in?
2. How do you know which agent to trust if they disagree with each other?
3. At what point does a multi-agent system become too autonomous to be safe?

### Student Activity — Design Your Agent Team
Students work in pairs to design a multi-agent system for a scenario of their choice from this list:
- A homework helper that researches, writes, and checks for plagiarism
- A travel planner that researches, books, and sends confirmation emails
- A sports analyst that watches game data and writes weekly reports

For their chosen scenario, students fill out:
```
Task: _______________
Orchestrator Agent (its job): _______________
Worker Agent 1 (specialty + what it receives/produces): _______________
Worker Agent 2 (specialty + what it receives/produces): _______________
Worker Agent 3 (specialty + what it receives/produces): _______________
Where does a human need to stay in the loop? _______________
What's the biggest risk if something goes wrong? _______________
```

### Teacher Notes
- Students find the "team analogy" very intuitive. Push them to think about failure modes — what happens when one agent produces bad output that the next agent uses without checking?
- Human-in-the-loop is worth emphasizing: most production systems have at least one human checkpoint before irreversible actions (sending emails, making purchases, publishing content).

---

## Week 5 — Build Your First Agent

### Learning Objectives
By the end of this lesson, students will be able to:
- Use a no-code agent builder to create a functional AI agent
- Test their agent, identify failure modes, and iterate
- Present and demo their agent to peers

### Tools (all free, no account required for basic use)
- **Claude.ai** — for conversational agent building with tools enabled
- **ChatGPT with custom instructions + browsing** — for web-connected agents
- **Zapier AI Agents** — for connecting agents to real workflows
- **Make.com** — for multi-step automation with AI nodes
- Optional for advanced students: **Flowise** (open-source, visual LangChain builder)

### Lesson Outline (75 min)
- **0:00–0:10** — Introduction to the build challenge and tool walkthrough
- **0:10–0:20** — Demo: Teacher builds a simple research agent live in 10 minutes
- **0:20–0:60** — Build session: Students build their own agent
- **0:60–0:75** — Demo day: Each student/pair demos their agent (2–3 min each)

### The Build Challenge
Students choose one of three agent types to build:

**Option A — The Research Agent**  
Goal: Given any topic, the agent researches it, summarizes the key findings, and lists 3 questions still worth exploring.  
Suggested tools: web search, text summarization

**Option B — The Study Buddy Agent**  
Goal: Given a subject and a student's weak areas, the agent creates a personalized study plan with practice questions.  
Suggested tools: knowledge base (upload your own notes), question generation

**Option C — The Creative Agent**  
Goal: Given a genre, theme, and length, the agent writes a short story and then critiques its own writing.  
Suggested tools: writing, self-review

### Build Worksheet
```
Agent Name: _______________
What does it do (one sentence)? _______________
What tools did you give it? _______________
What is the most important instruction in its system prompt? _______________
Biggest failure you found while testing: _______________
How did you fix it (or how would you fix it)? _______________
One thing your agent does surprisingly well: _______________
One thing it still can't do: _______________
```

### Demo Day Rubric
| Criteria | 1 | 2 | 3 |
|---|---|---|---|
| Agent completes its stated goal | Rarely | Sometimes | Consistently |
| Student can explain how it works | Vague | Partially | Clearly |
| Student identified at least one failure mode | No | Partially | Yes, with fix attempt |
| Presentation clarity | Hard to follow | Understandable | Clear and engaging |

### Teacher Notes
- Give students 5 minutes of "break it on purpose" time during testing — ask them to try to make their agent fail. This teaches adversarial thinking and builds intuition for robustness.
- Some agents will work well, some won't. That's the lesson. The post-build debrief is more important than the build itself.

---

## Week 6 — AI Safety, Ethics & Your Future

### Learning Objectives
By the end of this lesson, students will be able to:
- Identify at least 4 things that can go wrong with AI agents
- Articulate the ethical responsibilities of AI builders
- Describe 3 career paths in AI and the skills they require

### Key Concepts
| Term | Definition |
|---|---|
| Hallucination | AI generating false information with high confidence |
| Bias | Systematic errors in AI output that reflect unfairness in training data |
| Prompt injection | An attack where malicious text tricks an AI agent into ignoring its instructions |
| Alignment | The challenge of making AI systems pursue the goals their builders actually intend |
| AI safety | The field of research dedicated to ensuring AI systems behave reliably and beneficially |
| Responsible AI | A set of principles (fairness, transparency, accountability, privacy) for ethical AI development |

### Lesson Outline (75 min)
- **0:00–0:15** — Review: What were the failure modes from Week 5 demo day? Categorize them on the board.
- **0:15–0:35** — Lecture: The 4 major risk categories in agentic AI (misinformation, bias, privacy, autonomy gone wrong). Real examples from deployed systems.
- **0:35–0:55** — Ethics Debate (below)
- **0:55–0:70** — Career landscape: AI Engineer, ML Engineer, AI Safety Researcher, Prompt Engineer, AI Ethics Officer — what each role does and what skills they need.
- **0:70–0:75** — Final reflection

### The Ethics Debate
Split the class into three groups. Each group argues one position, then presents:

**Scenario:** A hospital wants to deploy an AI agent that can autonomously order medications for patients based on their symptoms and records. The agent would act without a doctor approving each order to reduce wait times.

- **Group A — Build it:** The benefits outweigh the risks. Present the case for deployment.
- **Group B — Don't build it:** The risks are too high. Present the case against.
- **Group C — Build it with constraints:** It's possible, but only with specific safeguards. Propose the safeguard system.

### Final Reflection Worksheet
```
Complete these sentences:

The most surprising thing I learned in this course was _______________

An AI agent I would want to build someday is _______________

The most important question about AI that nobody seems to be asking is _______________

One thing builders of AI agents are responsible for is _______________

A career in AI that interests me is _______________ because _______________
```

### Teacher Notes
- The hospital debate generates strong opinions. Good. Let it run. Bring it back by asking: "Is there a version of this that all three groups could accept?"
- Career discussion: emphasize that AI careers are not just for coders. Ethics, law, communication, product design, and education are all critical fields right now.

---

## Standards Alignment

### CSTA K-12 CS Standards
- 3A-AP-13: Create prototypes that use algorithms to solve computational problems
- 3B-AP-14: Evaluate the correctness of a program
- 3A-IC-24: Evaluate the ways computing impacts personal, ethical, social, economic, and cultural practices
- 3B-IC-25: Evaluate computational artifacts to maximize their beneficial effects and minimize harmful effects

### AI4K12 Big Ideas
- Big Idea 1: Computers perceive the world using sensors
- Big Idea 3: Computers can learn from data
- Big Idea 4: Intelligent agents require many kinds of knowledge to interact naturally with humans

### ISTE Student Standards
- 1c: Knowledge constructor
- 1d: Innovative designer
- 1e: Computational thinker

---

## Recommended Tools & Resources

### No-Code Agent Builders (Free)
- Claude.ai (claude.ai)
- ChatGPT (chatgpt.com)
- Zapier AI Agents (zapier.com/ai)
- Make.com (make.com)
- Flowise — open source (flowiseai.com)

### Background Reading for Teachers
- "A Student's Introduction to Large Language Models" — fast.ai
- "AI4K12 Big Ideas in AI" — ai4k12.org
- "What Are AI Agents?" — IBM Technology (YouTube)

### Guest Speaker Ideas
- AI Engineers at local tech companies
- University ML/AI lab researchers
- AI ethics researchers or policy advisors
- Start-up founders building agent products

---

## License

This curriculum is free to use, adapt, and share under Creative Commons Attribution 4.0 (CC BY 4.0).  
Please credit: *AgentEdu · Created by Jothsna Praveena Pendyala · agentedu.org*

If you use this curriculum in your classroom, we'd love to hear from you.  
📬 hello@agentedu.org · 📸 @jothsna.aitales
