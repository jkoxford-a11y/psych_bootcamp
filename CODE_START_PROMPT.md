# Claude Code — Start Prompt

Paste this as your first message to Code.

---

Read `BOOTCAMP_BUILD_PLAN.md` and `CONTENT_SOURCES.md` before writing anything. Both are in the repo root.

`BOOTCAMP_BUILD_PLAN.md` is the full spec — site structure, every module, design constraints, and what to write from scratch vs. adapt.

`CONTENT_SOURCES.md` contains the actual source text for Modules 2, 3, and 5. Use it. Don't approximate from the build plan summary — the real text is right there.

Before you start the build, confirm you've read both files and tell me:
1. The Jekyll/GitHub Pages setup you see in the existing repo (theme, config, anything already in place)
2. Your plan for the callout include syntax — see the technical note below before you decide

---

## Technical notes (read before building)

**Site title:** "AI Literacy — Psychology AI Integration Pilot"  
No favicon needed for now.

**Callout include syntax — important:**  
The `{% include callout.html content="..." %}` inline approach breaks when content has multiple steps or a list. Module 3's hands-on activity and Module 4's bot-building activity both have multi-line content. Use a `capture` block approach instead:

```liquid
{% capture do_it_now %}
Your multi-line content here.

- Step one
- Step two
{% endcapture %}
{% include callout-do-it-now.html content=do_it_now %}
```

Design the include component to accept content this way from the start.

**Module 4 is original writing:**  
There is no Notion source for the Boodlebox module. Write it entirely from the build plan spec. Plan to flag it for careful review before publish.

**Module 4 sharing mechanic:**  
The build plan flags one paragraph in Module 4 Part 4 (folder+bot sharing) as unverified. Mark it with a `<!-- TODO: verify Boodlebox folder+bot access flow before publishing -->` comment in the source and render a visible placeholder in the page: "Access method coming — verifying with Boodlebox before publishing."

**Section 2 stubs:**  
All five Section 2 pages render as clean stubs on day one — title, one-sentence description, "Content coming soon — check back before Fall 2026." Visible in navigation from launch. No broken links, no 404s.

**AI tools data file:**  
Build `_data/ai-tools.yml` as planned. The reference page reads from it with Liquid. Jon updates the YAML file to refresh tool info without touching the page. Add a visible "Last updated: June 2026" field in the YAML that renders on the page.

---

## Build order suggestion

1. Jekyll config + layouts + CSS + includes (scaffold first, no content)
2. Landing page + bootcamp index
3. Modules 0, 1 (original writes — no source file)
4. Modules 2, 3, 5 (adapt from `CONTENT_SOURCES.md`)
5. Module 4 (original write — flag for review)
6. Module 6 (original write — short)
7. Section 2 stubs
8. Reference page + ai-tools.yml

Stop after step 1 and show me the layout before writing any content. I want to confirm the navigation and visual treatment before content goes in.
