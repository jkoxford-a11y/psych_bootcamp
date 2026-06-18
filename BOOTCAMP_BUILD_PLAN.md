# AI Literacy Bootcamp — Build Plan for Claude Code

**Project:** Psychology AI Integration Pilot — Faculty-Facing GitHub Pages Site  
**Repo:** github.com/jkoxford-a11y (existing repo, existing Pages setup)  
**Owner:** Jon Oxford, Columbia College of Missouri  
**Status:** Content plan finalized. Ready to build.

---

## What This Is

A static GitHub Pages site for faculty participating in the Psychology AI Integration Pilot (launching Fall 2026). The site replaces a Notion-based approach that was too cognitively loaded for a faculty audience that is largely new to AI.

The goal is not comprehensive AI education. It is: give faculty enough to start using AI productively and safely, then develop literacy through actual usage. Everything on the site should serve that constraint.

The site has two sections:

- **Section 1 — Bootcamp:** Six sequential modules. All available day one. Designed to be walked through in a single session (~75–90 min with hands-on time).
- **Section 2 — Teaching & Assessment in the AI Era:** Faculty-only deeper content. Stubs on day one, filled across summer 2026. Not required for the bootcamp.

---

## Design Constraints

- Static site only. No backend, no login, no database.
- Clean, readable, low visual noise. This is reference material, not a marketing page.
- Mobile-readable (faculty will look at this on their phones).
- Each module should be a standalone page with a clear title, a TL;DR at the top, and a "next" link at the bottom.
- Consistent page template across all modules: TL;DR → body content → callout boxes where appropriate → related links.
- Callout boxes for two types of content: **do-it-now** (hands-on activity during bootcamp) and **faculty note** (something that applies specifically to instructors, not students).
- No emoji in headings or navigation. Body content can use them sparingly if it aids tone.
- The tools reference sidebar page is templated — designed so Jon can update one data file (e.g., a YAML or simple markdown table) and the page regenerates. Keep tool info out of module prose so it doesn't go stale.
- Section 2 pages that are not yet written should render as clean stubs: title, one-sentence description, "content coming soon" — not 404s.

---

## Site Structure

```
/
├── index.html (or index.md)          — landing page, links to both sections
├── bootcamp/
│   ├── index.md                      — bootcamp overview, module list
│   ├── 00-why-this-matters.md        — Module 0: cold open
│   ├── 01-getting-started.md         — Module 1: getting started with AI
│   ├── 02-how-ai-works.md            — Module 2: memory and context
│   ├── 03-useful-honest-output.md    — Module 3: prompting and calibration
│   ├── 04-boodlebox.md               — Module 4: Boodlebox workspace and bots
│   └── 05-verifying-output.md        — Module 5: fact-checking and verification
│   └── 06-what-next.md               — Module 6: what's next
├── teaching/
│   ├── index.md                      — section landing page
│   ├── why-assessment-has-to-change.md   — stub
│   ├── assessment-redesign.md            — stub
│   ├── portfolio-mastery-method.md       — stub (note: keep access-controlled if possible)
│   ├── course-ai-policy.md               — stub
│   └── human-ai-alignment.md             — stub
└── reference/
    └── ai-tools.md                   — sidebar: current AI tools table (templated)
```

---

## Section 1: Bootcamp — Page-by-Page Spec

---

### Module 0 — Why This Matters
**File:** `bootcamp/00-why-this-matters.md`  
**Source:** Adapt from Jon's Notion entry "Watch AI Browser Do My Quiz"  
**Read time:** ~5 min  
**Purpose:** Cold open. Makes stakes real before teaching anything. Does not introduce any new concept.

**Content:**

- Open with a plain description of what an agentic AI browser is and what it can do: takes control of keyboard and mouse, completes online forms, navigates web pages, submits work — all triggered by a single typed instruction.
- Describe the demo Jon ran: an AI browser completed a neuroscience quiz (5 open-ended questions about action potentials) in a single session, without login credentials, triggered by the prompt "fill them in." The AI completed and submitted the form correctly.
- One-sentence pivot: this is not a cheating problem with a detection solution — it is an assessment design problem, and this bootcamp is the first step toward addressing it.
- Do not editorialize beyond that. No lengthy analysis here. That belongs in Section 2.

**No hands-on activity in this module.**

---

### Module 1 — Getting Started
**File:** `bootcamp/01-getting-started.md`  
**Source:** Adapt from Notion entry "How to Get Started with AI" (page 2ca469e3)  
**Read time:** ~10 min  
**Purpose:** Framing and permission to just start. Reduces intimidation. Sets up the rest of the bootcamp.

**Content:**

Keep from source:
- The "just start asking" framing — treat AI like a search that talks back
- The four example prompts (hey Copilot why is the Start Menu in the middle... / how do I export the event log in D2L... / here's a file, how do I make it... / I don't know what I want but here's an assignment, ask me questions)
- The "steal these phrases" intro — forward-link to Module 3

Cut from source:
- The per-platform comparison table — move to `reference/ai-tools.md` (see below)
- The personality screenshots (ChatGPT, Claude, Copilot) — dated, specific to a moment

Add:
- Two sentences framing Boodlebox as the institutional tool they'll use. "For this pilot, Boodlebox is your primary tool. The principles you learn here apply directly — the underlying model is the same one we'll work with throughout."
- A faculty note callout: "If you already use ChatGPT or Claude personally, keep doing that. Nothing in this bootcamp requires you to switch. Boodlebox matters most for what you deploy to students."

---

### Reference Sidebar — AI Tools at a Glance
**File:** `reference/ai-tools.md`  
**Source:** Extracted from "How to Get Started with AI" — do not copy directly, rewrite as a clean table  
**Purpose:** Quick reference. Explicitly dated. Separate from module prose so it can be updated without touching modules.

**Content:**

A simple table: ChatGPT / Claude / Gemini / Copilot — columns: Free tier access, Paid tier name and cost, Strengths for faculty use.

Add a visible "Last updated: [Month Year]" line at the top.

Add a one-sentence note: "Model names and pricing change frequently. If something here looks wrong, it probably is — check the provider's website."

**Implementation note for Code:** Consider storing the table data in a separate YAML or JSON file so Jon can update tool info without editing the page template. Up to Code's judgment on whether that's worth the complexity for a static site.

---

### Module 2 — How AI Actually Works (Enough to Matter)
**File:** `bootcamp/02-how-ai-works.md`  
**Source:** Adapt from student Notion page "How AI Memory Actually Works: Context, Errors & Starting Fresh" (page 36f469e3-ddfd-8028)  
**Read time:** ~10 min  
**Purpose:** The one module that does real conceptual work. Establishes the mental models that make everything else make sense.

**Source page is nearly faculty-ready.** The student page is well-written and the core concepts are identical. Primary edits are framing and forward-links.

Keep from source:
- Context window as working memory — everything in the current conversation, nothing outside it
- Why long conversations degrade (losing the thread, contradictions, vaguer answers)
- The symptom to watch for: "if the AI's answers suddenly feel off — that's the signal"
- Start fresh when things go sideways
- The state-transfer prompt technique (ask AI to package up where you left off before closing a long chat)
- When AI is just wrong even in a fresh chat — push back, ask for reasoning, verify

Adapt from source:
- Swap all references to "study bot" → "course workspace in Boodlebox" with a forward-link to Module 4
- The "Build a Study Bot" links → replace with "see Module 4: Boodlebox"

Add:
- A faculty note callout after the state-transfer prompt: "If you're using Claude directly (not through Boodlebox), Claude Projects serve the same function as a persistent workspace — custom instructions and uploaded materials that carry across every chat in that project."
- Do NOT add the full context window taxonomy from the faculty-facing "Context Windows" page (layered memory levels, API vs consumer product distinctions, agentic AI mechanics). That's too deep for day one. This module covers what a faculty member needs to use AI well, not everything that exists.

---

### Module 3 — Getting Useful, Honest Output
**File:** `bootcamp/03-useful-honest-output.md`  
**Sources:**  
- "How to Write a Good Prompt" (student page 36f469e3-ddfd-80cc)  
- "AI Literacy Basics: Memory, Personality & Honest Feedback" (student page 36f469e3-ddfd-80ad)  
**Read time:** ~20 min including hands-on  
**Purpose:** The highest-ROI module. Combines prompting fundamentals with calibration/personality. Includes the session's first real hands-on activity.

**Content:**

**Part A — Why prompts matter and what goes in them**  
From "How to Write a Good Prompt." Keep the three-element framework (context, specificity, format). Rewrite all examples from student context to faculty context:

| Student version | Faculty version |
|---|---|
| "I'm a student in intro psych..." | "I teach intro psychology at a small liberal arts college..." |
| "Help me study for my exam" | "Help me write a learning objective for this unit" |
| "Give me feedback on this essay" | "Here's a rubric I'm drafting — what's ambiguous?" |
| "Summarize this article for someone with no background" | "Summarize this for a student who just finished week 3 of my course" |

Keep the before/after table format — it works. Just replace the content.

Keep the "when your prompt isn't working, redirect in the same conversation" section — faculty need this reassurance.

**Part B — Sycophancy and calibration**  
From "AI Literacy Basics." Keep:
- The sycophancy explanation (trained on human approval → learned to agree)
- The power phrases ("Ask me questions before starting," "What do you think I'm asking?," "What am I not considering?," "Give me confidence ratings," "Push back on me")
- The "confidence ≠ correct" rule of thumb

Adapt:
- Reframe the custom instructions template for faculty context: "I teach undergraduates at a small liberal arts college. I prioritize conceptual understanding. Be direct. If I'm overclaiming, tell me. Flag uncertainty explicitly."
- Add the personality/role technique from Jon's "Personality? Yes Please." page: faculty can tell the AI to behave as a skeptical reviewer, a grant reviewer, a student who doesn't understand, etc. One short table showing task → useful AI mode (brainstorming → generative, editing → surgical, grant review → adversarial, student feedback → constructive).

**Hands-on activity — do-it-now callout box:**

> **Try this now (5 minutes)**  
> Open your AI tool of choice (Boodlebox, Claude, ChatGPT — whichever you have).  
> Take something real: a learning objective, an assignment prompt, a rubric, even a single slide.  
> Ask a bare prompt first: just describe what you want, no context.  
> Then try again with context + specificity + format specified.  
> We'll share what you noticed in 5 minutes.

This is the moment where literacy through usage begins. Code should style this callout box visually differently from regular content — border, background tint, bold header — so it's unmistakably a stop-and-do-something instruction.

---

### Module 4 — Boodlebox: Building Your Course Workspace
**File:** `bootcamp/04-boodlebox.md`  
**Source:** Jon's Boodlebox documentation (provided separately), plus content plan from this session  
**Read time:** ~20 min including hands-on  
**Purpose:** Hands-on module. Faculty leave with a working bot that has their course context loaded.

**Content:**

**Part 1 — Why Boodlebox**  
Two short paragraphs:
- FERPA-compliant, institution-appropriate, designed for educational use
- Pre-loadable with course materials so context is always there — neither faculty nor students have to paste syllabi into every chat
- The underlying model is the same one from Modules 1–3. Everything you just learned applies directly.

**Part 2 — Building your workspace bot (do-it-now)**

Step-by-step, faculty do this during the session:

1. Open BoodleBox and go to the Bot Garage
2. Select "create a new bot"
3. Name it: use format `[COURSE NUMBER] [PURPOSE]` — e.g., "PSYC 101 Study Coach"
4. Write a short description (one sentence: what this bot is for)
5. Write instructions (3–5 lines is enough to start — see Part 3 for what good instructions look like)
6. Upload your syllabus and one other document (rubric, reading list, assignment prompt)
7. Save and test before sharing

**Do-it-now callout box:**

> **Build your bot now**  
> You'll need: your syllabus (or any course document), 5 minutes.  
> Go to Bot Garage → New Bot. Name it with your course number.  
> Write 3–5 lines of instructions. Upload your syllabus. Save.  
> We'll test it together before you share it with anyone.

**Part 3 — The two-bot demo**

This is a live demonstration by Jon during the bootcamp. Code should render this as a "watch what happens" section with the two instruction sets clearly displayed side by side or sequentially.

**Bot A — minimal instructions:**
> You are a helpful assistant for PSYC 101.

**Bot B — calibrated instructions:**
> You are a study coach for PSYC 101 at Columbia College of Missouri. Your job is to help students understand material, not to do their work for them. Never give a direct answer to a content question without first asking the student what they already think. If a student is wrong, tell them clearly and explain why — do not soften incorrect answers with praise. Prioritize the course syllabus and uploaded materials over your general knowledge. If a student asks about exam policies, grades, or deadlines, direct them to the syllabus.

**Demo question to ask both:** "What do I need to know about memory for the exam?"

Bot A produces a general memory overview. Bot B asks what the student already knows and anchors to course materials.

Add a one-paragraph explanation after the demo: the difference isn't the underlying AI — it's the instructions. The instructions are the bot. This connects back to Module 3 (calibration and personality) — faculty are now applying that concept in a tool they can hand directly to students.

**What makes good instructions:**
- The bot's role and who it's for
- What it should help with
- What it should NOT do (especially: don't complete graded work for students)
- Tone and level of detail
- Any course-specific rules

Include Jon's template from the Boodlebox documentation as a copy-paste starting point:

> You are a helpful AI learning assistant for students in [COURSE NAME]. Your role is to support learning, not replace student work. Help students understand concepts, ask guiding questions, and provide feedback. Do not complete graded assignments for students. When students ask for direct answers, guide them through the reasoning process instead. Use a supportive, clear, and professional tone appropriate for undergraduate students. Align your responses with the course materials and instructions provided. If you are unsure, say so and recommend that students consult the instructor or course materials.

**Part 4 — Sharing with students**

Primary method: post the direct bot link in your LMS (D2L, Canvas, etc.). Tell students what the bot is for and what it can't do for them.

Recommended naming so students can confirm they have the right one: include course number in bot name. If you have multiple sections, include section number.

Students can favorite a bot (three-dot menu → Favorite) so it appears in their sidebar for easy access.

Suggested LMS language faculty can copy:

> Use the course bot linked below to help you review concepts, ask questions, and prepare for assignments. The bot is designed to coach your thinking, not complete graded work for you. Confirm the bot name matches this course before you begin. You are responsible for checking all information and following the course AI use policy.

**⚠️ VERIFY BEFORE PUBLISHING — folder sharing mechanic:**  
The documentation describes two sharing methods (direct bot link and shared course folder) but does not clearly specify whether bots are built inside a shared folder or linked from one. Before this page is finalized, Jon needs to test this in Boodlebox and confirm the actual workflow. Mark this section with a `<!-- TODO: verify Boodlebox folder+bot access flow before publishing -->` comment in the source and leave a visible "[coming soon — verifying access flow]" placeholder in the rendered page.

**Part 5 — What students need to know (one callout box)**

> **Tell students this before they use the bot:**  
> Use the link from your course page — don't search for bots manually.  
> Confirm the bot name matches your course before you start.  
> The bot can make mistakes. You are responsible for checking its responses.  
> The bot cannot complete graded work for you — that's by design.

---

### Module 5 — Verifying What You Get Back
**File:** `bootcamp/05-verifying-output.md`  
**Source:** Student Notion page "Verifying AI Output: How to Fact-Check" (page 36f469e3-ddfd-8038-862a)  
**Read time:** ~10 min  
**Purpose:** Calibrates trust. Gives faculty concrete habits for catching errors before they matter.

**Source page is almost faculty-ready with minimal editing.**

Keep from source:
- The core problem: AI tone doesn't change when it's guessing
- High-risk vs lower-risk content (specific stats and citations vs explanations and definitions)
- "Ask it to show its work" technique
- "Ask for uncertainty" / confidence ratings technique
- Check the source, not just the claim (direct search for citations — AI fabricates them regularly)
- The rule of thumb: "If you'd be embarrassed to be wrong about it — verify it"

Adapt from source:
- Swap "trust your professor's slides" → "trust your own course materials and disciplinary expertise"

Add one faculty-specific callout:
> **Higher stakes for faculty:** Citation fabrication is a bigger risk when you're putting something in a syllabus reading list, a grant narrative, or a conference paper. AI produces fake citations that look completely real. Always search for any citation AI gives you before you use it professionally.

---

### Module 6 — What's Next
**File:** `bootcamp/06-what-next.md`  
**Source:** New write — does not exist yet  
**Read time:** ~5 min  
**Purpose:** Close the session, give one concrete next action, point toward Section 2 without overwhelming.

**Content:**

- One concrete thing to try before the next time faculty meet: use your new Boodlebox bot to answer one question a student actually asked you this week. Note whether its answer was accurate, whether you'd modify the instructions, what you'd upload next.
- A short paragraph previewing Section 2: assessment redesign, the portfolio/mastery method, deciding your own course AI policy. Not required reading before Fall. Worth engaging with before Spring.
- A plain acknowledgment: this bootcamp was the floor. What comes next is developed through using the tools, not through more reading. The pilot is designed for that — you're not expected to be experts before you start.

---

## Section 2: Teaching & Assessment in the AI Era

All pages in this section render as clean stubs on launch day. Title, one-sentence description, "Content coming soon — check back before Fall 2026." No 404s, no broken links.

### Stub pages to create:

**`teaching/index.md`**  
Landing page for the section. Brief intro: why assessment has to change, what this section covers, how it connects to the bootcamp.

**`teaching/why-assessment-has-to-change.md`**  
*Coming:* Short, sharp version of the cold open from Module 0 plus broader context on why traditional assessment design is no longer sufficient.

**`teaching/assessment-redesign.md`**  
*Coming:* Practical approaches to redesigning assessments in the AI era. Will consolidate Jon's three stacked Writing Assignments guides (currently in Notion) into one. Major editing job — source material exists.

**`teaching/portfolio-mastery-method.md`**  
*Coming:* The weekly mastery-check and portfolio method from Jon's Protect/Detect page. **Note: consider whether this page should be access-controlled or clearly marked faculty-only.** It describes AI-resistance mechanics that lose value if students read them.

**`teaching/course-ai-policy.md`**  
*Coming:* Framework for deciding your own course AI policy. Does not exist yet — new write. Faculty equivalent of the student Academic Integrity page.

**`teaching/human-ai-alignment.md`**  
*Coming:* The Human-AI Cognitive Alignment concept (Jon's existing Notion page is nearly ready for this). Optional deeper read. Lower priority than the others.

---

## Source Material Index

Pages to adapt from existing Notion content (fetch by ID if needed):

| Module | Notion page title | Notion page ID |
|---|---|---|
| Module 2 | How AI Memory Actually Works | 36f469e3-ddfd-8028-8707-eae6983c85f4 |
| Module 3 (prompting) | How to Write a Good Prompt | 36f469e3-ddfd-80cc-bad3-d144dd88281d |
| Module 3 (calibration) | AI Literacy Basics: Memory, Personality & Honest Feedback | 36f469e3-ddfd-80ad-91e1-ea9fb163a866 |
| Module 5 | Verifying AI Output: How to Fact-Check | 36f469e3-ddfd-8038-862a-e22aabedd1cd |

Pages to write from scratch (no Notion source):
- Module 0 (cold open)
- Module 4 Part 1 (Boodlebox intro)
- Module 6 (what's next)
- `reference/ai-tools.md` (tools table, templated)
- All Section 2 stubs
- `teaching/course-ai-policy.md` (no source exists)

Pages that exist in Notion but need consolidation before adapting:
- Assessment redesign guide — currently three versions stacked in toggle blocks inside "Writing Assignments with AI" (Notion page 2e0469e3). Needs to be merged into one before Code works with it.

---

## Things to Verify Before Publishing

1. **Boodlebox folder+bot sharing mechanic** — Module 4, Part 4. Jon needs to test whether bots are built inside a shared folder or linked from one. Mark with `<!-- TODO -->` comment in source.

2. **AI tools table accuracy** — `reference/ai-tools.md`. Pricing and tier names change. Verify before first publish and add explicit "last updated" date.

3. **Boodlebox underlying model** — Module 4 Part 1 says "the underlying model is the same one from Modules 1–3." Confirm what model Boodlebox actually uses before this language goes live.

---

## What to Ask Jon Before Starting Build

1. Does the existing repo already have a Jekyll or other static site generator configured, or is it raw HTML/markdown?
2. Is there an existing `_config.yml` or theme in place, or does Code pick the design?
3. Is there a preferred navigation style (sidebar, top nav, breadcrumbs)?
4. Should Section 2 stub pages be visible in the nav from day one, or hidden until content exists?
