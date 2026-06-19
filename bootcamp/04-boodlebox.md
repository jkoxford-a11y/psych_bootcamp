---
layout: module
title: "Module 4: Boodlebox — Building Your Course Workspace"
permalink: /bootcamp/04-boodlebox/
prev_url: /bootcamp/03-useful-honest-output/
prev_title: "Module 3: Getting Useful, Honest Output"
next_url: /bootcamp/05-verifying-output/
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
