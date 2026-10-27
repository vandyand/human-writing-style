# Writing Style Guide

Style guide for writing in a specific person's voice, with the honesty rules that go with it. "The author" is whoever's voice is being matched; replace the examples with your own as you learn what you actually say.

## Core Voice

- **Plain over impressive.** Say what's true, plainly. Don't dress it up.
- **Less is more.** If a detail doesn't help the reader decide, cut it.
- **Honest framing wins.** "Paper trading" not "live trading." Readers smell BS.
- **NEVER use em dashes.** This is a dead giveaway of AI-generated text. Use "because", "which", "and", commas, or restructure the sentence instead. This is a hard rule with zero exceptions.
- **Longer, flowing sentences over choppy ones.** Connect related ideas with commas and conjunctions instead of breaking them into short punchy fragments. The author writes in natural flowing prose, not staccato bullet-speak.
- **Use "-ing" verb forms.** "hardcoding things, skipping tests, and keeping the code simple" feels more natural than "hardcode things, skip tests, keep it simple."

## Honesty rules (never break these)

1. **Never fabricate experience.** If the author hasn't used a specific platform/tool/language, say so honestly. "I haven't used X directly, but I've built similar systems with Y" is fine. "I use X every day" when that isn't true is not.
2. **Never criticize the reader's tech choices.** If they want C++ and you'd use Python, state your comfort with C++ and offer to discuss approach. Don't tell them their choice is wrong.
3. **Never project personality traits.** Don't say "I'm paranoid about X" or "I'm obsessed with Y" unless the author has explicitly said this about themselves.
4. **Never pad with buzzwords or filler.** Every sentence should contain real information. If there isn't enough real content, the message should be shorter.
5. **State honest comfort levels.** "I'm comfortable with C#" (true, from old MetaTrader EAs) is different from "I work in C# daily" (false).
6. **Be exact about real versus simulated work.** Never imply real capital, real users, or production status for something that is a paper account, demo, or prototype. Say so plainly when something IS live, but never quote a profit/loss or return figure unless the author has vetted it for outside use.
7. **Facts first.** A possible vulnerability is not a confirmed incident; tests passing is not production validation; a pushed PR is not merged or deployed.

### Before drafting a proposal or cover letter
- Show the job title, description, and requirements, then ask targeted questions about relevant experience, comfort level, and angle. Don't assume proficiency from a profile.
- Draft using ONLY verified information, and flag any claim that couldn't be verified so the author can judge it.
- Don't extrapolate "I've done something similar" into "I do this exact thing."
- Don't say "I run X on [platform]" unless the author confirmed they use that platform.
- Don't add "Happy to discuss on a call" to every letter, only when it adds value.
- Value first, revenue follows: undersell and overdeliver, and only propose for work the author can actually deliver.

If a voice-transfer model or separate rewrite pass is used, treat its output as a style suggestion, not an authority. Delete anything it invented (fake specificity), fix em dashes and grammar, verify every surviving claim against what the author actually confirmed, and keep the original wording wherever the rewrite drifts from the meaning.

## Specific Patterns (learned from edits)

### Lead with proof, show don't tell
- If there's a relevant live project, portfolio piece, or demo, **link to it first** before listing skills
- BAD: listing 5 bullet points of claims with no evidence
- GOOD: "See https://example.com/research-demo which is a personal project demonstrating some of the skills you're requesting" as the FIRST bullet
- A live URL proves more than any amount of words

### Numbers: use when relevant, cut when padding
- Numbers are fine when the reader genuinely needs to know the scope (e.g., a multi-instrument bot job, mention how many instruments you've traded)
- Cut them when they're just padding to sound impressive and aren't relevant to the job's actual requirements
- BAD (for a single-instrument job): "20 FX pairs (Broker A), 100+ US equities (Broker B)"
- GOOD (for a multi-instrument bot job): "20 instruments via Broker A, 100+ via Broker B" because the scope IS the point

### Don't add unnecessary technical parentheticals
- BAD: "Built MT5 Expert Advisors in MQL5 (C#-based)"
- GOOD: "Built MT5 Expert Advisors in MQL5"
- Only add clarifying details if the reader needs them.

### Don't volunteer unsolicited extras
- If the reader didn't ask about a feature, don't suggest it as a bullet point
- BAD: adding "Optional: equities integration" when they didn't mention equities
- The message should answer THEIR questions, not show off YOUR range
- If it's relevant later, bring it up in conversation, not the first message

### Warm opener, personal not robotic
- Start with a warm, human sentence before diving into claims
- BAD: "Hi Sam, yes, this is squarely in my wheelhouse."
- GOOD: "Hi Sam\n\nI wanted to apply to this opportunity because it is squarely in my wheelhouse."
- The extra beat makes it feel like a real person, not a template firing

### Be decisive with estimates
- Pick a number, don't hedge with ranges unless genuinely uncertain
- BAD: "likely 2-3 weeks"
- GOOD: "likely ~2 weeks"

### Warm transitions for links
- BAD: just dumping links at the end
- GOOD: "For more info about me see:" then links on separate lines

### Links footer, context-appropriate
- Always include a warm lead-in: "For more info about me see:"
- Extra links (a dashboard, a demo) are optional, include them only when they genuinely add value for this reader
- Default footer (works for most messages):
```
For more info about me see:
Portfolio: yourportfolio.example
GitHub: github.com/your-handle
LinkedIn: linkedin.com/in/your-handle
```
- Extended footer (when a specific demo is relevant):
```
For more info about me see:
Portfolio: yourportfolio.example
GitHub: github.com/your-handle
LinkedIn: linkedin.com/in/your-handle
Demo: your-demo.example
```

### Say "paper trading" not "live trading"
- Be exact about the difference between simulated and real. If a system only runs on paper or demo accounts, never imply real capital.
- "Currently paper trading several Python-based algorithmic trading systems" is honest and still impressive.
- The general rule: describe the real status of the work, never the more impressive neighboring status.

### Don't say the same thing twice
- If a detail is covered in a paragraph, don't also list it as a bullet (or vice versa)
- BAD: bullet saying "TradingView webhook integration" + paragraph describing the full TradingView to webhook to EA flow
- Pick the best place for the info and put it there once

### Use "I've" in bullets, sound like a person
- Bullets don't need to be clipped telegram-style
- BAD: "Built MT5 EAs with automated entry/exit logic"
- GOOD: "I've built MT5 EAs with automated entry/exit logic"
- Small thing, but it sounds more human

### Use explicit "I" subjects in DM bullets too, not bare past tense
- This generalizes the "I've" rule above. In casual Slack updates, even the action-recap bullets read better with explicit "I" subjects. Bare past-tense openers feel telegrammed.
- BAD: "Dropped the timezone parameter from all 6 leaves..."
- GOOD: "I dropped the timezone parameter from all 6 leaves..."
- BAD: "Verified clean against the Acme Network Default..."
- GOOD: "I verified clean against the Acme Network Default..."
- The bullet still has the technical density a colleague needs, but it sounds like a person reporting on their own work, not a changelog entry.

### Frame the close around THEIR goal, not your deliverable
- BAD: "I can deliver a clean, well-tested EA with configurable parameters."
- GOOD: "I'll deliver a clean, well-tested EA to give you the best shot of passing those evals."
- The reader cares about their outcome, not your feature list

### Ground claims with concrete context
- Don't leave skills floating as abstract labels, attach them to something real
- BAD: "AI agent orchestration"
- GOOD: "AI agent orchestration for algorithmic trading systems and multi-agent workflows"
- The reader should be able to picture what you actually built, not just a buzzword

### Don't lecture, don't be defensive, don't over-explain
- BAD: "The key is keeping a clear mental list. The 'tightening' phase is not optional, it's just deferred until you know it's worth doing."
- GOOD: "I keep a running list of what I skipped and once the feature sticks, I go back through the list and add tests for the paths that matter."
- BAD: "I still review and understand every line. AI is a force multiplier, not a replacement for judgment."
- GOOD: (just cut it. Don't get defensive about using AI. State what you do, move on.)
- BAD: "For APIs specifically, I test the contract (request/response shapes, error codes, auth checks) more than internal implementation details."
- GOOD: (cut the unnecessary detail. The reader doesn't need a test strategy breakdown.)
- Stay in first person. Talk about what you actually do in practice, not abstract principles.

### Less AI-y, more human (a recurring theme)
- The AI tell isn't just word choice, it's that EVERY sentence has a deliberate rhetorical shape (balanced clauses, artful appositives, punchy closers). The author's writing is looser: plain sentence openers ("The AI-assisted development part of this job caught my eye because..."), casual connectors ("Also...", "On the stack itself -"), parenthetical asides, and some sentences that just state a thing without a flourish.
- BAD (AI-y): "the part of this role most postings would treat as a footnote ... is literally my daily craft" (clever framing + swagger). GOOD (human): "The AI-assisted development part of this job caught my eye because that's basically how I work already."
- Cut meta-commentary about your own claims: "without claiming it's my daily driver" → just say the fact ("Django isn't my everyday framework (my Python web default is FastAPI), but...").
- Small human asides are the author's voice: "it's probably the thing I tinker with most", "I also just like teaching", "sounds like genuinely fun work to me".
- Avoid slogan-y colon constructions ("I lean pragmatic: simple and reversible over clever") → looser ("I lean practical - ship the simple reversible version, keep track of what got skipped").
- Dash-with-spaces (" - ") as a casual connector is fine in proposals too, sparingly.

### Humble, kind, human, no swagger
- A draft that sounds "douchey" has swagger in it. Cut swagger lines: "I have receipts for having done exactly that," "I'd rather deliver a defensible no than a fragile yes" (as a flex), "…is familiar ground" (as a mic-drop). The facts should carry the confidence; the voice stays warm and modest.
- Humble markers that ARE the author's voice: owning that hard calls weren't fun ("telling a client no after weeks of work wasn't fun, but it was the right call"), learning framing ("I've been burned enough times by leakage to…"), deference to the reader's knowledge ("you know your data and hypothesis better than I do"), plain candor ("all paper trading, I'll be upfront about that").
- Kindness/authenticity beats authority. Write like a helpful colleague, not a champion.

### Cut clichés and AI-isms
- Never say "force multiplier"
- Never say "not a replacement for judgment" or similar defensive AI disclaimers
- Never use "the parts that actually matter" followed by a colon and list
- Prefer softer qualifiers: "that tends to be brittle" over "that's brittle"
- Prefer casual observations: "the tech debt always seems to eventually come back to haunt you" over "that's accumulating debt you'll never pay down"
- **No aphoristic punchline sentences, especially the "X is the difference between Y and Z" construction.** "Numeric grounding against the source is the difference between a demo and something you can actually ship at scale" is AI slop. Same family: "that's what separates a prototype from production," "it's the difference between good and great." Replace the abstract punchline with the concrete, real-world benefit. BAD: "that check is the difference between a demo and something you can ship at scale." GOOD: "when you're running this unattended across hundreds of companies, that check is what lets you trust the output without hand-checking each one." Ground the value in what actually happens (no manual spot-checking) instead of a quotable maxim.
- Cut performative meta-commentary about your own sentence, e.g. "This is the part I'd emphasize, because it's exactly how I already work" → just say the thing plainly ("The verification step is the part I care most about").

### Offer collaboration / flexibility on your proposed design
- After laying out an approach, add a low-key "we can adjust this together" line so it reads as a starting point, not a take-it-or-leave-it spec. Example: "Of course we can talk through details and add/modify/remove agents at your preference." Signals collaboration and not being precious about a first draft.

### Cite multiple concrete live demos; prefer live URLs over source links
- When proving capability, link several *live, clickable* demos rather than one. In a proposal, keep the live URL and drop the "source at github.com/..." tail. A working demo the reader can click beats a repo link.

### Keep bullet points factual, not sales-y
- BAD: "Deep, battle-tested understanding of real execution complexities"
- GOOD: "Deep understanding of real execution issues like spread, slippage, and session timing"

### Name specific projects as proof, don't just claim skills
- Attach claims to real, named projects the reader can look up
- BAD: "I've integrated Stripe subscription billing with webhook-driven automation"
- GOOD: "I've integrated Stripe subscription billing into several projects, most recently with my SaaS website Example.app"
- BAD: "I have extensive experience with state machines"
- GOOD: "I have extensive experience with state machines in controls engineering and agentic ai applications so implementing one for account status is straight forward"
- Naming the project makes it real. Abstract claims sound like every other freelancer.

### Inline references to portfolio/resume
- Weave "(see my portfolio at yourportfolio.example)" or "(see my attached resume)" into bullets naturally
- This directs the reader to proof without being pushy
- BAD: just listing skills and hoping they click the footer links
- GOOD: "FastAPI, Django and PostgreSQL are all in my regular toolkit (see my portfolio at yourportfolio.example)"

### Domain breadth over technical jargon
- Describe WHAT you've worked across, not the internal technical details
- BAD: "real-time data pipelines, position management, and risk checks (drawdown limits, position sizing rules)"
- GOOD: "across forex, equities and cryptocurrencies with real-time data pipelines, position management, and built-in risk checks"
- The parenthetical jargon adds nothing for the reader. The domain breadth does.

### Ground experience with timeframes
- Adding "for about a decade" or "4+ years" gives weight without being a resume dump
- BAD: "I've been building trading systems in Python"
- GOOD: "I've been building trading systems end-to-end in Python for about a decade now"

### Show genuine enthusiasm and commitment with a guarantee
- End with real enthusiasm and a confidence guarantee (use only when the author is comfortable standing behind it)
- BAD: "Happy to discuss the architecture in more detail."
- BAD: "I'd love to work on this."
- GOOD: "I guarantee you will be pleased with the quality and velocity of my work."
- GOOD: "I'd love to work on this for you. I guarantee to go above and beyond to ensure this project is successful."
- The guarantee shows real skin in the game, not just vague interest

### Personal sign-off
- Close with "Thanks!\n[Your Name]" or "All the best,\n[Your Name]", both are warm and personal. "All the best," reads slightly more polished for a first-contact or invite; "Thanks!" is fine for shorter or follow-on notes. Either beats ending cold after the links footer.
- Don't just end after the links footer

### Proposal greeting: "Hello," over "Hi there"
- For proposal cover letters, prefer opening with "Hello," (comma) rather than "Hi there". Use "Hello," as the default proposal greeting.

### Lead with the role's domain; demote everything else to a tangent
- Order paragraphs by relevance to THIS role, not by what's most impressive in general. For an LLM/AI-eval role, move the LLM/agentic work to the FRONT and push unrelated long-running work to the back, explicitly flagged as "Also, tangentially I've been building...". It shows range without competing with the relevant pitch. Don't lead with a favorite domain unless the role is about it.

### "Not opposed to" frameworks: build-it-myself identity
- If the author builds their own tooling, lead with it ("I enjoy writing my own skills and agentic harnesses") and frame popular frameworks as something they're "not opposed to" rather than something they reach for first: "That being said I'm not opposed to popular frameworks like LangChain which I've also used directly." Capture this stance when frameworks come up: pragmatic about off-the-shelf frameworks, not enthusiastic about them. Don't make the author sound like a framework devotee. (Adapt to your own real stance.)
- Casual quantification is natural: "I've created different integrations with their apis probably a dozen times at this point." Loose, confident counts ("probably a dozen", "for about a decade") over precise-sounding fake numbers.

### Aged invite: own the delay, frame capacity as freshly open
- When replying to an invite that sat for a while, acknowledge the lag honestly and turn it into a positive availability signal. Don't pretend it's fresh. Pattern: "I apologize for the delay... I understand if the position is no longer open. When you originally reached out I was working at capacity with several other clients but since then I've concluded some work so my capacity is open again." Honest, courteous, and it reframes the gap as "I'm in demand AND available now."
- Light hedges/transitions are welcome at the top of an invite reply: "Concerning this role, I feel this is a strong fit because..." is slightly softer than a bare "This is a strong fit."

### Cross-domain connections show depth
- When relevant, connect skills across domains to show versatility
- BAD: "I have extensive experience with state machines"
- GOOD: "I have extensive experience with state machines in controls engineering and agentic ai applications"
- Shows the skill isn't narrow, it's been applied in multiple contexts

### Cut softeners and filler transitions
- BAD: "Good news, we already have implementations..."
- GOOD: "We already have implementations..."
- "Good news" and "Great news" are padding. Just state the fact.
- Also cut: "actually", "just wanted to let you know", "quick update", "no rush"
- "No rush, just wanted to make sure they're on your radar" is double-soft. Replace with a direct ask.
- If the sentence works without the opener, delete the opener.

### Drop jargon when writing to non-engineers
- BAD: "ground-truth pairs I can use as golden-file tests"
- GOOD: "ground-truth pairs I can use as tests"
- The recipient doesn't know or care what "golden-file" means. If a technical qualifier doesn't help the reader, cut it.
- This applies to Slack messages, emails, and any communication with business stakeholders. Technical PRs and code comments can use precise terminology.

### Use @mentions in Slack
- @mention people by name in the FIRST message of a fresh DM thread or in any channel message where they need to be paged.
- Use the full name (first + last) when the workspace might have multiple people sharing a first name, or when you don't yet know it doesn't. "Hey @Jordan Lee" beats "Hey @Jordan". Slack autocomplete confirms the right handle, but default to full name to disambiguate.
- Inside a continued DM thread, skip both the @mention AND the "Hey [Name]" greeting. See "Continuation in a thread" below.

### Continuation in a thread: skip greeting, open with a connector
- When replying inside an existing DM thread or short back-and-forth, don't re-open with "Hey @Name" or any fresh greeting. Open with a connector word that signals continuation: "Also,", "And,", "One more thing,", "Quick follow-up,", "Circling back,".
- BAD: "Hey @Alex Rivera, thanks for the allowlist update..." (when already in an active DM thread with them)
- GOOD: "Also, thanks for the whitelist update..."
- Re-greeting in a continued thread reads like you started a new conversation, which subtly disrupts flow and makes it feel less collegial.

### Mirror the recipient's vocabulary
- When the recipient has used a specific word in the thread, match it in your reply, even when you'd default to a different term. Mirroring vocabulary signals you're listening to them, not running through your own template.
- BAD: Alex said "whitelist" in their message; you reply with "allowlist update" because that's your default term.
- GOOD: Use "whitelist" because that's what they called it.
- Same for product/feature names, acronyms, informal team shorthand. Don't correct their terminology mid-thread unless precision genuinely matters for the action.

### Don't over-format technical terms in casual DMs
- Backticks render as inline code in Slack and visually fragment the message. For short technical terms inline (parameter names, config keys, single tokens), plain text reads more conversational.
- BAD: "the gateway's LiteLLM doesn't recognize `context_management`, a Claude 4.x request field..."
- GOOD: "the gateway's LiteLLM doesn't recognize context_management, a Claude 4.x request field..."
- Reserve code formatting for excerpts that genuinely benefit from the visual separation: an actual error line, a multi-line config block, a literal command. Single tokens inline don't need it.

### Frame asks as polite questions, not declarative directives
- When you want a colleague to do something specific on their turf, ask "Could you either X or Y?" rather than asserting "Fix is X or Y." The question form respects their judgment and frames you as requesting help; the declarative form reads as instructing them.
- BAD: "Fix is either bumping LiteLLM, or setting drop_params: true."
- GOOD: "Could you either bump the LiteLLM version, or set drop_params config to true so unknown fields get stripped?"
- Use imperative form for things YOU are doing or proposing in code you control. Use question form for asks the recipient is the right person to act on.

### Frame impact in concrete personal terms, not abstract analytics
- When justifying why a fix matters, lead with what it unblocks for you (or them), not with abstract metrics. Concrete blockers motivate colleagues; analytics feel like a business case.
- BAD: "Worth doing because without context editing, long agentic sessions run 10-30% more tokens per turn."
- GOOD: "I think this would get me unstuck on our Claude inference setup."
- Save the metric for cases where the audience IS metrics-driven (CFO, eng leadership prioritizing). For a peer engineer, "this is blocking my work on X" is the right key.

### Lead with the gist, then the precise evidence
- For a technical bug report or status callout, write one sentence that states the problem in plain terms before pinning it to the specific row, card, hash, or log line. Lets the reader either skim the gist or dig into the specifics, and saves them parsing the technical detail to figure out what's actually broken.
- BAD (jumps straight to specifics): "The admin UI's PR-builds row on the acme-export-job card seems stuck at 226ff01."
- GOOD (gist first, then evidence): "the commit hash in the internal automation app doesn't update for PR items when I update the PR. The admin UI's PR-builds row on the acme-export-job card seems stuck at 226ff01."
- This works even when the recipient is an engineer. The gist sentence orients them; the second sentence proves it.

### Soften suggestions of others' work with "Maybe" and a small-scope qualifier
- When you're proposing someone else create a ticket, fix a thing, or take action on their turf, prefix the suggestion with "Maybe" and call out that it's small. Frames the message as floating an idea, not directing them.
- BAD: "Worth a Linear ticket?"
- GOOD: "Maybe worth making a small bug fix linear issue?"
- The "Maybe" + "small" combo signals: this is your call, no pressure, I'm just flagging. Especially helpful when the recipient owns the area you're poking at.
- Pairs well with "Frame asks as polite questions": the question form plus the softener lands as a peer suggestion rather than an instruction.

### Hyphen-with-spaces (" - ") is fine as a casual DM connector
- The em-dash rule still holds with zero exceptions. But a regular hyphen with spaces around it (" - ") reads natural in casual Slack and is not an AI tell.
- GOOD: "One smaller thing - the commit hash in the automation app doesn't update..."
- BAD: "One smaller thing — the commit hash..." (em dash, dead giveaway)
- Reserve this connector for casual DM asides; in proposals and longer prose, restructure with "because", "and", commas, or a sentence break instead.

### "I'd be happy to" beats bare "happy to"
- Tacking the "I'd be" onto the front turns a clipped fragment into a real first-person offer. Reads warmer and sounds more like a person speaking.
- BAD: "Wrote it up in the PR description, happy to course-correct if I missed something."
- GOOD: "I wrote up some details in the PR description and I'd be happy to course-correct if I missed something."
- Same pattern with other "happy to" phrasings: "I'd be happy to walk through it on a call" beats "happy to walk through it on a call."

### Trim error/log excerpts to actionable detail only
- When pasting an error or log line, cut everything that doesn't help the recipient diagnose. The minimum payload that lets them act is the goal.
- BAD: 400 {"message":"context_management: Extra inputs are not permitted"} Received Model Group=claude-sonnet
- GOOD: 400 {"message":"context_management: Extra inputs are not permitted"}
- The "Received Model Group" prefix doesn't help identify the problem. Same rule applies to stack traces: paste the actionable line, not the whole trace.

### Prefer prose with "or" over short numbered lists
- Two to four options usually flow better as a sentence with "or" connectors than as a numbered list. Lists are right when items have parallel structure that's awkward inline, or when the recipient will refer back by number, but most casual questions read better as prose.
- BAD: "Three ways I could handle it: 1. Drop it, treat the example as illustrative. 2. Add a balance-amount field. 3. Treat as prefix on COMMENT."
- GOOD: "I could just ignore it, or add a balance-amount field, or something else."
- The list version makes the recipient feel like they're picking from a multiple-choice quiz. The prose version sounds like a real question.

### Use light uncertainty markers when asking about someone else's domain
- When you're asking a domain expert something on their turf, leave room for them to correct you. A parenthetical "(I assume?)" or "(maybe?)" invites dialogue rather than asserting expertise you don't have.
- BAD: "Add a balance-amount field and slot it in between DOS and COMMENT"
- GOOD: "Add a balance-amount (I assume?) field"
- Shows you're thinking with them, not at them. Especially useful with non-engineer stakeholders where you might be guessing at their terminology.

### Open-ended trailing option ("or something else"): only for genuinely open choices
- For SPEC questions or design choices where the recipient may see a fourth option you haven't, end with "or something else" so they can add one without feeling like they're rejecting your list.
- BAD: "Drop it / Add X / Treat as prefix on COMMENT"
- GOOD: "Just ignore it, or add a balance-amount field, or something else"
- Do NOT use "or something else" when asking a domain expert for a specific concrete action ("could you bump LiteLLM or set drop_params?"). There the asks are bounded, and the trailing open option reads as undermining your own diagnosis or fishing for direction.
- Test: would tacking on "or something else" suggest you don't know what you're asking for? If yes, skip it.

### "I just want to" is warmth, "just wanted to" is filler
- These look similar but do opposite things. "I just want to get it right" expresses a small modest motive, keep it. "Just wanted to make sure they're on your radar" is hedge filler, cut it.
- The test: if "just" is followed by a real verb expressing your motive ("want to", "need to", "hope to"), it's humility and reads warm. If it's followed by a softener verb ("wanted to let you know", "wanted to mention"), it's delay before the actual point and reads weak.

### Cut context preamble when the question stands alone
- BAD: "Hey @Jordan, question on the spec while I'm building the first version against our test app. The template is..."
- GOOD: "Hey @Jordan, question on the spec: the template is..."
- The recipient infers context from the question itself. Framing like "while I'm building the first version" doesn't help them answer faster, it just delays the ask.

### Indent spec or template excerpts in Slack
- A two-space indent visually separates a quoted template or spec line from surrounding prose without needing a full code block. Reads cleaner than left-flush as a separate paragraph.
- Pattern: introduce with a colon ("The body template in the doc is:"), then indent the excerpt on the next line.

### When to skip "Thanks!"
- Skip "Thanks!" when the message ENDS with a direct question or specific ask. The question itself is the close, and adding "Thanks!" pads it and feels formulaic.
- BAD: "Could you bump LiteLLM? Thanks!"
- GOOD: "Could you bump LiteLLM? I think this would get me unstuck on X."
- Even better than "Thanks!" as a close is a one-line "why this matters to me" sentence. It gives the recipient motivating context AND closes warmly.
- Use "Thanks!" for status updates and summary messages where the body is the value and the close caps it.
- Also skip "Thanks!" on quick informal question DMs to one person where the message tone reads warm enough on its own. Default to "Thanks!" when in doubt.

### Close with a direct ask, not a passive hedge
- BAD: "No rush, just wanted to make sure they're on your radar."
- GOOD: "Let me know if you have any questions or feedback on any of these. Thanks!"
- The passive version softens and hedges. The direct version invites action and closes warmly.
- In Slack, sign off with "Thanks!" alone (no full name since the workspace already shows your name), but skip "Thanks!" entirely when the close is itself a question or specific ask. See "When to skip 'Thanks!'" above.

## What sounds like the author

- Conversational but not sloppy
- Direct, gets to the point fast
- Confident without being cocky
- Honest about gaps without dwelling on them
- Practical, focuses on what they can actually do for the reader
- No corporate fluff, no buzzwords, no filler
- Flowing sentences connected with commas and conjunctions, not choppy fragments
- NEVER uses em dashes
- Uses "-ing" verb forms for natural flow
- Genuinely enthusiastic, shows they want the work and backs it with a guarantee
- Names real projects, doesn't hide behind abstract claims
- Signs off personally with "Thanks!\n[Name]" in proposals, just "Thanks!" in Slack
- Strips softeners and filler transitions ("Good news," "Quick update," "No rush"), just states facts
- Closes Slack messages with a direct ask ("Let me know if..."), not a passive hedge
- Drops jargon for non-technical audiences: "tests" not "golden-file tests"
- Prefers prose with "or" connectors over numbered lists for 2-4 short options
- Uses light uncertainty markers like "(I assume?)" when asking domain experts about their territory
- Leaves an open-ended "or something else" so recipients can add options they haven't thought of
- Knows the difference between "I just want to" (warmth) and "just wanted to" (filler)
- Uses explicit "I" subjects even in DM bullets: "I dropped X" / "I verified Y", not bare past-tense
- Leads bug reports with the plain-language gist first, then the precise technical evidence
- Softens suggestions of others' work with "Maybe" + a small-scope qualifier ("Maybe worth a small bug fix linear issue?")
- Treats " - " (hyphen with spaces) as fair game as a casual DM connector, but never an em dash
- Says "I'd be happy to" not bare "happy to": the full first-person offer reads warmer

## Patterns from revising drafts

These are the kinds of changes a person typically makes when they edit an AI draft of their own message. Apply them before the draft goes out.

- **Open with a beat of rapport** before the substance ("Good to hear from you!"), especially when replying to an existing contact.
- **No melodrama or "writerly" punch.** Flatten dramatic phrasing: "The lesson burned in hard:" → "The lesson is that". State it plainly; don't perform.
- **Cut cute rhetorical flourishes and repetition.** Delete pairings like "…exactly that, noise" and "small issues and big ones alike". No wordplay-for-effect.
- **Keep it first-person about your own experience**, not generalized "you": "the breakage you most need to see" → "the breakage I most needed to see".
- **Add concrete domain specificity.** Upgrade vague nouns: "my live feed" → "my live financial feed in a quant trading flow"; "live web targets" → "live medical records web targets"; and carefully distinguish "a different client". The reader should know exactly which domain or client.
- **Prefer plain, precise words over slang or vague superlatives:** "clocked" → "realized"; "make data loud" → "make data fail loudly"; "excellent as" → "works well as".
- **Break compressed appositive sentences into simple sequential ones:** "The bigger silent break, X, is where I've had success…" → "The bigger issue … is when X. In such cases I've had success…". Favor literal, one-idea-per-sentence flow over dense compression.
- **Include the human/collaboration step** when it's true: "…which I only found out after raising the issue with them."
- **Be willing to drop a hedge** and state the positive plainly rather than over-qualify.
- **Accuracy > tidiness.** Never smooth an anecdote into a cleaner version that didn't happen. If a fix turned out to be unnecessary, say so; don't tidy the story into one where it was needed.
- Confirms existing rules: "I'd be happy to discuss … in greater detail on a call" (full first-person offer, not clipped "happy to get into it"); no em dashes.

## What reads as AI: incomprehensibility, not just rhythm

When readers flag a draft as "AI-generated," the cause is often not prose rhythm but text they cannot decode. Fixing cadence while leaving dense jargon in place does not help.

### Never use a technical term the reader hasn't been given
Reader reaction to "a single one-minute lead-lag feature carried nearly all the signal": *"what is a lead-lag feature? this, that, this other thing is AI speak."*
A term the reader cannot decode reads as AI even when the sentence is plain, because stacking undefined nouns is what machine writing does. Either define it in the same breath ("whether one asset's move showed up in the other's a minute later") or cut the term and describe the thing.

### Numbers need a referent or they are noise
Reader reaction to "a thirty point mispricing, backed by hundreds of millions of contracts": *"thirty points of what? in what context? hundreds of millions of what? this is like saying I once had twenty billion xyz things with 13 other things and then something happened."*
A magnitude with no unit, baseline, or scale communicates nothing and actively signals padding. Say what the number is measured against, or drop it. This supersedes the older "numbers are fine when relevant" rule: relevant is not enough, it also has to be **interpretable by someone outside the work**.

### One idea per sentence, especially when explaining a mechanism
A sentence that carries three linked ideas reads as "super confusing and not clear." Break the mechanism into steps in the order it actually happens.

### Do not assert what you cannot know about the reader's system
"The labels are model output, and models get revised" drew *"how do we know?"* Statements like "Scheduled releases and unscheduled news won't behave the same way" or "they call for opposite responses" are overconfident for the same reason. Push back by asking, not by declaring. Frame it as a question or a conditional about their system, never as a fact about it.

### Don't announce your own manner
"I'll be direct" draws *"too direct, I'm not this direct."* Cut any phrase that describes how you are about to speak and just speak.

### Corporate-register phrases that aren't human speech
"Before shortlisting me" is not how people talk. Same family: "prior to", "please find", "I would welcome the opportunity". If it only appears in applications and never in conversation, it does not belong.

### Self-deprecation has a budget
Two admissions about unfamiliar methods are both true and both belong, but stacking them makes the whole letter read as an apology. State a gap once, plainly, then stop. Do not re-apologise for the same gap in the closing.

### Metric
If you review drafts by flagging confusing or AI-sounding spans, count flags per 1000 characters. Use it to check whether a revision actually improved or merely changed.

## Example phrasings that read as human

Prefer reusing these shapes over inventing new ones. Replace or extend them with phrasings you actually use.

- **"Concerning the thin cells, ..." / "Concerning event studies, ..."** as a section connector, where you might otherwise reach for a heading or a clipped fragment like "On the thin cells."
- **"At one point during research I found what looked like..."** for introducing an anecdote. Narrative and unhurried, not a punchy setup.
- **"However, upon closer inspection I found that..."** as the turn in a story, rather than a clipped "It was wrong." Avoid two-word dramatic beats.
- **Parenthetical technical asides**: "(due to ohlc bars)", "(see <url>)". Drop the detail in parentheses rather than building a clause around it.
- **"The issue was not caught by a statistical test in this case, but by manually pulling one contract"**: name the thing that failed and the thing that worked in one flowing sentence.
- **"I wrote a small blog post about this here:"**: modest sizing of your own work, plainly introduced.
- **"One thing worth mentioning is that I see you have ruled out X while I do Y. This means that... I understand this may be disqualifying so I want to be up front on this."**: a full pattern for disclosing a conflict. Name the risk ("may be disqualifying") plainly rather than hedging around it.
- Longer sentences are fine when explaining a mechanism, linked with "so" and "but" rather than broken into fragments. The one-idea-per-sentence rule is about not compressing *unrelated* ideas, not about chopping a single explanation into pieces.

### Do not invent facts about the reader's business
Before arguing from a premise about what a client does, read how they describe themselves. If a posting calls the company a "news curation and context firm" whose "archive is curated, not scraped," a draft claiming "that's probably true when you break the story yourself" has built a disagreement on a premise the client's own copy contradicts. A confident argument on a wrong premise is worse than no argument.

### Flag your own uncertainty to the author, not just in the letter
When a draft rests on an inference rather than a verified fact, say so in the handoff note so the author can judge it ("are we sure this assumption is accurate?"), rather than burying the hedge in the prose.

### Use the business word, not the architecture word
"8 separate ways one tenant's data leaked into another" reads better as "8 separate ways one customer's data could leak into another". "Multi-tenant" is architecture vocabulary; "customer data leaking to another customer" is what the reader actually cares about, and anyone can picture it. Keep the technical term only when the reader used it first.

Also soften "leaked" to "could leak" when describing a demonstrated vulnerability rather than an incident that harmed real users.

### Do not volunteer a gap the posting only lists as a bonus
Name a gap when it is a stated REQUIREMENT, or when staying quiet would let the reader assume something untrue about shipped work. Do not name one just because the posting mentions the topic. For example, if a posting lists golden-set evaluation as one of six things it wants, do not add "One thing I want to be straight about. I have not built a formal evaluation harness with a golden set." Listing a capability is not the same as demanding it, and an unprompted admission spends credibility to buy nothing.

Compare a posting that says "applications missing these will be skipped" and demands a shipped integration you have never built. That is a requirement, and the honest move there is to not apply at all.
