---
layout: default
title: "Human-AI Cognitive Alignment"
permalink: /teaching/human-ai-alignment/
---

# AI Use Guide: Human-AI Cognitive Alignment

## Part 1: Getting What You Want

<div class="tldr"><strong>Core idea:</strong> AI can only work with the context it receives. Better context produces better output.</div>

<figure class="hero-figure">
  <img src="{{ site.baseurl }}/assets/images/human-ai-cognitive-alignment.png" alt="Infographic showing human mental context being translated into prompt context, AI producing better output, and a feedback loop for review, revision, and trying again.">
  <figcaption>Human-AI cognitive alignment: convert rich mental context into usable prompt context, review the output, revise, and try again.</figcaption>
</figure>

---

## The core idea

AI is a neural network — for our purposes, a black box. It takes input and produces a probable output.

That input is all it has to work with.

Your first prompt is rarely enough. Good AI use usually requires iteration. Treat it like a conversation with a colleague: you explain, check whether it understood, revise the context, and try again.

Your goals, memories, examples, standards, and background knowledge have to be converted into usable context, mostly through text.

---

## What context means

Context is everything available to the model in a chat:

- your messages
- previous replies
- uploaded files
- images
- search results
- project instructions
- saved preferences or memory, depending on the platform

The model does not have your full mind. It has the working context you give it.

Long chats can accumulate clutter. The model may lose earlier details, blend topics, or follow irrelevant context. Keep chats short and focused when possible.

Do not change topics inside the same chat unless the topics are closely related.

---

## Same prompt, different context

Both images below come from the same basic request: a whiteboard-style image showing complex ideas compressing into simpler forms.

The difference is context.

<div style="display:grid; grid-template-columns:repeat(auto-fit, minmax(280px, 1fr)); gap:1.25rem; align-items:start; margin:1.25rem 0;">
  <figure style="margin:0;">
    <svg viewBox="0 0 900 560" role="img" aria-label="A generic whiteboard-style image with vague diagrams, scribbles, and simplified marks." style="width:100%; height:auto; border:1px solid #ddd; border-radius:10px; background:#fff;">
      <rect width="900" height="560" fill="#fbfbf8"/>
      <rect x="24" y="24" width="852" height="512" rx="18" fill="#ffffff" stroke="#c9c9c9" stroke-width="4"/>
      <text x="52" y="68" font-size="28" font-family="Arial, sans-serif" fill="#183a6b" font-weight="700">WITHOUT CONTEXT</text>
      <text x="52" y="102" font-size="18" font-family="Arial, sans-serif" fill="#555">The AI gets the visual genre.</text>
      <g stroke="#2f5597" stroke-width="4" fill="none" opacity=".8">
        <path d="M70 160 C120 110, 180 200, 235 145 S350 110, 390 180"/>
        <path d="M74 230 C130 220, 150 270, 230 252 S350 230, 405 280"/>
        <path d="M86 330 C140 295, 210 370, 270 320 S350 315, 415 350"/>
      </g>
      <g fill="#f2d7d5" stroke="#c0392b" stroke-width="2" opacity=".9">
        <circle cx="505" cy="150" r="16"/><circle cx="558" cy="184" r="12"/><circle cx="610" cy="142" r="20"/><circle cx="672" cy="188" r="14"/>
        <rect x="500" y="245" width="52" height="34" rx="7"/><rect x="584" y="260" width="72" height="38" rx="8"/><rect x="698" y="248" width="44" height="44" rx="10"/>
      </g>
      <g stroke="#777" stroke-width="3" opacity=".85">
        <line x1="74" y1="425" x2="230" y2="425"/><line x1="74" y1="455" x2="320" y2="455"/><line x1="74" y1="485" x2="270" y2="485"/>
        <line x1="500" y1="420" x2="735" y2="420"/><line x1="500" y1="455" x2="690" y2="455"/><line x1="500" y1="490" x2="750" y2="490"/>
      </g>
      <g fill="#183a6b" opacity=".75">
        <circle cx="150" cy="180" r="5"/><circle cx="193" cy="260" r="5"/><circle cx="310" cy="212" r="5"/><circle cx="335" cy="336" r="5"/>
      </g>
      <path d="M425 280 L475 280" stroke="#444" stroke-width="8" marker-end="url(#arrow1)"/>
      <defs><marker id="arrow1" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto"><path d="M0,0 L0,6 L9,3 z" fill="#444"/></marker></defs>
      <text x="52" y="525" font-size="20" font-family="Arial, sans-serif" fill="#222">Surface request: “complex writing becomes simpler.”</text>
    </svg>
    <figcaption><strong>Without context:</strong> plausible whiteboard aesthetic, but the idea stays generic.</figcaption>
  </figure>

  <figure style="margin:0;">
    <svg viewBox="0 0 900 560" role="img" aria-label="A structured psychology whiteboard showing lived experience becoming semantic knowledge that guides adaptive action." style="width:100%; height:auto; border:1px solid #ddd; border-radius:10px; background:#fff;">
      <rect width="900" height="560" fill="#fbfbf8"/>
      <rect x="24" y="24" width="852" height="512" rx="18" fill="#ffffff" stroke="#c9c9c9" stroke-width="4"/>
      <text x="52" y="68" font-size="28" font-family="Arial, sans-serif" fill="#183a6b" font-weight="700">WITH CONTEXT</text>
      <text x="52" y="102" font-size="18" font-family="Arial, sans-serif" fill="#555">The AI gets the conceptual job.</text>
      <defs><marker id="arrow2" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto"><path d="M0,0 L0,6 L9,3 z" fill="#444"/></marker></defs>
      <g font-family="Arial, sans-serif" text-anchor="middle">
        <rect x="50" y="160" width="125" height="120" rx="18" fill="#eef4ff" stroke="#2f5597" stroke-width="3"/>
        <text x="112" y="195" font-size="17" fill="#183a6b" font-weight="700">LIVED</text><text x="112" y="220" font-size="17" fill="#183a6b" font-weight="700">EXPERIENCE</text><text x="112" y="250" font-size="15" fill="#333">episodes</text>
        <rect x="220" y="160" width="125" height="120" rx="18" fill="#f0f7ed" stroke="#4f7d34" stroke-width="3"/>
        <text x="282" y="195" font-size="17" fill="#2e5a1c" font-weight="700">ATTENTION</text><text x="282" y="220" font-size="17" fill="#2e5a1c" font-weight="700">& MEMORY</text><text x="282" y="250" font-size="15" fill="#333">select / encode</text>
        <rect x="390" y="160" width="125" height="120" rx="18" fill="#fff4e8" stroke="#c76b21" stroke-width="3"/>
        <text x="452" y="195" font-size="17" fill="#9b4511" font-weight="700">PATTERNS</text><text x="452" y="220" font-size="17" fill="#9b4511" font-weight="700">& MEANING</text><text x="452" y="250" font-size="15" fill="#333">compress</text>
        <rect x="560" y="160" width="125" height="120" rx="18" fill="#f2efff" stroke="#5b4aa1" stroke-width="3"/>
        <text x="622" y="195" font-size="17" fill="#392d7a" font-weight="700">SEMANTIC</text><text x="622" y="220" font-size="17" fill="#392d7a" font-weight="700">KNOWLEDGE</text><text x="622" y="250" font-size="15" fill="#333">concepts</text>
        <rect x="730" y="160" width="125" height="120" rx="18" fill="#fff0f0" stroke="#b23a3a" stroke-width="3"/>
        <text x="792" y="195" font-size="17" fill="#8c1d1d" font-weight="700">ADAPTIVE</text><text x="792" y="220" font-size="17" fill="#8c1d1d" font-weight="700">ACTION</text><text x="792" y="250" font-size="15" fill="#333">behavior</text>
      </g>
      <g stroke="#444" stroke-width="6" marker-end="url(#arrow2)">
        <line x1="180" y1="220" x2="212" y2="220"/><line x1="350" y1="220" x2="382" y2="220"/><line x1="520" y1="220" x2="552" y2="220"/><line x1="690" y1="220" x2="722" y2="220"/>
      </g>
      <path d="M790 304 C720 385, 210 385, 120 306" stroke="#183a6b" stroke-width="5" fill="none" marker-end="url(#arrow2)"/>
      <text x="455" y="420" font-size="18" font-family="Arial, sans-serif" fill="#183a6b" text-anchor="middle" font-weight="700">Feedback loop: action creates new experience</text>
      <g font-family="Arial, sans-serif" font-size="16" fill="#333">
        <text x="70" y="475"><tspan font-weight="700" fill="#183a6b">Evolution</tspan> builds mechanisms</text>
        <text x="290" y="475"><tspan font-weight="700" fill="#4f7d34">Development</tspan> tunes the system</text>
        <text x="540" y="475"><tspan font-weight="700" fill="#c76b21">Social life</tspan> shapes inputs</text>
        <text x="70" y="510"><tspan font-weight="700" fill="#5b4aa1">Cognition</tspan> organizes meaning</text>
        <text x="390" y="510"><tspan font-weight="700" fill="#b23a3a">Errors and mismatches</tspan> can become disorders</text>
      </g>
    </svg>
    <figcaption><strong>With context:</strong> the same request becomes a psychology model: experience → semantic knowledge → adaptive action.</figcaption>
  </figure>
</div>

Context does not just add detail. It changes what the AI thinks the task is.

A prompt tells the AI what to make.  
Context tells the AI what the work is for.

---

## Saving good workflows

At the end of a productive session, ask the AI to write a reusable prompt or summary.

Use that prompt to start a cleaner, shorter chat next time.

A short chat with a strong starting prompt usually beats a long chat full of drift.

---

## Projects and custom bots

For recurring tasks — a specific course, research workflow, assignment type, or writing style — use a Project or custom chatbot.

These tools can store standing instructions and files, so the AI starts with consistent context before you type a new prompt.

This improves consistency. It also reduces how much you have to repeat.

Ask your chatbot how to set one up.

---

## Two cautions about how AI communicates

AI often sounds confident even when it should not.

This is not because it intends to deceive. It has no intent. It produces fluent language based on patterns in its training and the context you provide.

AI can also be too agreeable. Human feedback training can reward answers people like, which can make the model more likely to affirm weak ideas instead of challenging them.

Counter this with explicit instructions:

> Flag uncertainty and give confidence ratings.
>
> Be objective, not encouraging.
>
> Tell me what could be wrong.
>
> Separate evidence from speculation.
>
> Do not invent sources.

Most AI platforms also allow saved preferences or custom instructions. These are good places for standing instructions about honesty, uncertainty, and critique.

---

## Before using any output

Ask:

- Is this accurate?
- What evidence supports it?
- What did I fail to tell it?
- What assumptions did it make?
- Does this match the task?

AI output is not finished work until a human has checked it.

---

## Weak prompt / better prompt

**Weak:** Help me with my paper.

**Better:** I am writing a five-page paper for Intro Psych on sleep and memory. Here is the rubric. Do not rewrite the paper. Give me the three highest-priority revisions and explain why.

---

## Summary

AI works from context.

Think of the context window as the model's working memory: standing instructions, your prompt, uploaded materials, and the running conversation.

Shorter chats, clear goals, saved workflows, and explicit instructions for honesty will consistently outperform long, unfocused sessions.

This is Part 1. Part 2 will cover responsible use: learning, teaching, privacy, attribution, and work that is actually yours.

---

## Phrases to steal

Use these when you do not yet know what you need.

> Ask me questions before starting.

> What do you think I am asking?

> What am I not considering?

> What assumptions are you making?

> Give me confidence ratings. What are you most and least certain about?

> Be objective, not encouraging.

> Tell me what could be wrong.

> Search the web and find evidence-based solutions.

> Let's iterate. I do not know exactly what I want yet. What is possible?

> Turn this productive chat into a reusable prompt for next time.

---

<nav class="module-nav" aria-label="Section navigation">
  <a class="module-nav__prev" href="../">← Back to Teaching & Assessment</a>
  <a class="module-nav__next" href="../../">Back to home →</a>
</nav>
