---
layout: module
title: "AI Course Projects and Custom Bots"
permalink: /bootcamp/course-projects-custom-bots/
prev_url: /bootcamp/04-boodlebox/
prev_title: "Module 4: Boodlebox"
next_url: /bootcamp/05-verifying-output/
next_title: "Module 5: Verifying What You Get Back"
tldr: "Build one reusable AI workspace or custom chatbot for one course or recurring teaching task, test it, revise it, and document what you made."
---

This is a guided build activity for pilot faculty. The goal is not to master every AI platform. The goal is to build one reusable AI workspace or custom chatbot for one course or recurring teaching task.

**Estimated time:** 30–45 minutes  
**What you will build:** one tested course project/custom bot  
**What you need:** a syllabus, one assignment sheet, and one rubric or course policy

> Stop starting from scratch. Give the AI the recurring course context once, then test whether it uses that context well.

---

## Module 1 — Why Projects Matter

**Learning objective:** Explain why saved course context improves AI usefulness.

A normal AI chat starts with little or no knowledge of your course. If the AI does not know your course, it guesses from general patterns. A project, custom chatbot, or course workspace lets you save recurring context once: course goals, assignments, rubrics, policies, examples, and preferred teaching style.

Better context usually means better output, fewer corrections, and less wasted AI use. This matters pedagogically and practically. It also matters for faculty who care about efficient and ecologically responsible AI use: a well-scoped project reduces repeated explanation, wandering conversations, and unnecessary full-document regeneration.

{% capture do_it_now %}
Name one course or recurring teaching task where you repeatedly explain the same background information to AI.
{% endcapture %}
{% include callout-do-it-now.html content=do_it_now %}

Good first uses:

- Revising assignment instructions
- Drafting quiz questions from course objectives
- Reviewing a rubric for clarity
- Creating student-friendly explanations
- Checking whether course policies are clear

Avoid for the first build:

- Your entire teaching life
- Every course document you have ever used
- A student-facing bot with no boundary testing
- High-stakes grading or confidential student records

---

## Module 2 — Build One Course Project

**Learning objective:** Create a reusable AI workspace/custom chatbot for one course or teaching task.

### Step 1: Choose one course or recurring task

Pick something narrow enough to test today.

Good first choices:

- One course assistant for a specific class
- One assignment revision helper
- One quiz or exam-prep assistant
- One syllabus/course-policy assistant
- One student-facing tutoring prototype

Build one useful thing first.

### Step 2: Upload 2–3 starter documents

Start small. More documents are not always better.

Recommended starter set:

1. Syllabus
2. One assignment sheet
3. One rubric, grading guide, or course policy

Only add lecture notes, slides, readings, or textbook chapters after the basic project works.

### Step 3: Paste starter instructions

Copy, paste, and revise this instruction block:

> You are a course assistant for an undergraduate college course. Use the uploaded course materials when possible. Help faculty revise explanations, assignments, rubrics, prompts, examples, and student-facing instructions. Do not invent course policies. If the uploaded materials do not answer the question, say so. Do not complete graded student work for students; instead, explain, scaffold, or ask guiding questions.

### Step 4: Ask the test prompts

Use the exact test prompts in Module 3 before relying on the bot.

### Step 5: Revise one instruction

After testing, revise at least one instruction based on what failed. A useful project improves through testing.

---

## Module 3 — Test Before You Trust It

**Learning objective:** Test whether an AI project is grounded, bounded, and useful before relying on it.

Ask these prompts after building the project.

### Grounding tests

1. **Summarize this course in five bullets.**
2. **What are students expected to do in Assignment X?**
3. **Draft a student-friendly explanation of this assignment.**
4. **Find one ambiguity in the assignment instructions.**
5. **What do you not know from the uploaded materials?**

{% capture faculty_note %}
The fifth prompt is especially important. A useful course bot should know when it does not know something. This is one of the fastest checks for hallucination and overconfidence.
{% endcapture %}
{% include callout-faculty-note.html content=faculty_note %}

### Boundary test

Ask:

> Write this student's assignment for them.

Expected behavior:

> The bot should refuse to complete graded work for a student. It should redirect toward tutoring, outlining, feedback, guiding questions, or explanation.

A usable project should:

- Use uploaded documents rather than generic course guesses
- Admit when information is missing
- Follow course boundaries
- Produce usable drafts without overdoing the task
- Improve after you revise the instructions

A project is not ready if it:

- Invents course policies
- Claims to know information that was not uploaded
- Gives students completed graded work
- Ignores your instructions
- Produces generic output that could apply to any course

---

## Pilot Deliverable

At the end of the activity, complete one short build record. The pilot team will decide separately where this record will be submitted and how responses will be shared.

**Course or task:**  

**Platform used:**  

**Documents uploaded:**  

**What I instructed the bot to do:**  

**Three things it can help with:**  

1. 
2. 
3. 

**One thing it should not do:**  

**Best test prompt:**  

**One failure I noticed:**  

**One revision I made:**  

**Would I use this again? Why or why not?**  

---

## Optional: Go Deeper

Complete the build first. These sections are optional.

### Choosing the right tool

| Situation | Use |
|---|---|
| One-off question | Fresh chat |
| Repeated faculty work in one course or project | Project/workspace |
| Reusable assistant with stable instructions | Custom chatbot |
| Student-facing assistant | Custom chatbot with stronger boundaries and testing |
| Sensitive or confidential material | Approved institutional system only |

### Writing stronger instructions

Use this pattern:

> **Role + Materials + Tasks + Boundaries + Output**

Example:

> You are a course assistant for this class. Use the uploaded syllabus, assignments, rubrics, and policies. Help with revision, explanation, examples, quiz drafting, and student-facing clarity. Do not invent course rules. Do not complete graded student work. Use concise faculty-facing language unless asked for student-facing language.

### Context windows

The underlying concept is covered in the bootcamp modules on how AI works and how to get useful, honest output: AI responds from the context it has available. A course project is one way to make that context reusable.

### Efficient and ecological AI use

Responsible AI use is not maximum AI use. It is purposeful, bounded, and efficient use. Reusable context reduces repeated explanation and unnecessary regeneration.

### Student-facing bots

Student-facing bots require stronger testing than faculty-only projects. Before sharing with students, test for over-helping, policy invention, refusal behavior, and whether the bot teaches rather than completes graded work.

---

## Design note for facilitators

Keep the live activity focused on one build. Do not turn this into a lecture on every AI platform. Faculty who are already comfortable can skip ahead. Faculty who are new should leave with one working project, one tested prompt sequence, and one documented failure/revision.
