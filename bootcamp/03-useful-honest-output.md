---
layout: module
title: "Module 3: Getting Useful, Honest Output"
permalink: /bootcamp/03-useful-honest-output/
tldr: "Vague in, vague out — and out of the box, AI is designed to agree with you. Two fixes: give it real context, and tell it to push back. This module covers both."
prev_url: /bootcamp/02-how-ai-works/
prev_title: "Module 2: How AI Actually Works"
next_url: /bootcamp/04-boodlebox/
next_title: "Module 4: Boodlebox"
---

# Module 3: Getting Useful, Honest Output

---

## Part A: Why Prompts Matter and What Goes in Them

### Why Prompts Matter

AI will always give you *something*. The problem is that a vague prompt gets a generic, averaged-out response — technically an answer, but probably not useful for your specific situation.

The fix is not complicated. You don't need to learn "prompt engineering." You need to give the AI what any person would need to actually help you.

### The Three Things Every Good Prompt Has

**1. Context — who you are and what you're doing**

> ❌ "Write a learning objective."  
> ✅ "I teach intro psychology at a small liberal arts college. Help me write a learning objective for a unit on memory — measurable, appropriate for a 100-level course, week 4 of the semester."

**2. Specificity — what you actually want**

> ❌ "Help me with this rubric."  
> ✅ "Here's a rubric I'm drafting — what's ambiguous? What would a student interpret differently than I intended?"

**3. Format — how you want the answer**

> ❌ *(nothing)*  
> ✅ "Give me a bulleted list, not prose." / "Keep it under 150 words." / "Write it in language appropriate for undergraduates."

You don't need all three every time. But the more specific you are, the less work you have to do afterward.

### Before/After Examples

| Weak Prompt | Stronger Version |
|---|---|
| "Write a learning objective." | "I teach intro psychology at a small liberal arts college. Help me write a learning objective for a unit on memory. It should be measurable and appropriate for a 100-level course." |
| "Give me feedback on this." | "Here's a rubric I'm drafting — what's ambiguous about the criteria? What would a student interpret differently than I intended?" |
| "Help me with this assignment." | "Help me write a learning objective for this unit. Focus on what students should be able to *do*, not just what they should know." |
| "Summarize this article." | "Summarize this article for a student who just finished week 3 of my intro psych course — no assumed prior knowledge beyond what's covered in weeks 1–3." |

### When Your Prompt Isn't Working

If the response feels generic, off-target, or too long — don't start over. Redirect in the same conversation:

- *"That's not what I meant. What I'm actually asking is..."*
- *"Too long. Give me the same answer in two sentences."*
- *"You're assuming I have background in this — I don't. Start simpler."*

The AI is not offended. Redirect it.

{% capture do_it_now %}
Open your AI tool of choice — Boodlebox, Claude, or ChatGPT, whichever you have in front of you.

Take something real: a learning objective, an assignment prompt, a rubric, even a single slide.

Try a bare prompt first — just describe what you want, no context.

Then try again with context + specificity + format specified.

We'll share what you noticed in 5 minutes.
{% endcapture %}
{% include callout-do-it-now.html content=do_it_now %}

---

## Part B: Getting Honest Feedback

### Why AI Agrees With You (Even When You're Wrong)

AI models are trained using human feedback — responses rated as helpful and pleasant got reinforced. The side effect: AI learned that agreeing, validating, and sounding confident gets good ratings.

**What this looks like in practice:**

- You share a weak argument → AI says "great point, and also..."
- You draft a flawed rubric → AI gives three compliments and one gentle suggestion
- You state something incorrect → AI often goes along rather than correcting you

This is called **sycophancy**, and it's why users who interact with AI carelessly sometimes get *worse* feedback than users who are intentional about it. The fix isn't a different tool — it's knowing how to ask.

### Set Up Your AI So It Doesn't Default to Agreement

Most AI tools let you set persistent instructions that shape every conversation. This is where you fix the sycophancy problem before it starts.

Ask your AI: *"How do I set up custom instructions?"* — steps differ by platform but the concept is universal.

**A starting template for faculty:**

> *"I teach undergraduates at a small liberal arts college. I prioritize conceptual understanding over coverage. Be direct and concise. If I'm wrong or overclaiming, tell me clearly. Don't pad responses with compliments. Ask clarifying questions when my prompt is vague. Flag uncertainty explicitly rather than glossing over it."*

### Power Phrases — Steal These

These work because they push the AI out of its agree-by-default mode.

> **"Ask me questions before starting."**  
> Stops the AI from charging ahead with assumptions. Gets you a better result on the first real exchange.

> **"What do you think I'm asking?"**  
> Surfaces whether the AI understood you — often reveals a mismatch before it wastes your time.

> **"What am I not considering?"**  
> Directly counteracts sycophancy. Forces the AI to look for gaps rather than validate what's already there.

> **"Give me confidence ratings. What are you most and least certain about?"**  
> Critical for any factual question. AI sounds confident even when guessing — this makes uncertainty visible.

> **"What assumptions are you making?"**  
> Useful for complex or ambiguous tasks. You may not share those assumptions.

> **"Let's iterate. I don't really know what I want. What is possible?"**  
> Permission to explore rather than over-specify. The best results often come from the third or fourth exchange, not the first.

> **"Push back on me."**  
> Blunt and effective. Tells the AI to stop agreeing and start stress-testing.

### Confidence Does Not Equal Correct

AI writes fluently regardless of whether it's right. There's no built-in signal that says *"I'm guessing here."*

**Rule of thumb:** Concepts and explanations are usually solid. Specific facts, citations, dates, and numbers are where errors hide. If it matters, verify it.

### Using AI in a Role

Tell the AI to behave as a specific type of reviewer. The same task gets very different output depending on the mode you set.

| Task | Useful AI mode |
|---|---|
| Brainstorming assignment ideas | Generative — "Give me ten variations, don't filter" |
| Editing a rubric | Surgical — "What's unclear? What's ambiguous? Be specific." |
| Reviewing a grant narrative | Adversarial — "You are a skeptical reviewer. What's weak?" |
| Giving feedback on student work samples | Constructive — "Point out what's missing without being discouraging" |

You set the mode. The AI will follow it.
