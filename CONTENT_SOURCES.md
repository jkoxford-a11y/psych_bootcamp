# Content Sources for Code

This file contains the actual source text for modules where the build plan says "adapt from Notion." Code should adapt these verbatim sources per the build plan's editing instructions — not write approximations from the spec summary.

Module 4 (Boodlebox) and Module 0 and Module 6 have no source here — those are original writes per the build plan.

---

## Source A — Module 2
**Notion title:** How AI Memory Actually Works: Context, Errors & Starting Fresh  
**Adapt per:** Build plan Module 2 editing instructions

---

**TL;DR** AI doesn't have unlimited memory. Long conversations degrade. Knowing why — and what to do about it — saves you a lot of frustration.

---

### What Is a Context Window?

Think of a context window as the AI's working memory. It can only "see" what's in the current conversation. Everything outside that window — previous chats, things you told it last week, work from a different session — doesn't exist to it.

That window has a size limit, measured in **tokens**. A token is roughly a word. Every message you send, and every response you receive, uses tokens from that budget. When the budget runs low, performance degrades — the AI starts losing track of earlier parts of the conversation.

**The practical version:** Long chats tend to go worse than short ones. That's not random.

---

### Why AI Makes Mistakes in Long Conversations

As a conversation gets longer, a few things tend to happen:

- The AI starts forgetting constraints or instructions you set early on
- It contradicts things it said earlier
- Answers get vaguer or less accurate
- It may "drift" away from the specific task you established

When this happens, students often assume the AI is just bad at the topic. Usually the real cause is a full or nearly-full context window. It's not getting dumber — it's losing the thread.

**Symptom to watch for:** If the AI's answers suddenly feel off, inconsistent, or like it forgot what you were doing — that's the signal.

---

### What To Do About It

#### Start Fresh When Things Go Sideways

The simplest fix is also the most counterintuitive: stop, open a new chat, and start over. Don't keep pushing a degraded conversation hoping it improves. A fresh context window means a fresh slate — and usually better answers.

#### Save Your Context Before You Do

Before you close a long chat, ask the AI to package up what you accomplished:

> *"Summarize this conversation: what we were working on, decisions we made, and where we left off. Make it detailed enough that I can paste it into a new chat and pick up without losing anything."*

Then paste that summary at the start of your next chat. You've effectively transferred the session.

#### Use a Course Workspace for Ongoing Work

The deeper fix: if you're constantly re-explaining your course, your assignment, or your expectations — that's a sign you need a workspace pre-loaded with that context. That way it's there from the first message of every chat. [→ See Module 4: Boodlebox]

---

### When AI Is Just Wrong (Not Degraded)

Context window issues explain *some* AI errors — but not all of them. AI can also simply be wrong, even in a fresh chat at the start of a conversation.

**What to do:**

- Push back directly: *"I think that might be incorrect — can you double-check?"* AI will often self-correct when challenged
- Ask it to explain its reasoning — errors often surface when the AI has to show its work
- For anything that actually matters (a fact, a citation, a specific claim), verify it yourself

AI sounds confident whether it's right or wrong. That tone is not a reliability signal. See Module 5: Verifying What You Get Back.

---

## Source B — Module 3 (Part A: Prompting)
**Notion title:** How to Write a Good Prompt  
**Adapt per:** Build plan Module 3 Part A editing instructions — rewrite all examples from student context to faculty context

---

**TL;DR** Vague in, vague out. The single biggest upgrade most users can make isn't a better AI tool — it's a better first message.

---

### Why Prompts Matter

AI will always give you *something*. The problem is that a vague prompt gets a generic, averaged-out response — technically an answer, but probably not useful for your specific situation.

The fix isn't complicated. You don't need to learn "prompt engineering." You need to give the AI what any person would need to actually help you.

---

### The Three Things Every Good Prompt Has

**1. Context — who you are and what you're doing**

> ❌ "Explain confirmation bias."  
> ✅ "I'm a student in an intro psychology course. We just covered confirmation bias. Explain it in a way that would help me apply it to a real example I could use on an exam."

**2. Specificity — what you actually want**

> ❌ "Help me with my essay."  
> ✅ "Here's my thesis paragraph. Tell me what's weak about the argument, not what's good."

**3. Format — how you want the answer**

> ❌ *(nothing)*  
> ✅ "Give me a bulleted summary, not a wall of text." / "Explain it like I have no background in this." / "Keep it under 150 words."

You don't need all three every time. But the more specific you are, the less work you have to do afterward.

---

### Before/After Examples

| Weak Prompt | Stronger Version |
|---|---|
| "What is the hippocampus?" | "What does the hippocampus do, and what happens when it's damaged? Use a concrete example." |
| "Give me feedback on this." | "What's the weakest part of this argument? Don't tell me what's good." |
| "Help me study for my exam." | "Quiz me on the key concepts from this list. Ask one question at a time and wait for my answer." |
| "Summarize this article." | "Summarize this article in 3 bullet points written for someone with no background in psychology." |

*(When adapting: replace these four examples with faculty equivalents. See build plan Module 3 table for the faculty versions.)*

---

### When Your Prompt Isn't Working

If the response feels generic, off-target, or too long/short — don't start over. Just correct it in the same conversation:

- *"That's not what I meant. What I'm actually asking is..."*
- *"Too long. Give me the same answer in two sentences."*
- *"You're assuming I have background in this — I don't. Start simpler."*

The AI is not offended. Redirect it.

---

## Source C — Module 3 (Part B: Calibration and Sycophancy)
**Notion title:** AI Literacy Basics: Memory, Personality & Honest Feedback  
**Adapt per:** Build plan Module 3 Part B editing instructions — reframe custom instructions template for faculty context

---

**TL;DR** Out of the box, AI is designed to agree with you. That makes it *feel* helpful but actually makes it less useful. A few small changes fix this — and the difference is significant.

---

### Why AI Agrees With You (Even When You're Wrong)

AI models are trained using human feedback — responses rated as helpful and pleasant got reinforced. The side effect: AI learned that agreeing, validating, and sounding confident gets good ratings.

**What this looks like in practice:**

- You share a weak argument → AI says "great point, and also..."
- You write a flawed essay → AI gives three compliments and one gentle suggestion
- You state something incorrect → AI often goes along rather than correcting you

This is called **sycophancy**, and it's why users who interact with AI carelessly sometimes get *worse* feedback than users who are intentional about it. The fix isn't a different tool — it's knowing how to ask.

---

### Customizing Your AI: The Setup That Changes Everything

Most AI tools let you set persistent instructions that shape every conversation. This is where you fix the sycophancy problem before it starts.

Ask your AI: *"How do I set up custom instructions or a system prompt?"* — steps differ by platform but the concept is universal.

**A starter template you can copy:**

> *"Be direct and concise. If I'm wrong, tell me clearly. Don't pad responses with compliments. Ask clarifying questions when my prompt is vague. Don't fill in gaps with assumptions — flag them instead. Prioritize accuracy over making me feel good."*

*(When adapting for faculty: add the faculty-specific context per build plan — "I teach undergraduates at a small liberal arts college..." etc.)*

---

### Power Phrases — Steal These

These work because they force the AI out of its agree-by-default mode.

> **"Ask me questions before starting."**  
> Stops the AI from charging ahead with assumptions. Gets you a better result on the first real exchange.

> **"What do you think I'm asking?"**  
> Surfaces whether the AI understood you — often reveals a mismatch before it wastes your time.

> **"What am I not considering?"**  
> Directly counteracts sycophancy. Forces the AI to look for gaps rather than validate what's there.

> **"Give me confidence ratings. What are you most and least certain about?"**  
> Critical for any factual question. AI sounds confident even when guessing — this makes uncertainty visible.

> **"What assumptions are you making?"**  
> Especially useful for complex or ambiguous tasks. You may not share those assumptions.

> **"Let's iterate. I don't really know what I want. What is possible?"**  
> Permission to explore rather than over-specify. The best results often come from the third or fourth exchange, not the first.

> **"Push back on me."**  
> Blunt and effective. Tells the AI to stop agreeing and start stress-testing.

---

### Confidence ≠ Correct

AI writes fluently regardless of whether it's right. There's no built-in signal that says *"I'm guessing here."*

**Rule of thumb:** Concepts and explanations are usually solid. Specific facts, citations, dates, and names are where errors hide. If it matters, verify it.

---

## Source D — Module 5
**Notion title:** Verifying AI Output: How to Fact-Check  
**Adapt per:** Build plan Module 5 editing instructions — swap "professor's slides" for "your own course materials," add faculty callout on citations

---

**TL;DR** AI sounds authoritative whether it's right or wrong. A few habits protect you from confidently using something incorrect.

---

### The Core Problem

AI generates text that *reads* like it comes from a confident, knowledgeable source. The tone doesn't change when it's guessing. There's no asterisk that says "I'm not sure about this one."

This isn't a flaw someone forgot to fix — it's how the technology works. The output is a statistically plausible continuation of your prompt, not a lookup from a verified database. That's why AI can produce a convincing-sounding citation that doesn't exist, or state a specific statistic that's slightly wrong, in the same fluent tone it uses for things it gets exactly right.

---

### What AI Gets Wrong Most Often

**High risk — always verify:**
- Specific statistics and numbers
- Citations, author names, publication dates
- Very recent events (AI knowledge has a cutoff date)
- Anything highly specific and checkable

**Lower risk — usually reliable:**
- Explanations of concepts and mechanisms
- Definitions
- Structuring and organizing ideas you provide
- Summarizing material you uploaded yourself

---

### How to Actually Verify

**Ask it to show its work**

> *"Walk me through your reasoning step by step."*

Errors often surface when the AI has to be explicit. A confident wrong answer sometimes falls apart under examination.

**Ask for uncertainty**

> *"What are you least certain about in that response?"*  
> *"Give me confidence ratings on each of these claims."*

Not foolproof, but it surfaces hedges the AI was glossing over.

**Check the source, not just the claim**

If AI gives you a citation — author, journal, year — search for it directly. Don't assume it exists. AI fabricates citations with some regularity, and they look completely real.

**Use your course materials and disciplinary expertise as the standard**

If AI says something that contradicts your textbook, your own field knowledge, or your course's framing of a concept — trust the course materials first. AI draws from the internet broadly; your expertise is the filter.

---

### A Practical Rule of Thumb

> If you'd be embarrassed to be wrong about it in a meeting or in print — verify it.

Concepts and explanations are usually fine. Specific, checkable facts are where errors hide.
