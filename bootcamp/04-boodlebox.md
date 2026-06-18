---
layout: module
title: "Module 4: Boodlebox — Building Your Course Workspace"
permalink: /bootcamp/04-boodlebox/
tldr: "Boodlebox is the institutional AI tool for this pilot. By the end of this module, you'll have a working bot loaded with your course materials. The instructions you write are the bot."
prev_url: /bootcamp/03-useful-honest-output/
prev_title: "Module 3: Getting Useful, Honest Output"
next_url: /bootcamp/05-verifying-output/
next_title: "Module 5: Verifying What You Get Back"
---

# Module 4: Boodlebox — Building Your Course Workspace

> **Note for Jon:** This module is original writing based on the build plan spec. Review carefully before publishing — particularly Part 4 (sharing mechanic), which is flagged for verification below.

## Part 1: Why Boodlebox

Boodlebox is the AI platform for this pilot for two reasons: it's FERPA-compliant and designed for educational use, and it lets you pre-load course materials so context is always there.

That second part matters more than it sounds. Every time you start a new chat with a general-purpose AI tool, you're starting from scratch — no knowledge of your course, your students, your expectations. In Boodlebox, you build a bot with your syllabus, your rubrics, and your instructions built in. Every conversation starts with your context already present. Your students don't have to paste in the syllabus. You don't have to re-explain what level you're teaching.

Everything you just learned about prompting and calibration in Modules 1–3 applies directly here.

## Part 2: Building Your Course Workspace Bot

You'll do this during the session. You'll need: access to Boodlebox (link from your bootcamp facilitator) and your syllabus, or any course document that describes what the course covers.

{% capture do_it_now %}
**Build your bot now** — syllabus in hand, about 5 minutes.

1. Open Boodlebox and go to the **Bot Garage**
2. Select **Create a new bot**
3. Name it: use format `[COURSE NUMBER] [PURPOSE]` — e.g., *PSYC 101 Study Coach*
4. Write a one-sentence description of what this bot is for
5. Write 3–5 lines of instructions (see Part 3 below for what good instructions look like)
6. Upload your syllabus and one other document — a rubric, reading list, or assignment prompt
7. Save and test before sharing

We'll test it together before you share it with anyone.
{% endcapture %}
{% include callout-do-it-now.html content=do_it_now %}

## Part 3: The Two-Bot Demo

The difference between a useful course bot and a generic one isn't the AI model — it's the instructions. Here's a live illustration.

**Bot A — minimal instructions:**

> You are a helpful assistant for PSYC 101.

**Bot B — calibrated instructions:**

> You are a study coach for PSYC 101 at Columbia College of Missouri. Your job is to help students understand material, not to do their work for them. Never give a direct answer to a content question without first asking the student what they already think. If a student is wrong, tell them clearly and explain why — do not soften incorrect answers with praise. Prioritize the course syllabus and uploaded materials over your general knowledge. If a student asks about exam policies, grades, or deadlines, direct them to the syllabus.

**Demo question asked to both:** *"What do I need to know about memory for the exam?"*

Bot A produces a general memory overview drawn from its training data. Bot B asks what the student already knows and anchors its response to the course materials.

The difference is the instructions. The instructions are the bot.

This connects back to Module 3 — you're applying calibration and role-setting in a tool you can hand directly to students.

### What Good Bot Instructions Include

- The bot's role and who it's for
- What it should help with
- What it should *not* do — especially: do not complete graded assignments for students
- Tone and level of detail
- Any course-specific rules (exam policies, citation format, etc.)

**Template you can copy and modify:**

> You are a helpful AI learning assistant for students in [COURSE NAME]. Your role is to support learning, not replace student work. Help students understand concepts, ask guiding questions, and provide feedback. Do not complete graded assignments for students. When students ask for direct answers, guide them through the reasoning process instead. Use a supportive, clear, and professional tone appropriate for undergraduate students. Align your responses with the course materials and instructions provided. If you are unsure, say so and recommend that students consult the instructor or course materials.

## Part 4: Sharing with Students

<!-- TODO: verify Boodlebox folder+bot access flow before publishing -->

The primary method for sharing your bot is to post the direct bot link in your LMS (D2L, Canvas, or whatever you use). Tell students what the bot is for and what it cannot do for them.

**Naming so students know they have the right one:** Include your course number in the bot name. If you have multiple sections, include the section number. Students can confirm they're in the right place before they start.

Students can save a bot for easy access using the Favorites feature (three-dot menu → Favorite).

**Suggested LMS language you can copy:**

> Use the course bot linked below to help you review concepts, ask questions, and prepare for assignments. The bot is designed to coach your thinking, not complete graded work for you. Confirm the bot name matches this course before you begin. You are responsible for checking all information and following the course AI use policy.

**Access method coming — verifying with Boodlebox before publishing.** The documentation describes two sharing methods (direct bot link and shared course folder) but the exact workflow for shared folder access is being confirmed. This section will be updated before launch.

## Part 5: What Students Need to Know

{% capture faculty_note %}
**Tell students this before they use the bot:**

- Use the link from your course page — don't search for bots manually
- Confirm the bot name matches your course before you start
- The bot can make mistakes. You are responsible for checking its responses
- The bot cannot complete graded work for you — that's by design
{% endcapture %}
{% include callout-faculty-note.html content=faculty_note %}
