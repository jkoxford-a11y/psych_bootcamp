---
layout: module
title: "Module 2: How AI Actually Works (Enough to Matter)"
permalink: /bootcamp/02-how-ai-works/
tldr: "AI doesn't have unlimited memory. Long conversations degrade. Knowing why — and what to do about it — saves you a lot of frustration."
prev_url: /bootcamp/01-getting-started/
prev_title: "Module 1: Getting Started"
next_url: /bootcamp/03-useful-honest-output/
next_title: "Module 3: Getting Useful, Honest Output"
---

# Module 2: How AI Actually Works (Enough to Matter)

## What Is a Context Window?

Think of a context window as the AI's working memory. It can only "see" what's in the current conversation. Everything outside that window — previous chats, things you told it last week, work from a different session — does not exist to it.

That window has a size limit, measured in **tokens**. A token is roughly a word. Every message you send, and every response you receive, uses tokens from that budget. When the budget runs low, performance degrades — the AI starts losing track of earlier parts of the conversation.

**The practical version:** Long chats tend to go worse than short ones. That's not random.

## Why AI Makes Mistakes in Long Conversations

As a conversation gets longer, a few things tend to happen:

- The AI starts forgetting constraints or instructions you set early on
- It contradicts things it said earlier
- Answers get vaguer or less accurate
- It may drift away from the specific task you established

When this happens, it's tempting to assume the AI is just bad at the topic. Usually the real cause is a full or nearly-full context window. It's not getting dumber — it's losing the thread.

**Symptom to watch for:** If the AI's answers suddenly feel off, inconsistent, or like it forgot what you were doing — that's the signal.

## What To Do About It

### Start Fresh When Things Go Sideways

The simplest fix is also the most counterintuitive: stop, open a new chat, and start over. Don't keep pushing a degraded conversation hoping it improves. A fresh context window means a fresh slate — and usually better answers.

### Save Your Context Before You Do

Before you close a long chat, ask the AI to package up what you accomplished:

> *"Summarize this conversation: what we were working on, decisions we made, and where we left off. Make it detailed enough that I can paste it into a new chat and pick up without losing anything."*

Then paste that summary at the start of your next chat. You've effectively transferred the session.

{% capture faculty_note %}
If you're using Claude directly (not through Boodlebox), Claude Projects serve the same function as a persistent workspace — custom instructions and uploaded materials that carry across every chat in that project. You set it up once and the context is there from the first message of every session.
{% endcapture %}
{% include callout-faculty-note.html content=faculty_note %}

### Use a Course Workspace for Ongoing Work

The deeper fix: if you're constantly re-explaining your course, your assignment, or your expectations — that's a sign you need a workspace pre-loaded with that context. That way it's there from the first message of every chat. [See Module 4: Boodlebox]({{ site.baseurl }}/bootcamp/04-boodlebox/)

## When AI Is Just Wrong (Not Degraded)

Context window issues explain *some* AI errors — but not all of them. AI can also simply be wrong, even in a fresh chat at the start of a conversation.

**What to do:**

- Push back directly: *"I think that might be incorrect — can you double-check?"* AI will often self-correct when challenged
- Ask it to explain its reasoning — errors often surface when the AI has to show its work
- For anything that actually matters (a fact, a citation, a specific claim), verify it yourself

AI sounds confident whether it's right or wrong. That tone is not a reliability signal. [See Module 5: Verifying What You Get Back]({{ site.baseurl }}/bootcamp/05-verifying-output/)
