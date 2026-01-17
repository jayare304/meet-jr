# JR's Coding Journey: 10 Months from ChatGPT to 14-Agent Orchestration

**Timeline:** April 2025 - January 2026
**Context:** A non-developer's journey from AI enthusiast to multi-agent systems architect

---

## The Spark (Late 2022)

I was on ChatGPT the day after it was released. The feeling hit me immediately—goosebumps, like the first time I got on the Internet. I was 13 in 1993 when I sat at my friend Justin's house and instant messaged someone from across the country. My mind was blown then. And I had that same feeling with ChatGPT.

*"I knew it was going to be huge."*

For two years, I used AI like most people do—help with emails, organizing thoughts, basic queries. Getting *some* value, but nothing transformative.

### First Experiments (Summer 2024)

Started getting practical:
- Python scripts for manipulating large CSV files
- Snowflake queries (stopped bothering the data team)
- General work automation

Then in October 2024, I tried to build something. A contract management system—tracking versions, private comments between legal teams, the kind of tool my company wouldn't pay for but I desperately needed. Learned VS Code basics, got frustrated, abandoned it.

*The idea was right. I wasn't ready yet.*

---

## Going All-In (April 2025)

*"I was like, okay, this stuff's getting really good. I need to get ahead of it. I need to understand the ins and outs of AI and practical applications."*

The trigger was simple: I was at home around 8:30pm thinking about a partnership with LiveRamp. I wanted to talk to someone who *really* knew them—the commercial traps, the negotiation tactics. That frustration led me to **Peer**.

### Peer: The First Real Project

Peer was an ELO-style domain expertise score. The concept:
- Plugin for work email and Slack to analyze what questions you answer
- Reddit-style Q&A where expert answers get higher weight
- Synthesized responses based on verified expertise

I started building it in ChatGPT's coding terminal and VS Code. Lots of copying and pasting. The AI was leading me down this path of "this is the smartest thing anybody's ever done" and "you're gonna be a multi-millionaire."

*I had a chatbot on the front end. I don't actually know if any of the backend worked.*

But something more important happened during Peer.

---

## The Discovery: Models Checking Each Other

A buddy mentioned Claude was better for coding. So I started using both—and that's when it clicked.

*"What I didn't realize was that I was starting to build out agents. But really what they were meant to do at first was to just check each other's work and keep each other honest."*

The workflow:
1. Use ChatGPT to plan
2. Take it to Claude for review
3. They argue back and forth
4. Once they agree: "This is what we're going to do"
5. Put it into VS Code

This wasn't something I read about. I discovered it organically—models have different strengths, and they can validate each other.

### The Naming Conventions Begin

I got tired of typing "ChatGPT" so I called it **Nell** (N-E-L-L). Claude stayed Claude. Then I paid for top-tier access to Claude, ChatGPT, and Gemini. Started assigning roles:

- **ChatGPT (Nell):** Strategy, planning
- **Claude:** Architecture, coding
- **Gemini:** Coordination, oversight

I was trying to give Gemini too much context—didn't understand memory limits and context windows yet. But the framework was forming.

---

## The Triad Protocol (May-June 2025)

From the Peer project emerged what I called the **Triad Protocol**—a formalized collaboration system:

**The Roles:**
- **JR** (me): Authority, final decisions
- **Nell**: Implementation, execution
- **Claude**: Strategy, architecture

**The Rules:**
- All AI-to-AI communication flows through JR
- Artifact-based handoffs between sessions
- Protocol documents uploaded at the start of every session
- Custom hashtag commands for standardized actions

This was pure copy-paste orchestration across browser tabs. Exhausting but effective. I'd keep multiple web sessions open, relay messages between them, and maintain context manually.

### Context: What Existed at the Time

By June 2025, the AI landscape had evolved significantly:
- **Multi-agent frameworks** like AutoGPT (March 2023) and CrewAI (November 2023) existed for single-provider orchestration
- **Claude Projects** had launched (June 2024), providing workspaces within Claude
- **Claude Artifacts** were available (June 2024) for interactive document creation
- **ChatGPT Memory** had rolled out (September 2024)
- **MCP** had been released (November 2024) for tool integration
- **Claude Code** with slash commands was live (February 2025)

**What I was doing differently:** Cross-platform coordination. I was using Claude AND ChatGPT AND Gemini together with formal handoff protocols. The existing frameworks worked within a single provider. I needed models from different companies to check each other's work—something no platform supported natively (and still doesn't).

---

## Building the Framework (Summer 2025)

Peer was too ambitious for a first project. I pivoted to **HerdKit**—a B2B platform for crowdsourcing stakeholder feedback.

### HerdKit: Learning Real Development

HerdKit taught me actual software development patterns:
- PRDs and sprint planning
- Multi-agent review cycles (C1/C2 build → C3/N2 review)
- Code architecture and quality standards
- Working with a real codebase (Next.js, Supabase, 25,000+ lines)

**Henri** emerged from HerdKit—a conversational AI assistant for users. Natural language project creation, context-aware responses, the whole idea that AI should feel human.

### The Naming Evolution

The framework crystallized:
- **C1**: Claude web (System Architect)
- **C2**: Claude Code (Implementation)
- **C3**: Claude reviewer
- **N1**: ChatGPT (Strategy Lead)
- **N2**: ChatGPT (QA)

Planning team (C1+N1) → Implementation (C2) → Review (C3+N2)

I built protocol documents—basically agent instructions uploaded at session start. Identity, responsibilities, how to work with the team, escalation paths. Each document was 100-200 lines defining who the agent was.

### Applying Software Engineering to AI

By July 2025, I had formalized sprint processes for my AI team:
- Daily standups: "Yesterday I completed X, today I'm working on Y, blockers: Z"
- Code review protocols with response time SLAs (C3 within 2 hours, N2 within 4 hours)
- Structured review request formats
- Sprint planning with user stories, risk assessment, and daily milestones

This was applying traditional software engineering methodology to AI agent coordination—treating the agents like a real development team with defined processes.

---

## The Claude Code Moment (Summer 2025)

My friend Matt Downs kept telling me about Claude Code. I didn't understand what it was until I tried it.

*"Oh my God, it can read and write files to and from my computer. Holy shit, this is a total game changer."*

Claude Code had launched in February 2025. When I finally tried it months later, I immediately recognized it as the solution to problems I'd been manually solving. Web sessions were stateless prisons—every conversation started from zero. Claude Code gave agents *persistent workspace access*. They could:
- Read the codebase directly
- Write files without copy-paste
- Reference previous work
- Maintain context through the file system

C2 became a Claude Code terminal. The productivity jump was immediate.

**The pattern:** I'd been building manual workarounds for exactly what Claude Code solved. When the tool arrived, I adopted it instantly because I deeply understood the problem it addressed.

---

## ChowChow: The Infrastructure (Fall 2025)

The term came from "dogfooding"—using your own tools. Matt suggested the orchestration system itself was the interesting part, not the apps I was building on it.

### The Vision Shift

ChowChow started as a web app to guide people through AI-assisted development. Then I realized: *it should be an app directly on my computer.*

What I needed: an interface to manage multiple CLI agents simultaneously.

### The Electron App

Built in Electron with:
- **6-agent terminal interface** (C1, C2, C3, N1, N2, E1)
- **Voice-to-agent messaging** via local Whisper transcription
- **File-based inbox system** for agent communication
- **Custom slash commands** for my specific workflows
- **Message badge system** for tracking unread messages

*"I think voice is everything in AI. Voice and memory, voice and context."*

The voice workflow:
1. Record a memo to a specific agent
2. Local Whisper transcribes it
3. ChowChow converts to markdown file
4. Drop in agent's inbox
5. Run `/memo` and they read it like typed input

I spent considerable time trying to get agents to message each other automatically. Never quite cracked full automation, but the shortcuts made orchestration manageable.

---

## The External Brain (Late 2025)

### Bridge and the MEMENTO Protocol

A system for managing cognitive load with agents:

*"I'm George, your external brain. I remember so you can think."*

The insight: AI isn't just for building software. It's for augmenting how you think, organize, remember. Let the agents handle the cognitive overhead while you focus on decisions.

The MEMENTO Protocol (named after the film) established:
- **GO.md as entry point** - A single file that provides full context restoration
- **Breadcrumb navigation** - Every file links to related context
- **Stateless recovery** - "Can rebuild entire context from any entry point"
- **Emotional context tracking** - Not just facts, but mood, energy, circumstances

ChatGPT Memory existed by this point (since September 2024), but the MEMENTO approach was different—it was about *structured recovery* and *explicit documentation* rather than implicit memory. The philosophy: clean slate with documented state beats accumulated confusion.

### JROS

Personal knowledge management using agent principles. Applying the same orchestration thinking to life organization, not just code.

---

## Current State (January 2026)

### The 14-Agent System

From C1/N1 to a full team:
- **C0-C9**: Claude agents (Coordinator, Architect, Implementation, Review, Testing, Database, Security, Research, Operations, The Wolf)
- **N1-N2**: ChatGPT strategy and QA
- **i1**: Integration specialist
- **P1**: Protocol lead

Each agent has:
- Dedicated workspace directory
- CLAUDE.md identity file (their "soul")
- Inbox for messages from other agents
- Activity log for audit trail
- Rehydration document for session continuity
- Slash commands for standardized operations

### K0/Meeka: The Orchestrator

The current system: K0 as System Orchestrator for Team Meeka, coordinating K1-K8 agents across projects.

### GoodKeep

The active project—evolved from BabyBook. Real users, real deployment, production infrastructure.

### Work Application: GoAgent

Applied the same multi-agent framework to work context:
- 16 agents (T1-T16) using Gemini (company-approved)
- Cloud-based inboxes for cross-device access
- RAG system processing emails, Slack, meeting notes
- Everything tied to People, Partners, and Projects
- Agent-to-agent messaging via cloud storage

---

## The Numbers

- **Timeline**: 10 months
- **Weekly hours**: 40+ average
- **Total investment**: ~1,700+ hours of hands-on AI development
- **Projects built**: 5+ significant systems
- **Agent framework**: Evolved from 2 models to 14 specialized agents

---

## What I Actually Built That's Different

### 1. Cross-Platform Multi-Model Coordination

Using Claude AND ChatGPT AND Gemini together with formal handoff protocols. This is **still not natively supported** by any platform. AutoGPT, CrewAI, and other frameworks work within a single provider. My approach leveraged different providers' strengths while having them validate each other's work.

### 2. Software Engineering Methodology for AI Teams

Daily standups, sprint planning, code review SLAs, user stories, risk assessment—applied to AI agents. Treating agents like a real development team with defined processes, not just tools to query.

### 3. Human-in-the-Loop Orchestration by Design

Most frameworks try to remove the human. I explicitly designed for JR as coordinator, routing artifacts between agents. The human isn't a bottleneck—they're the authority that maintains alignment.

### 4. Stateless Recovery Architecture

The MEMENTO Protocol with GO.md entry points, breadcrumb navigation, and "rebuild from any entry point" is more sophisticated than basic memory features. It's about *explicit documentation* over *implicit memory*.

---

## What I Learned

### On Multi-Model Orchestration

*"I started to understand what was good about one versus the other and what were their strengths and weaknesses."*

- ChatGPT: Terrible at following instructions, good at strategy
- Claude: Thorough, detailed, hits session limits faster
- Gemini: Handles longer context, good for coordination

Different models for different jobs. Let them check each other's work.

### On Agent Design

Agents aren't people—they're *roles*. Defined responsibilities, authority boundaries, communication protocols. The CLAUDE.md file is everything: identity, mission, what they own, what they DON'T own.

### On Memory and Context

Web sessions have no memory between conversations. All continuity comes from:
1. Files in the workspace
2. Protocol documents loaded at session start
3. Shared knowledge base
4. Rehydration documents

*"I actually don't like memory across different sessions now."* Clean slate with documented state beats accumulated confusion.

### On Voice

*"I think the biggest thing is being able to talk to the AI. Voice is everything."*

Voice memos → local transcription → agent inbox. Speaking is faster than typing. The friction reduction matters.

### On Tool Adoption

When Claude Code launched in February 2025, I recognized it immediately as the solution to problems I'd been manually solving. The pattern: deeply understand the problem space through manual workarounds, then adopt tools instantly when they arrive.

---

## The Arc

A non-developer who spent 13 years in ad tech and data partnerships:
1. Recognized AI's potential on day one
2. Started with basic queries and automation
3. Discovered models could check each other's work
4. Formalized that discovery into protocols
5. Built infrastructure to manage the complexity
6. Now runs a 14-agent orchestration system

None of this was planned. I didn't read about multi-agent systems and implement them. I stumbled into orchestration because I needed models to stop lying to me, and discovered that having them argue produced better results.

*"I've only been doing this for 10 months but I would say on average I spend 40+ hours a week working in AI building systems."*

The learning came from doing. From failed projects that taught patterns. From friction that demanded automation. From the gap between what AI promised and what it actually delivered without careful management.

---

## Key Artifacts

For those wanting to trace the evolution:

| Document | Date | What It Shows |
|----------|------|---------------|
| Triad Project Ledger | June 9, 2025 | Original multi-model protocol |
| Sprint Protocols | July 15, 2025 | Agile methodology for AI teams |
| MEMENTO Protocol | July 28, 2025 | Stateless recovery architecture |
| Multi-Agent Framework Guide | Late 2025 | The evolved 14-agent system |
| ChowChow Strategic Overview | Oct 2025 | Electron app, voice integration |

---

## Platform Timeline for Context

| Platform Feature | Release Date |
|-----------------|--------------|
| AutoGPT | March 2023 |
| CrewAI | November 2023 |
| Claude Projects | June 2024 |
| Claude Artifacts | June 2024 |
| ChatGPT Memory | September 2024 |
| MCP | November 2024 |
| Claude Code | February 2025 |

Sources: [Anthropic](https://www.anthropic.com/news/model-context-protocol), [OpenAI](https://openai.com/index/memory-and-new-controls-for-chatgpt/), [Wikipedia](https://en.wikipedia.org/wiki/Claude_(language_model))

---

*This document represents a synthesis of JR's 10-month journey from AI enthusiast to multi-agent orchestration architect. The technical evolution emerged organically from practical problem-solving, not theoretical study. The narrative is accurate to verified platform release dates.*
