# Content Updates — Bootcamp Modules 2–6

## Instructions for Code

Replace the content of each file listed below with the content provided in this document. Each section is clearly labeled with the target file path.

- Do not change any Jekyll frontmatter keys that already exist in the files — only update the `title` value where specified
- Preserve all existing layout references (`layout: module`)
- Preserve all existing prev/next link frontmatter if present
- The callout boxes use the capture block syntax already implemented — apply consistently
- Modules 0 and 1 are not included here — leave those files as-is for now

One additional fix while you're in the repo: the site title on the landing page is rendering twice ("AI Literacy — Psychology AI Integration Pilot — AI Literacy — Psychology AI Integration Pilot"). Fix the `_config.yml` site title or the default layout title concatenation so it renders once.

---

## FILE: bootcamp/02-how-ai-works.md

```
---
layout: module
title: "Module 2: How AI Actually Works (Enough to Matter)"
prev: /bootcamp/01-getting-started/
prev_title: "Module 1: Getting Started"
next: /bootcamp/03-useful-honest-output/
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

**For ongoing work, pre-load your context.** If you find yourself re-explaining your course, your assignment, or your expectations at the start of every new chat — that's the problem Module 4 solves. [→ Boodlebox](/bootcamp/04-boodlebox/)

{% capture faculty_note %}
Using Claude directly rather than through Boodlebox? Claude Projects work the same way — custom instructions and uploaded documents that carry across every chat in that project. Set it up once; it's there from the first message every time.
{% endcapture %}
{% include callout-faculty-note.html content=faculty_note %}

---

## When it's wrong, not degraded

Context limits explain some AI errors. Not all of them. AI can be flatly wrong even in a fresh conversation with plenty of window left.

Push back when something seems off — AI will often self-correct when challenged. Ask it to show its reasoning. For anything that actually matters — a citation, a statistic, a claim you're about to put in writing — verify it yourself. The confident tone is not a reliability signal. [→ Module 5](/bootcamp/05-verifying-output/)

---

## Key takeaways

- AI can only see the current conversation — nothing from previous sessions exists to it
- Long chats degrade; when output starts feeling off, open a new chat rather than pushing through
- Capture your state before closing a long session so you can resume without losing progress
- Confident and fluent doesn't mean correct — wrong answers sound exactly like right ones
```

---

## FILE: bootcamp/03-useful-honest-output.md

```
---
layout: module
title: "Module 3: Getting Useful, Honest Output"
prev: /bootcamp/02-how-ai-works/
prev_title: "Module 2: How AI Actually Works"
next: /bootcamp/04-boodlebox/
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

Concepts and explanations are generally reliable. Specific facts, citations, dates, and names are where errors concentrate. If it matters, verify it. [→ Module 5](/bootcamp/05-verifying-output/)

---

## Key takeaways

- Context, specificity, and format are the levers — specificity almost always helps
- AI defaults to agreement; this is a training artifact, not a feature — override it explicitly
- Giving AI a role changes how it responds, not just what it covers
- Fluent and confident doesn't mean correct — specific checkable facts are where errors hide
```

---

## FILE: bootcamp/04-boodlebox.md

```
---
layout: module
title: "Module 4: Boodlebox — Building Your Course Workspace"
prev: /bootcamp/03-useful-honest-output/
prev_title: "Module 3: Getting Useful, Honest Output"
next: /bootcamp/05-verifying-output/
next_title: "Module 5: Verifying What You Get Back"
---

**TL;DR** Boodlebox is the institutional AI tool for this pilot. You'll build a bot loaded with your course materials during this session. The instructions you write are the bot — everything from Module 3 applies directly.

---

## Why Boodlebox

Two reasons. First, it's FERPA-compliant and built for educational use — appropriate for anything involving your course and your students. Second, you can pre-load it with your materials so the AI starts every conversation already knowing your course, your expectations, and your constraints.

That second part changes the experience significantly. General-purpose AI starts every new chat from zero — no knowledge of what you teach, how you assess, or what level your students are at. A Boodlebox bot has your syllabus, your rubrics, and your instructions built in before anyone asks it a single question. The underlying model is the same one you've been working with across Modules 1–3. The skills transfer directly.

---

## Build your bot now

You'll need access to Boodlebox and your syllabus, or any course document that describes what the course covers. This takes about five minutes.

Read the two-bot demo below before you write your instructions — it'll make them better.

{% capture do_it_now %}
1. Open Boodlebox → **Bot Garage**
2. Select **Create a new bot**
3. Name it: `[COURSE NUMBER] [PURPOSE]` — e.g., *PSYC 101 Study Coach*
4. Write one sentence describing what this bot is for
5. Write 3–5 lines of instructions
6. Upload your syllabus and one other document — rubric, reading list, or assignment prompt
7. Save — then test before sharing with anyone
{% endcapture %}
{% include callout-do-it-now.html content=do_it_now %}

---

## The two-bot demo

The difference between a useful bot and a generic one is the instructions. The AI model underneath is identical. Here's what that looks like.

**Bot A — minimal instructions:**
> You are a helpful assistant for PSYC 101.

**Bot B — calibrated instructions:**
> You are a study coach for PSYC 101 at Columbia College of Missouri. Your job is to help students understand material, not do their work for them. Never give a direct answer to a content question without first asking what the student already thinks. If a student is wrong, say so clearly and explain why — don't soften incorrect answers. Prioritize the course syllabus and uploaded materials over your general knowledge. If a student asks about exam policies, grades, or deadlines, direct them to the syllabus.

**Question asked to both:** *"What do I need to know about memory for the exam?"*

Bot A returns a general overview of memory from its training data. Bot B asks what the student already knows and works from the course materials.

Same model. Different instructions. The instructions are the bot.

---

## What good instructions include

- The bot's role and who it's for
- What it should help with
- What it should *not* do — especially: do not complete graded assignments
- Tone and level of detail
- Course-specific rules (policies, citation format, what to do when uncertain)

A starting template:

> You are a learning assistant for students in [COURSE NAME]. Your role is to support learning, not replace student work. Help students understand concepts, ask guiding questions, and give feedback. Do not complete graded assignments. When students ask for direct answers, guide them through the reasoning instead. Use a clear, professional tone appropriate for undergraduates. Prioritize course materials over general knowledge. If you're unsure, say so and recommend the student consult the instructor.

---

## Sharing with students

Post the direct bot link in your LMS — D2L, Canvas, wherever your students live. Tell them what it's for and what it can't do for them. That's the whole workflow.

Name the bot with your course number so students can confirm they have the right one before they start. If you run multiple sections that need different bots, add the section number. Students can also favorite a bot (three-dot menu → Favorite) so it stays accessible in their sidebar.

Suggested LMS language:

> Use the course bot linked below to review concepts, ask questions, and prepare for assignments. It's designed to coach your thinking, not complete graded work. Confirm the bot name matches this course before you begin. You're responsible for checking its responses.

<!-- TODO: verify Boodlebox folder+bot access flow before publishing -->
> ⚠️ **Access method — verifying before launch.** The documentation describes both a direct bot link and a shared course folder for access. The exact workflow for the folder method is being confirmed with Boodlebox. This section will be updated before the bootcamp runs.

---

## What students need to know

{% capture faculty_note %}
Tell students this before they use the bot:

- Access it from the link in your course page — don't search manually
- Confirm the bot name matches your course before you start
- It can make mistakes — you're responsible for checking responses
- It cannot complete graded work for you — that's intentional
{% endcapture %}
{% include callout-faculty-note.html content=faculty_note %}

---

## Key takeaways

- Pre-loading course materials means neither you nor your students have to re-explain context every session
- The instructions are the bot — a calibrated system prompt changes outputs dramatically, not slightly
- Share via direct link posted in your LMS; include the course number in the bot name
- Test before sharing — ask it the questions your students will actually ask
```

---

## FILE: bootcamp/05-verifying-output.md

```
---
layout: module
title: "Module 5: Verifying What You Get Back"
prev: /bootcamp/04-boodlebox/
prev_title: "Module 4: Boodlebox"
next: /bootcamp/06-what-next/
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
```

---

## FILE: bootcamp/06-what-next.md

```
---
layout: module
title: "Module 6: What's Next"
prev: /bootcamp/05-verifying-output/
prev_title: "Module 5: Verifying What You Get Back"
---

**TL;DR** The bootcamp was the floor. Literacy develops through use, not through more reading. Here's what to do with that.

---

## One thing to try this week

Use your Boodlebox bot to answer one question a student actually asked you recently. Notice whether the response was accurate, whether you'd change the instructions, what you'd upload next. That iteration loop — use it, notice what's off, adjust — is how the tool gets useful.

---

## Where this goes

The bootcamp covered the mechanics. The harder questions — how to redesign assessments, how to set a course AI policy, what to tell students — live in the Teaching & Assessment section. That content is being developed across summer 2026. It's not required reading before Fall. It's worth engaging before Spring.

[→ Teaching & Assessment in the AI Era](/teaching/)

---

## What the pilot is actually for

You're not expected to be experts before Fall. The pilot is designed around the assumption that you'll develop fluency through teaching with these tools, not before you do. What you built today — a bot with your course materials, a working mental model of how AI behaves — is enough to start.

The point of starting is to have something real to reflect on by December.

---

## Key takeaways

- Use the bot this week on something real — iteration is how it gets useful
- Assessment redesign and course AI policy are summer reading, not prerequisites for Fall
- Fluency comes from use — the pilot is structured around that, not against it
```
