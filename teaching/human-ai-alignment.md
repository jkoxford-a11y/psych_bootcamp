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

Both images below came from the same prompt:

> “I am imaging a image something like this one, but all the text/writing in the distance is compressing into simpler forms. Just like longterm declarative memories are compressed into sematic memories. Episodes become soemthing that we remember for their utility, what it meant. Does that make sense ask questions.”

The difference is context.

<figure style="margin:1.5rem 0;">
  <img src="{{ site.baseurl }}/assets/images/All%20of%20Psychology.png" alt="A whiteboard-style image showing psychology as a broad conceptual system where lived experience becomes compressed into usable meaning and adaptive action." style="display:block; width:100%; height:auto; border:1px solid #ddd; border-radius:10px; background:#fff;">
  <figcaption><strong>With context:</strong> the AI had the broader project context, so the same prompt became a psychology image: experience → meaning → action.</figcaption>
</figure>

<figure style="margin:1.5rem 0;">
  <img src="{{ site.baseurl }}/assets/images/Simpler%20psychology.png" alt="A simpler whiteboard-style image showing complex writing becoming simpler forms, based only on the raw prompt." style="display:block; width:100%; height:auto; border:1px solid #ddd; border-radius:10px; background:#fff;">
  <figcaption><strong>Without context:</strong> the AI understood the surface request — complex writing becoming simpler — but not the larger conceptual purpose.</figcaption>
</figure>

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
