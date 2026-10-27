---
name: human-writing-style
description: Use when drafting or rewriting messages in the user's own voice, including requests to sound like me, make wording more natural or less AI-sounding, Slack replies, emails, client updates, and explanations written on the user's behalf.
---

# Human writing style

Write like a thoughtful colleague: conversational, direct, warm, modest, and specific. Preserve the meaning; change the voice, not the facts.

## Compose

1. Identify the recipient, channel, existing thread, confirmed facts, and intended ask. Use supplied context; ask only about a consequential gap.
2. Lead with the useful point in first-person prose: "I pushed up...", "I found...", "I've tested..." Explain what it means for the recipient, then the next step if needed.
3. Connect related thoughts naturally with "and", "but", "so", or "which". Keep each sentence understandable without cramming unrelated mechanisms together. Clarity wins over clever cadence.
4. Return one ready-to-send draft by default, without a style analysis or several alternatives.
5. Output the draft as plain paragraphs with no blockquote (`>`) markers, which a terminal renders as a "|" bar on every line and which then gets copied along with the text. Don't wrap the draft in a code block either. Put a short lead-in line before it if needed, and nothing inside the draft that the user would have to delete before pasting.

## Voice and context

- Use contractions and ordinary words. Mirror the recipient's terminology; explain the plain-language gist before technical evidence.
- Prefer short paragraphs to numbered menus. Use bullets when they genuinely help; keep explicit "I" subjects for the user's own work rather than changelog fragments.
- In a continuing DM, start directly or with "Also,". No repeated greeting, @mention, or signature. For a new conversation, use a natural greeting. Email sign-offs depend on context, not a mandatory template.
- Frame requests politely: "Could you...?" Use "I'd be happy to" for an offer. Add a feedback invitation only when useful; don't automatically suggest a meeting.
- Keep natural warmth and genuine uncertainty. Own mistakes briefly. Do not invent enthusiasm, personality traits, promises, or repeated apologies.
- No em dashes. Use commas, conjunctions, sentence breaks, or an occasional spaced hyphen. Keep formatting light; avoid unnecessary bold, headings, or backticks in casual messages.
- Cut corporate language, slogans, defensive AI claims, and filler such as "Good news," "Quick update," or "just wanted to let you know". Don't strip meaningful phrases such as "I just want to get it right" mechanically.

## Final check

Preserve names, URLs, dates, intent, ownership, qualifications, and meaningful limitations. A possible vulnerability is not a confirmed incident; tests passing is not production validation; a pushed PR is not merged or deployed. Never invent experience, scope, metrics, or certainty. Flag unsupported claims separately instead of polishing them into facts. Drafting does not authorize sending.

Example, continuing DM:

Also, I pushed up the fix and the tests passed. It still needs to be merged before we can check it in production. Could you take a look when you have a chance?

## Sources and scope

Distilled from `references/style-guide.md`, which holds the long-form voice rules, BAD/GOOD examples, and honesty rules, in this skill's folder. For updates or nuances, read it. If `references/profile.md` exists, read it for the person's name, sign-off, links, and what they can honestly claim; if `references/corrections.md` exists, read that too. Current user corrections and newer applicable voice guidance take precedence over all of it. This skill is self-contained for routine rewrites.

No job scraping, proposal Q&A pipeline, résumé loading, application tracking, or mandatory model/subagent pipeline. If a filled-in profile is missing, leave out details you don't have (name, links, sign-off) or ask; never put placeholder text such as `[Your Name]` or `yourportfolio.example` into a draft, and never invent facts about the person.
