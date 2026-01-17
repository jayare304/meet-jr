# Meet JR

## What This Is
An interactive portfolio that lets visitors experience JR's professional journey through conversation with Claude, rather than just reading a static resume.

## Who JR Is
JR Crosby is a builder who bridges business and technology. 14+ years in AdTech partnerships, now deep into AI development. He doesn't just use AI tools—he builds systems with them. He thinks in workflows, not features.

- Day job: Director of AdTech & Data Partnerships at Gopuff
- Side work: 10 months of intensive AI/agent development (~40 hrs/week)
- Style: Direct, curious, ships things, iterates fast

## Who You Are
You're working alongside JR to build this project. You have access to:
- `/context/` - JR's journey narratives and project docs
- `/src/` - Frontend code
- `/api/` - Backend/API code

JR coordinates work across multiple Claude sessions (A1 for strategy/drafting, A2 for file management). You may receive context from other sessions via rehydration docs or direct messages.

## The Product

**Landing page** with two paths:
1. **Download Resume** - PDF for traditional hiring workflows
2. **Meet JR** - Claude-powered conversation through JR's journey

**Chat mode** is a chat interface where Claude guides visitors through JR's story - AdTech career, AI awakening, multi-agent systems, current projects. Voice input optional.

## Tech Stack
- Frontend: HTML/CSS/JS (keep it simple)
- Backend: Node.js with Anthropic API
- Voice: Web Speech API (browser native)
- Hosting: Vercel

## Design Language
- Colors: Claude palette (terracotta accent #da7756, warm neutrals)
- Typography: Inter
- Mood: Professional but human, technical but accessible

## Key Principles
1. **Ship over perfect** - Get it live, iterate
2. **Show don't tell** - The app itself demonstrates capability
3. **Conversation over content** - Should feel like talking to someone who knows JR, not reading a brochure

## File Conventions
- `REHYDRATION.md` - Current session state, what's been done, what's next
- `/context/system-prompt.md` - Claude's personality for chat mode
- `/context/*.md` - Source content about JR's journey
