---
layout: module
title: "Module 2: How AI Actually Works (Enough to Matter)"
permalink: /bootcamp/02-how-ai-works/
prev_url: /bootcamp/01-getting-started/
prev_title: "Module 1: Getting Started"
next_url: /bootcamp/03-useful-honest-output/
next_title: "Module 3: Getting Useful, Honest Output"
---

**TL;DR** AI has working memory, not unlimited memory. Long chats degrade. A few habits make this a non-issue.

---

## What a context window actually is

Every AI conversation runs inside a context window — the full text of everything said so far, your messages and the AI's responses combined. The AI can only see what's in that window. Previous conversations, work from a different chat, things you told it last week — none of that exists to it.

The window has a size limit measured in tokens (roughly: words). As it fills up, performance degrades. Earlier instructions get forgotten. The AI starts contradicting itself or giving vaguer answers than it was giving an hour ago.

This isn't the AI getting confused about your topic. It's losing access to the beginning of its own context.

**The tell:** A conversation that was working suddenly feels off — vague, inconsistent, like it forgot what you were doing. That's the limit.

---

## What to do about it

**Start fresh.** Close the chat and open a new one. Don't try to rehabilitate a degraded conversation. A new window is a new start.

**Before you do, capture your state.** Paste this before closing any long chat you want to continue:

> *"Summarize this conversation: what we were working on, decisions we made, and where we left off. Make it detailed enough that I can paste it into a new chat and pick up without losing anything."*

Paste the summary at the top of your next chat. Session transferred.

**For ongoing work, pre-load your context.** If you find yourself re-explaining your course, your assignment, or your expectations at the start of every new chat — that's the problem Module 4 solves. [→ Boodlebox](../04-boodlebox/)


---

## When it's wrong, not degraded

Context limits explain some AI errors. Not all of them. AI can be flatly wrong even in a fresh conversation with plenty of window left.

Push back when something seems off — AI will often self-correct when challenged. Ask it to show its reasoning. For anything that actually matters — a citation, a statistic, a claim you're about to put in writing — verify it yourself. The confident tone is not a reliability signal. [→ Module 5](../05-verifying-output/)

---

## Key takeaways

- AI can only see the current conversation — nothing from previous sessions exists to it
- Long chats degrade; when output starts feeling off, open a new chat rather than pushing through
- Capture your state before closing a long session so you can resume without losing progress
- Confident and fluent doesn't mean correct — wrong answers sound exactly like right ones
