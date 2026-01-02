# OpenTools Hub - Project Ideas

Project ideas and feature requests for OpenTools Hub. See [ABOUT.md](ABOUT.md) for more info.

## Open Questions

- [ ] Figure out how this project relates to [vibe-coding-guide](https://github.com/tmad4000/vibe-coding-guide)

---

## Vibe UI Hints

- [ ] Medium — *Unclaimed*

**Summary**

A Mac app that provides gentle visual hints to guide users through UI interactions. When you ask an AI assistant (ChatGPT, Claude) or search Google for "how to do X" and get step-by-step instructions, this app overlays subtle highlights on your screen showing exactly where to click.

**Core Features**

- Screen Overlay Hints: Gentle visual indicators (highlights, arrows) that say "click here" for each step
- Accessibility API Integration: Uses macOS Accessibility APIs to identify clickable elements
- AI Instruction Parsing: Takes step-by-step instructions and maps them to UI elements on screen

**Future Enhancements**

- Chrome Extension: Extend to web apps for more precise element targeting within browsers
- Auto-Click Mode: "Just do it for me" - automatically execute the clicks/actions
- Multi-App Support: Works across any macOS application

**Technical Considerations**

- Look at how [HomeRow](https://www.homerow.app/) implements keyboard-driven UI navigation for inspiration
- macOS Accessibility APIs for element detection
- Overlay window that sits above all other windows
- Potentially use Vision/OCR for apps that don't expose accessibility info

**Use Cases**

1. Following tutorial steps without switching between windows
2. Helping less technical users navigate unfamiliar apps
3. Automated workflows that are too simple for full scripting
4. Accessibility aid for users who need visual guidance

---

## Open Contexts

- [ ] Medium — *Unclaimed*

**Summary**

An open-source alternative to [Contexts.co](https://contexts.co) — a fast window switcher for macOS. The key differentiator: **sort by recency, not just alphabetically**, even when filtering windows within a specific application.

**Core Features**

- Window Switcher: Quick keyboard-driven window switching (like Contexts)
- Recency Sorting: Sort windows by most recently used, not alphabetically
- Per-App Filtering: Filter to show only windows from a specific app, still sorted by recency
- Fuzzy Search: Type to filter windows by title or app name

**Why Open Source?**

Contexts.co is great but:
- Only sorts alphabetically within apps
- Closed source, can't add features
- The window switcher is the main value — focus on doing that one thing well

**Technical Considerations**

- macOS Accessibility APIs for window enumeration
- Track window focus timestamps for recency sorting
- Global hotkey activation
- Fast, native UI (Swift/AppKit or SwiftUI)

---

## Smart Backpack Inventory

- [ ] Small — *Unclaimed*

**Summary**

An app to help you track what's in your backpack and verify contents before leaving. Useful for ensuring you have specific items (like gloves on a cold day or specific gear for a hobby) without manual checking.

**Core Features**

- Daily Checklist: "I want to add X" or "remove Y" for today
- Context Awareness: Suggest items based on weather or calendar events
- Simple UI: Quick toggle for item presence

---

## Global Shortcut Registry

- [ ] Small — *Unclaimed*

**Summary**

A central place to keep track of all your keyboard shortcuts across different applications so you don't accidentally overwrite them or create conflicts.

---

## Vibe Matcher Social Network

- [ ] Large — *Unclaimed*

**Summary**

A generalized matching app (dating or friendship) that uses machine learning to quantify and match people based on "vibes" and deep compatibility factors that are often hard to classify.

**Core Features**

- Robust Factor Quantization: Moving beyond surface interests to deeper compatibility
- ML-driven Matching: Using algorithms to find people who actually vibe well
- Generalized Networking: Useful for finding friends, collaborators, or partners

---

## Learning Optimization Suite

- [ ] Large — *Unclaimed*

**Summary**

A comprehensive "learning suite" that moves away from traditional courses and focuses on personal knowledge management, reflection, and adaptive learning.

**Core Features**

- Easy Reflection: Streamlined notes and logs for active reflection
- Adaptive Placement: Quick 3-question quizzes to determine your level in a subject
- Resource Aggregation: Pulls and compares free courses (e.g., MIT OpenCourseWare)
- Spaced Repetition: Integrated active recall tools
- Learning Export: Export your "current understanding" to talk to other tools/people

---

## Hands-Free Biker Assistant

- [ ] Medium — *Unclaimed*

**Summary**

A voice-integrated directions and assistant app specifically for bikers whose hands are full and eyes need to be on the road.

**Core Features**

- Voice-First Interface: Ask "what's going on?" or get directions via voice
- Specialized Biking Data: Directions optimized for safety and bike paths

---

## Sus Food Scanner

- [ ] Medium — *Unclaimed*

**Summary**

A classifier app that allows you to scan food that looks "sus" to check if it might be spoiled.

---

## Crowd-Sourced Life Guide

- [ ] Medium — *Unclaimed*

**Summary**

A platform for "nuggets of wisdom" on adulting tasks like taxes, applying to programs, or general life advice.

**Core Features**

- Crowdsourced Advice: Similar to specialized forums but structured for quick lookup
- Topic Categories: Taxes, healthcare, education, etc.

---

## Real-Feel Temperature Guide

- [ ] Small — *Unclaimed*

**Summary**

An app that tells you how the temperature *actually* feels, taking into account wind, humidity, and providing intuitive descriptions for people who don't have a good mental map of Celsius/Fahrenheit.

---

## UI Shortcut Coach & Suggester

- [ ] Medium — *Unclaimed*

**Summary**

An intelligent assistant that watches your screen and identifies when you're "doing things the dumb way" (e.g., clicking through menus for actions that have shortcuts). It provides gentle, contextual reminders to use optimal keyboard shortcuts.

**Core Features**

- Screen Interaction Monitoring: Identifies repetitive mouse-based workflows
- Contextual Nudges: Real-time suggestions for shortcuts you could have used
- Web & Desktop Support: Works across browsers and native applications

---

## Intelligent Wait-Aware Scheduler

- [ ] Medium — *Unclaimed*

**Summary**

A task scheduler that accounts for tasks that require "waiting time" (e.g., waiting for a build, a response, or a delivery) and automatically adjusts your plan.

**Core Features**

- Auto-Planner: Intelligent scheduling based on due dates and dependencies
- Variable Input Levels: From quick task entry to detailed scheduling

---

## Cultural Context & Slang Translator

- [ ] Medium — *Unclaimed*

**Summary**

A translator for different philosophical frameworks, cultural spheres, and generational slang.

**Potential Domains**

- Generational: Gen Alpha, Gen Z, Millennial slang
- Academic/Professional: Industry-specific terminology (EA, Tech, Rationalist)
- Platform-Specific: Discord, Reddit, or Message-specific terminology
- Personal/Group: Friend group inside jokes or personal notation

---

## Karabiner Disabler

- [ ] Small — *Unclaimed*

**Summary**

A CLI tool or utility to temporarily disable Karabiner-Elements for a set amount of time or until toggled back on with a command.

**Core Features**

- Timed Disable: `disable-karabiner --duration 10m`
- Toggle Mode: Quickly enable/disable via command or global hotkey
- Status Indicator: Visual or audio feedback when Karabiner is disabled

---

## Minimalist CSV Editor

- [ ] Small — *Unclaimed*

**Summary**

A lightweight, high-performance CSV editor focused on speed and keyboard-driven workflows.

**Core Features**

- Instant-On: No splash screens or heavy UI, opens large files instantly
- Keyboard-Centric: Vim-like or spreadsheet-optimized navigation
- Clean Interface: Focus on data without unnecessary formatting bloat

---

## Google Workspace Shortcut Enhancer

- [ ] Small — *Unclaimed*

**Summary**

A tool or extension to add missing productivity shortcuts to Google Sheets and other Google products, including custom "Fill Color" shortcuts and global remapping.

**Core Features**

- Fill Color Shortcuts: Assign specific keys to your most-used cell highlight colors
- Advanced Remapping: Overwrite default Google shortcuts or add new ones
- Sheet-Specific Macros: Trigger complex actions with simple key combinations

---

*Add new ideas above this line*
