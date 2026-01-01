# OpenTools Hub - Project Ideas

Project ideas and feature requests for OpenTools Hub. See [ABOUT.md](ABOUT.md) for more info.

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

*Add new ideas above this line*
