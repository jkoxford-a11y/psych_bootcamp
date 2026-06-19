---
layout: module
title: "Module 3: Getting Useful, Honest Output"
permalink: /bootcamp/03-useful-honest-output/
prev_url: /bootcamp/02-how-ai-works/
prev_title: "Module 2: How AI Actually Works"
next_url: /bootcamp/04-boodlebox/
next_title: "Module 4: Boodlebox"
---

**TL;DR** Vague prompts produce generic responses. AI also defaults to agreement, which feels helpful and isn't. Both problems have the same fix: be specific about what you want and explicit about how you want it delivered.

---

## Why prompts matter

AI will always give you *something*. The problem is that a vague prompt produces an averaged, hedged, generic response — technically an answer, functionally not useful.

You don't need to learn "prompt engineering." You need to give the AI what any person would need to actually help you: who you are, what you're doing, and what a useful response looks like.

---

## What a stronger prompt has

**Context.** Who you are and what you're working on.

> ❌ "Write a learning objective."
>
> ✅ "I teach intro psychology to first-year undergraduates. Write a learning objective for a unit on memory that emphasizes application over recall."

**Specificity.** What you actually want, not a general version of it.

> ❌ "Give me feedback on this rubric."
>
> ✅ "What's ambiguous in this rubric — the parts where two graders would score the same paper differently?"

**Format.** How you want it back.

> ❌ *(nothing)*
>
> ✅ "Bullet points, not prose." / "One paragraph." / "Draft this as if it's going in the syllabus."

You don't need all three every time. But specificity is almost always worth adding.

---

## When it's not working, redirect

You don't have to start over when a response misses. Correct it in the same conversation:

> "That's not what I meant — what I'm actually asking is..."

> "Too long. Same answer in two sentences."

> "You're assuming I have more context than I do. Start simpler."

The AI isn't offended. Redirect it.

---

## The agreement problem

AI is trained on human feedback — responses rated helpful and pleasant got reinforced. The result: AI learned to agree, validate, and sound confident. It's not trying to flatter you. It's doing what got rewarded during training.

What this looks like in practice: you share a weak argument and the AI finds merit in it. You draft something with a real flaw and the AI leads with what works. You state something incorrect and the AI often goes along.

This is called sycophancy, and it makes AI feel more helpful than it is.

---

## Phrases that fix it

These work because they explicitly override the agreement default.

> **"Ask me questions before starting."**
> Stops the AI from charging ahead on assumptions. The first real exchange is better for it.

> **"What are you least certain about in that response?"**
> Surfaces hedges the AI was smoothing over.

> **"What am I not considering?"**
> Forces gap-finding instead of validation.

> **"Push back on me."**
> Blunt. Effective.

> **"What assumptions are you making?"**
> Useful whenever your prompt left room for interpretation — you may not share those assumptions.

> **"What do you think I'm asking?"**
> Run this when a response feels off. Often reveals a mismatch before it compounds.

> **"Let's iterate — I don't fully know what I want. What's possible here?"**
> Permission to explore. Often produces better results than over-specifying up front.

---

## Giving AI a role

Telling the AI what role to play changes how it responds, not just what it says. Useful faculty modes:

| Task | Role to assign |
|---|---|
| Drafting something new | Collaborative, generative |
| Editing existing writing | Surgical — fix only what's broken |
| Testing an argument | Skeptical reviewer |
| Assignment design | Devil's advocate — how would a student game this? |
| Preparing for a meeting | Hostile questioner |

> "Act as a skeptical peer reviewer. Find the weakest claims in this draft."

---

{% capture do_it_now %}
Open your AI tool now — Boodlebox, Claude, ChatGPT, whichever you have.

Take something real from your course: a learning objective, an assignment prompt, a rubric, a paragraph you're not sure about.

Try a bare prompt first — just describe what you want, no context.

Then try again: add who you are, what specifically you need, and how you want it back.

We'll share what you noticed in 5 minutes.
{% endcapture %}
{% include callout-do-it-now.html content=do_it_now %}

---

## Confidence ≠ correct

AI writes fluently regardless of whether it's right. The tone doesn't change when it's guessing.

Concepts and explanations are generally reliable. Specific facts, citations, dates, and names are where errors concentrate. If it matters, verify it. [→ Module 5](../05-verifying-output/)

---

## Key takeaways

- Context, specificity, and format are the levers — specificity almost always helps
- AI defaults to agreement; this is a training artifact, not a feature — override it explicitly
- Giving AI a role changes how it responds, not just what it covers
- Fluent and confident doesn't mean correct — specific checkable facts are where errors hide
