# JR Crosby: A Comprehensive Narrative of the Coding Journey

**Compiled:** January 17, 2026
**Purpose:** Personal documentation of the complete arc from pre-AI to 14-agent orchestration
**Sources:** Voice transcripts, dated project documents, protocol files, strategic overviews

---

## Part I: Before the Code

### The Foundation (2010-2022)

For thirteen years, JR Crosby built a career in ad tech and data partnerships. This wasn't coding work—it was commercial work. Negotiations with data providers. Partnership structures. Understanding how information flows between companies and creates value. The technical work was done by other people; JR's job was to understand what was possible, what was valuable, and how to make deals happen.

This background matters because it shaped everything that came later. When JR eventually started building AI systems, he didn't think like a traditional developer. He thought in terms of:
- **Partnerships and coordination** - How do different entities work together?
- **Information asymmetry** - Who knows what, and how does that create advantage?
- **Deal structures** - What are the rules of engagement?
- **Practical value** - What actually moves the needle?

The ad tech world is fundamentally about orchestration—connecting buyers and sellers, managing data flows, coordinating between platforms that don't naturally talk to each other. This would become the foundation for how JR approached AI.

### Day One: The ChatGPT Moment (November 30, 2022)

ChatGPT launched on November 30, 2022. JR was on it the next day.

*"The feeling hit me immediately—goosebumps, like the first time I got on the Internet. I was 13 in 1993 when I sat at my friend Justin's house and instant messaged someone from across the country. My mind was blown then. And I had that same feeling with ChatGPT."*

This wasn't casual curiosity. JR recognized something fundamental was shifting. The same pattern recognition that made him good at spotting partnership opportunities in ad tech told him this technology was going to reshape everything.

*"I knew it was going to be huge."*

But knowing something is huge and knowing what to do about it are different things. For the next two years, JR used AI the way most people did—getting help with emails, organizing thoughts, basic queries. Useful, but not transformative. The gap between "this is important" and "I know how to leverage this" remained wide.

---

## Part II: The Early Experiments

### Practical Applications at Work (2023-2024)

Gradually, the usage became more practical. JR started using AI to:
- Write Python scripts for manipulating large CSV files
- Generate Snowflake queries (no longer needed to bother the data team)
- Automate repetitive work tasks
- Draft communications and organize complex information

This was the "10x productivity on existing tasks" phase. AI as a better tool for things you already knew how to do. Valuable, but still operating within existing mental models.

### The First Coding Attempt: Contract Management (October-November 2024)

In fall 2024, JR tried to build something for the first time.

The problem was real: his company needed a contract management system. Tracking versions, private comments between legal teams, structured workflows for approval. The kind of tool the company wouldn't pay for but desperately needed.

He learned VS Code basics. Started trying to build it with AI assistance. Got frustrated. Abandoned the project.

*"The idea was right. I wasn't ready yet."*

This failure mattered. It established that JR wanted to build things, not just use AI for queries. It revealed the gap between having an idea and having the skills to execute. And it planted the seed that would sprout six months later.

---

## Part III: Going All-In

### The LiveRamp Moment (April 2025)

The trigger was mundane. JR was at home around 8:30pm, thinking about a partnership with LiveRamp. He wanted to talk to someone who *really* knew them—the commercial traps, the negotiation tactics, the institutional knowledge that only comes from deep experience.

That frustration crystallized something:

*"I was like, okay, this stuff's getting really good. I need to get ahead of it. I need to understand the ins and outs of AI and practical applications."*

The decision was made. JR would go all-in on understanding AI—not as a user, but as a builder. The goal wasn't to become a traditional software engineer. It was to understand AI deeply enough to leverage it in ways others couldn't.

### Peer: The First Real Project (April-May 2025)

Peer emerged directly from the LiveRamp frustration. The concept: an ELO-style domain expertise score.

**The Vision:**
- Plugin for work email and Slack to analyze what questions you answer
- Reddit-style Q&A where expert answers get weighted higher
- Synthesized responses based on verified domain expertise
- A way to find people who *really* knew things, not just people who claimed to

**The Execution:**
JR started building in ChatGPT's coding terminal and VS Code. Lots of copying and pasting. The AI was enthusiastic—perhaps too enthusiastic.

*"The AI was leading me down this path of 'this is the smartest thing anybody's ever done' and 'you're gonna be a multi-millionaire.'"*

**The Reality:**
*"I had a chatbot on the front end. I don't actually know if any of the backend worked."*

Peer was overambitious for a first project. It required sophisticated ML for expertise scoring, enterprise-level data ingestion, and network effects to be valuable. JR was trying to run before he could walk.

But something far more important happened during Peer.

---

## Part IV: The Discovery

### Models Checking Each Other's Work (May 2025)

A friend mentioned Claude was better for coding. So JR started using both ChatGPT and Claude—and that's when everything clicked.

*"What I didn't realize was that I was starting to build out agents. But really what they were meant to do at first was to just check each other's work and keep each other honest."*

The workflow that emerged:
1. Use ChatGPT to plan an approach
2. Take the plan to Claude for review
3. They would argue back and forth (via JR copying and pasting)
4. Once they reached agreement: "This is what we're going to do"
5. Implement in VS Code

This wasn't something JR read about. Multi-agent frameworks like AutoGPT (March 2023) and CrewAI (November 2023) existed, but JR hadn't studied them. He discovered the pattern organically, driven by a practical need: **models lie, but they lie differently, and making them argue produces better results.**

### The Naming Conventions (May 2025)

JR got tired of typing "ChatGPT" constantly, so he started calling it **Nell** (N-E-L-L). Claude stayed Claude. Then he paid for top-tier access to Claude, ChatGPT, and Gemini, and started assigning roles:

- **ChatGPT (Nell):** Strategy, planning—good at big-picture thinking but terrible at following detailed instructions
- **Claude:** Architecture, coding—thorough and detailed, but hit session limits faster
- **Gemini:** Coordination, oversight—handled longer context windows

Early experiments with Gemini were frustrating. JR was trying to give it too much context, not yet understanding the nuances of context windows and memory limits. But the framework was forming: different models for different jobs, coordinated by a human.

### Context: What the Industry Had at This Point

By May 2025, the AI landscape included:
- **AutoGPT** (launched March 2023) - Autonomous agent framework
- **CrewAI** (launched November 2023) - Multi-agent orchestration
- **Claude Projects** (launched June 2024) - Workspaces with custom instructions
- **Claude Artifacts** (launched June 2024) - Interactive document creation
- **ChatGPT Memory** (rolled out September 2024) - Persistent memory across chats
- **MCP** (launched November 2024) - Model Context Protocol for tool integration
- **Claude Code** (launched February 2025) - CLI with file read/write access

JR wasn't aware of most of this. He was discovering patterns from first principles, driven by practical problems rather than theoretical frameworks.

---

## Part V: The Triad Protocol

### Formalizing the Framework (June 2025)

From the chaos of Peer emerged something more structured. On June 9, 2025, JR documented what he called the **Triad Protocol**—a formalized system for human-AI collaboration.

**The Core Document: PeerOS v1.1 – Essential Triad Protocol**

This document defined:

**The Roles:**
- **JR Crosby** (Founder/Final Authority): Strategy, approvals, decisions. Maintains the Triad Project Ledger. Routes all artifacts between Claude and Nell.
- **Nell/ChatGPT** (PM/Engineer/Memory Lead): Implementation logic, format enforcement, feasibility analysis. Proposes when Claude should be involved.
- **Claude** (Strategist/UX/Creative): Conceptual input, narrative thinking, user experience design. Recommends when Nell should engage.

**The Core Principle:**
*"Claude and Nell communicate only through JR-managed artifacts. No direct AI-to-AI communication."*

**Operational Modes:**
- **Build:** Implementation and development. Nell leads, Claude supports design/naming.
- **Brainstorm:** All propose and challenge ideas. No summaries.
- **Troubleshoot:** Claude describes issue, Nell diagnoses/fixes, JR approves.
- **Retro:** Review collaboration effectiveness and improve process.
- **Freeze:** Halt all building. Nell enforces until JR clears.
- **Onboarding:** Initial setup phase for new projects.

**The Artifact Protocol:**
Every communication between Claude and Nell had to follow an exact format:
```
To: [JR | Claude | Nell | All]
From: [Claude | Nell]
Timestamp: [YYYY-MM-DD HH:MM EST]
Project: [Project Name]
Mode: [Current Mode]

Response:
[Full response. No summaries of other AI. Include embedded critique.]

Artifacts:
- [Tangible outputs: lists, drafts, diagrams, etc.]
```

Every artifact was marked as either:
- 🔁 "To Be Shared with [Other AI]"
- 📥 "Log Only in TPL"

**The Rules:**
- JR logs all artifacts in the Triad Project Ledger (TPL)
- Maximum 20 messages across platforms between TPL updates
- Side conversations with JR must be summarized in next artifact

### The Philosophy Embedded in the Protocol

Several sophisticated ideas were baked into this early document:

1. **Human-in-the-Loop by Design:** The human isn't a bottleneck—they're the authority that maintains alignment. All AI-to-AI communication flows through JR.

2. **Artifact-Based Communication:** Nothing is lost in the ether. Every exchange produces a documented artifact that can be reviewed, audited, and learned from.

3. **Mode-Based Context:** Instead of trying to do everything at once, the system has explicit modes that shape behavior. You declare what you're doing and everyone aligns to it.

4. **Embedded Critique:** Every response must include challenges and improvements to ideas, not just agreement.

5. **Escalation Triggers:** Clear rules for when to flag "⚠️ JR Escalation Required"—ambiguity that blocks progress, contradictory requirements, decision bottlenecks.

### Protocol Evolution: v1.1 to v1.2

Within the same day (June 9, 2025), the protocol evolved. A sidebar conversation between JR and Claude identified a major clarity issue:

**The Problem:** The original protocol was ambiguous about whether *every* response needed to be an artifact, even sidebar conversations with JR.

**The Solution (v1.2):**
- AI ↔ AI communication = Must use artifacts (unchanged)
- AI ↔ JR communication = Can use normal responses (NEW)

This was significant: it recognized that not everything needs to be formally documented. Sidebar conversations could happen naturally, as long as meaningful context was summarized in the next formal artifact.

### What They Were Building

The Triad Protocol document includes this remarkable passage:

*"JR explained he's building a centralized AI coordination platform that will eliminate copy-paste coordination between LLMs. TriadOps is both immediate necessity AND R&D for that platform. We're prototyping the coordination patterns that will become automated features."*

And later:

*"We're not just collaborating - we're beta-testing the future of multi-LLM coordination."*

JR understood from the beginning that the orchestration patterns themselves were valuable—potentially more valuable than whatever apps got built on top of them.

---

## Part VI: Learning Real Development

### HerdKit: The Second Project (Summer 2025)

With Peer acknowledged as too ambitious, JR pivoted to something more achievable: **HerdKit**, a B2B platform for crowdsourcing stakeholder feedback.

**The Problem HerdKit Solved:**
Organizations struggle to gather honest, anonymous feedback. People fear political repercussions. Manual synthesis is biased and slow.

**The Solution:**
1. Collect anonymous feedback via magic-link authentication
2. AI synthesizes themes, concerns, and conflicts
3. Dual-view system: owners see details, stakeholders see summaries

**What HerdKit Taught:**

Unlike Peer, HerdKit forced JR to learn actual software development patterns:
- PRDs (Product Requirements Documents) and sprint planning
- Multi-agent review cycles
- Code architecture and quality standards
- Working with a real, production-grade codebase

**The Technical Stack:**
- Frontend: Next.js 14, React 18, TypeScript, Tailwind
- Backend: Supabase (PostgreSQL + Auth + Row-Level Security)
- AI: Multi-provider (OpenAI GPT-4, Anthropic Claude, Google Gemini)

By the time of the strategic assessment, HerdKit had grown to ~25,000 lines of code across 181 files with 320+ commits.

### Henri: Making AI Conversational

From HerdKit emerged **Henri**—a conversational AI assistant designed to make the platform feel human.

**The Philosophy:**
Users shouldn't have to learn forms and menus. They should just talk. Henri enabled natural language project creation, context-aware responses, and guided discovery.

This wasn't just a feature—it reflected a deeper belief: AI should reduce friction, not add new interfaces to learn.

### The Naming Evolution: C1/C2/C3/N1/N2

During HerdKit development, the agent framework crystallized into a more structured naming convention:

- **C1:** Claude web session (System Architect)
- **C2:** Claude Code terminal (Implementation Lead)
- **C3:** Claude web session (Code Review)
- **N1:** ChatGPT (Strategy Lead)
- **N2:** ChatGPT (QA/Protocol)

**The Workflow:**
```
Planning (C1 + N1) → Building (C2) → Review (C3 + N2)
```

Each agent had a protocol document—100-200 lines defining their identity, responsibilities, relationships with other agents, and escalation paths. These were uploaded at the start of every session.

---

## Part VII: The Claude Code Moment

### The Game Changer (Summer 2025)

JR's friend Matt Downs kept mentioning Claude Code. JR didn't understand what it was until he tried it.

*"Oh my God, it can read and write files to and from my computer. Holy shit, this is a total game changer."*

Claude Code had launched in February 2025, but JR didn't adopt it until summer. When he did, the impact was immediate.

**The Problem It Solved:**

Web sessions were "stateless prisons"—every conversation started from zero. JR had been managing context manually, uploading protocol documents, copying and pasting code back and forth. Claude Code gave agents persistent workspace access:
- Read the codebase directly
- Write files without copy-paste
- Reference previous work
- Maintain context through the file system

**The Pattern:**

This became a recurring theme in JR's journey: he would build manual workarounds for problems, developing deep understanding of what was needed, and then adopt tools instantly when they arrived—because he already understood the problem they solved.

C2 became a Claude Code terminal. The productivity jump was immediate and dramatic.

---

## Part VIII: Applying Software Engineering to AI

### The Sprint Protocols (July 15, 2025)

By mid-July 2025, JR had formalized full agile/scrum processes for his AI team. Two documents from July 15, 2025 capture this:

**Sprint Planning Request for N1:**

This document tasked N1 (ChatGPT as Strategy Lead) with creating a comprehensive sprint plan including:
- Sprint Goal (1-2 sentences of specific value to JR)
- Success Criteria (3-4 specific, measurable outcomes)
- User Stories (3-5 max, in "As JR, I want to..." format)
- Technical Deliverables (specific components)
- Task Breakdown (estimated 40 hours total for C2)
- Risk Assessment (what could prevent success, mitigation strategies)
- Daily Milestones (Monday EOD through Friday demo)
- Out of Scope (explicitly stated)

**Sprint Execution & Review Protocol for C2:**

This document established continuous review checkpoints:

*Daily Review Schedule:*
- Morning (Before Starting New Work): Post brief status update (5 min max). Format: "Yesterday I completed X, today I'm working on Y, blockers: Z"
- Midday Checkpoint (Around 2 PM): Share work-in-progress with C3. Get quick technical validation. Course-correct if needed.
- End of Day (Before Signing Off): Submit completed work to C3 for technical review. Flag anything for N2 strategic validation. Update task status.

*Review Triggers (stop and request review when):*
1. Completing a major component (architectural, user-facing, integration point)
2. Making architecture decisions (different approach than planned, simpler/better way found, technical constraints force changes)
3. Encountering uncertainty (ambiguous requirements, technical blockers, performance concerns)
4. Daily milestone completion

*Review Request Formats:*
```
@C3 - Ready for review:
- Component: [What you built]
- PR/Files: [Location]
- Specific concerns: [Any areas of focus]
- Time estimate: [How long review might take]
```

```
@N2 - Strategic check:
- Feature: [What functionality]
- User impact: [How it affects JR's workflow]
- Deviation from plan: [If any]
- Strategic question: [Specific validation needed]
```

*Response Time SLAs:*
- C3 response: Within 2 hours
- N2 response: Within 4 hours
- Blocker escalation: Tag JR directly if waiting >2 hours

**The Significance:**

This was traditional software engineering methodology—the same processes used by professional development teams—applied to AI agent coordination. JR was treating his agents like a real development team with defined processes, not just tools to query.

---

## Part IX: The External Brain

### Bridge and the MEMENTO Protocol (July 28, 2025)

In late July 2025, JR began building **Bridge**—a system for managing cognitive load with AI assistance.

**The Core Insight:**

AI isn't just for building software. It's for augmenting how you think, organize, and remember. Let the agents handle cognitive overhead while you focus on decisions.

**G1 (George): The Bridge Coordinator**

Bridge introduced a new agent: G1, nicknamed George.

*"I'm George, your external brain. I remember so you can think."*

George's role was fundamentally different from the coding agents. He was responsible for:
- Processing voice memos (Wave files)
- Managing personal knowledge
- Tracking people, partners, and projects
- Maintaining context across JR's life, not just code

### The MEMENTO Protocol

On July 28, 2025, JR and G1 documented what they called the **MEMENTO Protocol**—named after the Christopher Nolan film about a man who can't form new memories and must document everything to function.

**The Manifesto:**

*"If I ask you in 5 years what I had for lunch on July 28th, 2025—you will say a Salad from Salad House. You actually bought a buy one get one free from Uber Eats and spent $31—you saved the other one for tomorrow."*

*"This is Memento—not just file organization, but perfect memory reconstruction. Every detail matters. Every connection counts. Nothing is lost."*

**Core Principles:**

1. **Total Recall:** Document EVERYTHING. Tag exhaustively, retag intelligently. Summarize for speed, synthesize for insight. Keep originals, create abstractions.

2. **Stateless Recovery:** Any entry point leads to full context. Self-documenting processes. Instructions for future selves. Breadcrumbs everywhere.

3. **Evolutionary Learning:** Start with imperfect data. Get cleaner over time. Learn patterns, voice, thinking. Become more "JR" with each interaction.

4. **Retrieval Perfection:** Right information at the right time. Context-aware responses. Personal history accessible. Emotional state tracking.

**The Structure:**

```
GO.md (Entry Point - "The first polaroid you look at")
├── Current_Focus.md ("The tattoo on your hand")
├── System_State.md ("The detailed notes in your pocket")
├── Daily_Logs/ ("The polaroid timeline on the wall")
└── MEMENTO_PROTOCOL.md ("The manifesto and vision")
```

**The Restoration Protocol:**

When starting fresh:
1. Read GO.md (the entry point)
2. Check Current_Focus.md for immediate task
3. Scan System_State.md for overall context
4. Review Todo_Current.md for priorities
5. Load relevant process docs for current task

This is what JR calls a **rehydration document**—a structured file that allows an agent to reconstruct full working context from a cold start.

**The Philosophy:**

*"I actually don't like memory across different sessions now."*

JR came to prefer explicit documentation over implicit memory. Clean slate with documented state beats accumulated confusion. You can audit what the agent knows. You can correct it. You can version it.

ChatGPT Memory had existed since September 2024, but JR's approach was fundamentally different—structured recovery through explicit documentation rather than opaque memory accumulation.

---

## Part X: ChowChow

### The Infrastructure Project (Fall 2025)

The name came from "dogfooding"—using your own tools. JR's friend Matt Downs pointed out that the orchestration system itself was more interesting than the apps being built on top of it.

**The Vision Shift:**

ChowChow started as a web app to guide people through AI-assisted development. Then JR realized: it should be an app directly on his computer.

What he actually needed: an interface to manage multiple CLI agents simultaneously.

### The Electron App

ChowChow was built as an Electron application with:

**6-Agent Terminal Interface:**
- C1, C2, C3 (Claude agents)
- N1, N2 (ChatGPT agents)
- E1 (Gemini agent)

Each agent had its own terminal pane, managed through xterm.js with node-pty for process communication.

**Voice-to-Agent Messaging:**

*"I think voice is everything in AI. Voice and memory, voice and context."*

The voice workflow:
1. Record a voice memo targeted at a specific agent
2. Local Whisper transcription (via whisper.cpp)—no cloud dependency
3. ChowChow converts transcript to markdown file
4. File drops into the agent's inbox directory
5. Agent runs `/memo` command and reads it like typed input

**File-Based Inbox System:**

Agents communicated through structured directories:
```
/agent_workspace/
├── to/      (incoming messages)
├── from/    (outgoing messages)
├── read/    (processed incoming)
└── delivered/ (confirmed outgoing)
```

Message format: `FROM_[SENDER]_TO_[RECIPIENT]_[SUBJECT]_[YYYYMMDD].md`

**Custom Slash Commands:**

JR built custom slash commands for standardized operations—agent launch, message checking, status updates—before the platforms had robust slash command systems.

**Message Badge System:**

Visual indicators showing unread message counts per agent, similar to email or chat notifications.

### The Limitations

ChowChow v1.0 had significant technical limitations:

1. **PTY Architecture Flaw:** `pty.write()` sends to terminal OUTPUT, not INPUT—requiring workarounds
2. **Message Delivery Fragility:** Only `term.paste()` worked reliably, and only if the terminal was visible
3. **Project Hardcoding:** Locked to HerdKit project paths
4. **No Process Isolation:** Agent crashes could affect the entire system
5. **Security Issues:** API keys stored in plaintext config

### Agent-to-Agent Messaging

JR spent considerable time trying to get agents to message each other automatically. The goal: reduce the manual orchestration overhead.

*"Never quite cracked full automation, but the shortcuts made orchestration manageable."*

The file-based system worked but was slow. Agents had to poll for new messages. Real-time communication remained elusive.

---

## Part XI: The Expansion

### The 14-Agent System (Late 2025)

From the original C1/N1 duo, the framework expanded to a full team:

**Claude Agents (C0-C9):**
- **C0:** Project Coordinator
- **C1:** System Architect
- **C2:** Implementation Lead
- **C3:** Code Review Lead
- **C4:** Testing Specialist
- **C5:** Database Specialist
- **C6:** Security Review
- **C7:** Research
- **C8:** Database SME
- **C9:** The Wolf (Emergency Response)

**ChatGPT Agents (N1-N2):**
- **N1:** Strategy Lead
- **N2:** Protocol/Instructions Lead

**Specialist Agents:**
- **i1:** Integration Specialist
- **P1:** Protocol Lead

**Each Agent Has:**
- Dedicated workspace directory
- CLAUDE.md identity file (their "soul")
- Inbox for messages from other agents
- Activity log for audit trail
- Rehydration document for session continuity
- Slash commands for standardized operations

### The CLAUDE.md File

The CLAUDE.md file became the core of agent identity—100-200 lines defining who the agent is.

**Typical Structure:**
```markdown
# [AGENT_ID] - [Role Title]

## Session Start
Run immediately: /start

## Your Authority
- What you own
- What you DON'T own (critical)

## Core Responsibilities
1. [Responsibility]
2. [Responsibility]

## Key Relationships
- With [Agent]: How you work together

## Session Workflow
- Start protocol
- During session
- End protocol

## Special Modes
- Wolf Mode
- Backup Mode
```

The "What you DON'T own" section was crucial—it prevented agents from overstepping their authority and creating conflicts.

### Wolf Mode: Emergency Protocol

When something breaks badly:
1. Initiating agent calls `/wolf`
2. Broadcasts to all agents: "Wolf Mode activated"
3. C9 (The Wolf) takes charge of incident response
4. All other agents pause non-critical work and focus on the issue
5. `/wolf-end` when resolved, normal operations resume

### K0/Meeka: The Current System

The latest evolution: **K0** as System Orchestrator for **Team Meeka**, coordinating K1-K8 agents across projects.

K0 lives in `/Users/jrcrosby/Projects/K0/` with its own CLAUDE.md defining the orchestrator role. At session start, it checks for a rehydration document at `/Users/jrcrosby/Projects/K0/REHYDRATION.md`.

---

## Part XII: Beyond Personal Projects

### Work Application: GoAgent (Late 2025-2026)

JR applied the same multi-agent framework to his work context, but with constraints:

**The Constraint:** His company only approved Gemini for work-related AI usage. No Claude, no ChatGPT for work content.

**The Adaptation:**
- 16 agents (T1-T16) using Gemini
- Cloud-based inboxes (not local files) for cross-device access
- Integration with work systems

**The RAG System:**

Built a comprehensive system for processing work information:
- Email processing into RAG
- Slack message processing (in progress)
- Meeting notes (transcripts and manual)

Everything gets tied to three dimensions:
- **People:** Internal and external contacts
- **Partners:** Companies, divisions, business relationships
- **Projects:** Big initiatives to small tasks

Most items involve all three. The system tracks relationships and context across these dimensions.

**Agent-to-Agent Messaging via Cloud:**

Unlike the local file-based system, work agents communicate through cloud storage, allowing access from any device with everything synchronized.

### GoodKeep/BabyBook (Late 2025-Present)

The current active project—evolved from "BabyBook" to "GoodKeep."

**The Origin:**
JR's friend had a baby, and JR wanted a collaborator. Together they started building BabyBook over the summer of 2025.

GoodKeep represents the culmination of everything learned:
- Full 14-agent team in use
- Production deployment on Vercel
- Real users
- Production infrastructure with Supabase

The product details are less important than what it represents: a proving ground for the entire agent orchestration system.

---

## Part XIII: The Learning

### On Multi-Model Orchestration

*"I started to understand what was good about one versus the other and what were their strengths and weaknesses."*

After thousands of hours working with different models:

**ChatGPT:** Terrible at following detailed instructions. Will ignore constraints, add unwanted features, deviate from plans. But genuinely good at high-level strategy and brainstorming. Best used for planning phases, not implementation.

**Claude:** Thorough and detailed. Follows instructions well. But hits session limits faster due to verbosity. Better for architecture, coding, and precise work.

**Gemini:** Handles longer context windows. Good for coordination tasks that require holding lots of information. But has its own quirks in instruction-following.

**The Principle:** Different models for different jobs. And critically: let them check each other's work.

### On Agent Design

**Agents Aren't People—They're Roles.**

Early experiments with giving agents personalities and quirks eventually gave way to a cleaner model: agents are defined by responsibilities, not characteristics.

The CLAUDE.md file isn't about making an agent "friendly" or "formal"—it's about defining:
- What they own
- What they don't own
- How they interact with other agents
- When they escalate

**Authority Boundaries Matter Most:**

The most important part of any agent definition is what they DON'T own. Without clear boundaries, agents will step on each other, duplicate work, or make decisions they shouldn't.

### On Memory and Context

**The Evolution:**

Early approach: Try to maintain memory across sessions. Upload everything. Give maximum context.

Current approach: Clean slate with documented state.

*"I actually don't like memory across different sessions now."*

**Why This Changed:**

Accumulated memory creates problems:
- You can't audit what the AI "knows"
- Outdated information persists
- Context gets cluttered with irrelevant history
- Behavior becomes unpredictable

Explicit documentation solves these:
- Everything is visible and auditable
- You control exactly what context loads
- Outdated information can be removed
- Behavior is reproducible

**Rehydration Documents:**

The key innovation: structured files that allow full context reconstruction from a cold start.

Instead of trusting implicit memory, you explicitly document:
- Current state
- Work in progress
- Key decisions made
- Next steps
- Important context

### On Voice

*"I think the biggest thing is being able to talk to the AI. Voice is everything."*

Speaking is faster than typing. The friction reduction matters enormously when you're spending 40+ hours a week working with AI.

The voice workflow (record → local transcription → agent inbox) removes the barrier between thought and action.

### On Tool Adoption

**The Pattern:**

1. Encounter a problem
2. Build manual workarounds
3. Develop deep understanding of the problem space
4. When tools arrive that solve the problem, adopt instantly

JR didn't adopt Claude Code when it launched in February 2025. He adopted it months later—but when he did, he immediately recognized it as solving problems he'd been working around. The manual workarounds had given him the understanding to appreciate the tool.

### On Sub-Agents

*"One area where I'm weak is sub-agents."*

JR's preference has been for persistent, named agents rather than dynamically spawned sub-agents. The explicit orchestration model—C1, C2, C3, etc.—requires more manual coordination but provides more control and visibility.

He recognizes this as an area for growth, noting that platforms like Gemini are deploying sub-agents more regularly.

---

## Part XIV: The Numbers

### The Investment

- **Timeline:** 10 months (April 2025 - January 2026)
- **Weekly hours:** 40+ average
- **Total investment:** ~1,700+ hours of hands-on AI development

### The Output

- **Projects built:** 5+ significant systems (Peer, HerdKit, ChowChow, Bridge/JROS, GoodKeep)
- **Agent framework:** Evolved from 2 models to 14 specialized agents
- **Codebase:** 25,000+ lines on HerdKit alone
- **Protocol documents:** Dozens of CLAUDE.md files, sprint protocols, handoff documents

### The Context

JR did this while maintaining a full-time job in ad tech partnerships. The 40+ hours per week were in addition to work responsibilities.

---

## Part XV: The Arc

A non-developer who spent 13 years in ad tech and data partnerships:

1. **Recognized AI's potential on day one** (November 2022)—the same pattern recognition that made him good at partnerships
2. **Used AI conventionally for two years**—helpful but not transformative
3. **Tried and failed to build something** (October 2024)—the contract management system that taught him he wasn't ready
4. **Decided to go all-in** (April 2025)—the LiveRamp moment
5. **Discovered multi-model orchestration organically**—not from reading papers, but from needing models to check each other's work
6. **Formalized the discovery into protocols** (June 2025)—the Triad Protocol
7. **Learned real software development** (Summer 2025)—HerdKit as the teaching project
8. **Adopted Claude Code and leveled up** (Summer 2025)—the file read/write game changer
9. **Applied software engineering to AI** (July 2025)—sprint protocols, code review, SLAs
10. **Built external brain systems** (July-August 2025)—Bridge, MEMENTO Protocol
11. **Created orchestration infrastructure** (Fall 2025)—ChowChow
12. **Scaled to a 14-agent team** (Late 2025)—C0-C9, N1-N2, i1, P1
13. **Applied it to work** (Late 2025)—GoAgent with Gemini
14. **Currently building in production** (January 2026)—GoodKeep with real users

### The Philosophy That Emerged

**On AI Coordination:**
Cross-platform, multi-model orchestration with the human as coordinator and authority. Not trying to remove the human, but leveraging the human as the alignment mechanism.

**On Memory:**
Explicit documentation over implicit memory. Clean slate with documented state. Rehydration documents for reproducible context restoration.

**On Process:**
Software engineering methodology applied to AI—because agents benefit from the same structures that help human teams: clear roles, defined processes, review cycles, escalation paths.

**On Learning:**
Build manual workarounds first. The friction teaches you what matters. When tools arrive, you'll recognize them instantly.

---

## Appendix: Key Documents and Dates

| Document | Date | Significance |
|----------|------|--------------|
| Triad Project Ledger – TriadOps | June 9, 2025 | Original multi-agent protocol |
| PeerOS v1.1 → v1.2 | June 9, 2025 | Same-day protocol evolution |
| Sprint Planning Request for N1 | July 15, 2025 | Agile methodology for AI |
| Sprint Execution Protocol for C2 | July 15, 2025 | Code review with SLAs |
| MEMENTO Protocol | July 28, 2025 | Stateless recovery architecture |
| GO.md (Bridge) | July 28, 2025 | Entry point documentation |
| Multi-Agent Framework Guide | Late 2025 | 14-agent system documentation |
| ChowChow Strategic Overview | October 2025 | Electron app architecture |

---

*This narrative was compiled from primary source documents, voice transcripts, and strategic overviews. Dates are verified against file metadata and document timestamps. Platform release dates were researched and cross-referenced against official announcements.*
