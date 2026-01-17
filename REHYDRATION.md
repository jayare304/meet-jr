# Rehydration - Meet JR

## Domain
**jrcrosby.info**

## Current State
Project scaffolding complete. Landing page and resume exist. Chat mode not yet built.

## What Exists
- `src/index.html` - Landing page with two CTAs (working)
- `src/assets/jr-resume.html` - HTML resume in Claude colors (working)
- `context/system-prompt.md` - Claude personality for chat mode (drafted)
- `context/jr-comprehensive-coding-narrative.md` - Full journey (~6,500 words)
- `context/jr-coding-journey.md` - Condensed journey (~3,500 words)

## What's Next
1. **Chat app** - Build `src/chat/` with chat interface
2. **API endpoint** - Create `api/chat.js` for Claude conversations
3. **PDF resume** - Generate from HTML for download
4. **Voice input** - Add Web Speech API to chat mode
5. **Deploy** - Get live URL for Anthropic application
6. **GitHub repo** - Create and push

## Context
This is part of JR's Anthropic application (Solutions Architect, Applied AI). The goal is to ship a live demo that shows he can build with Claude, not just talk about it.

A1 (web Claude) handles strategy. A2 (Claude Code) handles files. JR coordinates.

## Last Session
- Created project structure
- Wrote CLAUDE.md (evergreen)
- Built landing page
- Updated resume to Claude colors
- Drafted system prompt for chat mode
- Renamed project from jr-adventure to meet-jr
- Removed all "adventure" terminology
