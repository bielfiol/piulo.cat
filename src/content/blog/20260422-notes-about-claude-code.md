---
title: "Notes about using Claude Code"
pubDate: "2026-04-22"
description: "Reflections on using Claude for code generation and workflows."
tags: ["astro", "blog", "ai", "programming"]
author: "Bielfiol"
---

## Notes about using Claude Code

Today I experimented with Claude to help write code and structure a new Astro blog post. The goal was to keep the content simple, practical, and ready for publishing.

With Claude Code I can use '#' to write an instruction and Claude Code saves it to CLAUDE.md.
For example:
># Use comments sparingly. Only comment complex code.

## Referencing files

To mention a file we can use '@'.
For example, if I want to refer myFolder/myFile.pas I'll write:
>Analyze @myFolder/myFile.pas

## Planning mode

To enable Planning Mode press Shift + Tab twice (once if you want auto-accepting edits).

In Planning Mode Claude will:
- Read more files in your project
- Create a detailed implementation plan
- Show you exactly what it intends to do
- Wait for your approval before proceeding


## Thinking modes
The available thinking modes include:
- "Think" - Basic reasoning
- "Think more" - Extended reasoning
- "Think a lot" - Comprehensive reasoning
- "Think longer" - Extended time reasoning
- "Ultrathink" - Maximum reasoning capability

## Planning vs Thinking

Planning Mode works best for broad tasks involving multiple files, while Thinking Mode suits complex logic and debugging. Both can be combined, but keep in mind they use more tokens.

## Commands

### /clear
Removes completely the conversation history.

### /compact
Summarizes your entire conversation history preserving the learning.

### /init
Creates the CLAUDE.md file in your project.

### /help
Shows all available commands.

### /cost
Displays the tokens consumed in the current session.

### /model
Switches the model (Sonnet, Opus, etc.).

### /exit
Closes Claude Code.