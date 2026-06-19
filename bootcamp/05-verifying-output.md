---
layout: module
title: "Module 5: Verifying What You Get Back"
permalink: /bootcamp/05-verifying-output/
prev_url: /bootcamp/04-boodlebox/
prev_title: "Module 4: Boodlebox"
next_url: /bootcamp/06-what-next/
next_title: "Module 6: What's Next"
---

**TL;DR** AI sounds authoritative whether it's right or wrong. The tone is not a reliability signal. A few habits protect you from confidently using something incorrect.

---

## The core problem

AI generates text that reads like it comes from a confident, knowledgeable source. That doesn't change when it's guessing. There's no asterisk, no hedge in tone, no signal that this particular sentence is less reliable than the one before it.

This isn't a flaw that will be patched — it's how the technology works. Output is a statistically plausible continuation of your prompt, not a lookup from a verified database. A fabricated citation looks identical to a real one. A slightly wrong statistic reads the same as a correct one.

---

## What gets wrong most often

**Verify these:**
- Specific statistics and numbers
- Citations — author names, journals, publication years
- Recent events (AI knowledge has a cutoff; it doesn't know what happened last month)
- Anything highly specific and checkable

**Generally reliable:**
- Explanations of concepts and mechanisms
- Definitions
- Structuring and organizing ideas *you* provide
- Summarizing material you uploaded yourself

The pattern: AI is better at working with your content than producing factual specifics from its own training.

---

## How to actually check

**Ask it to show its work.**
> *"Walk me through your reasoning step by step."*

Errors surface under examination. A confident wrong answer often falls apart when the AI has to be explicit about how it got there.

**Ask for uncertainty.**
> *"What are you least certain about in that response?"*
>
> *"Flag anything you're not confident about."*

Not foolproof — but it surfaces hedges the AI was glossing over.

**Search for any citation it gives you.**

Don't assume it exists. AI fabricates citations with some regularity and they look completely real — correct journal name, plausible author, reasonable year. Search before you use it anywhere.

**Use your expertise as the filter.**

If AI says something that contradicts your course materials, your field knowledge, or your own judgment — trust those first. AI draws from the internet broadly. Your disciplinary expertise is the standard, not a tie-breaker.

{% capture faculty_note %}
Citation fabrication is higher stakes when something goes into a syllabus reading list, a grant narrative, or anything in print. Verify every citation AI generates before it leaves your hands.
{% endcapture %}
{% include callout-faculty-note.html content=faculty_note %}

---

## A note on AI with web search

Many AI tools can search the web before responding — Claude, Perplexity, ChatGPT with search enabled. For literature-grounded tasks, asking AI to search first is worth doing. It reduces citation fabrication, pulls in recent work beyond the AI's training cutoff, and — crucially — when AI presents sources inline you can follow the link directly rather than hunting for a citation blind.

That last part matters. A linked source you can click is a fundamentally different verification situation than a citation you have to go find yourself.

It doesn't eliminate the problem entirely. Search results vary in quality, and AI can mischaracterize a real source as readily as it fabricates a fake one — a real paper, summarized wrong, is still a wrong claim. The rule stays the same: verify what it says a source says, not just that the source exists.

A prompt worth keeping:

> *"Search the literature before responding. Present your sources so I can check them."*

---

## A practical rule

If you'd be embarrassed to be wrong about it in a meeting or in print — verify it.

Concepts and explanations are generally fine. Specific, checkable facts are where errors concentrate.

---

## Key takeaways

- Fluent and confident doesn't mean correct — the tone never changes when AI is guessing
- Specific facts, citations, and statistics are highest risk; concepts and explanations are generally reliable
- Search for any citation before using it — fabricated references look real
- Asking AI to search the web and present sources reduces risk but doesn't eliminate it
- Your disciplinary expertise is the standard; AI is the draft, not the authority
