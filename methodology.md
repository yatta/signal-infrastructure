# Building a Signal Infrastructure — A Methodology
**A guide for Claude to help a person design their own AI-assisted sensemaking system.**

## How to use this file

This file is meant to be given to Claude (in a Project, in Code, or in Cowork) as a methodology guide. Claude should use it to walk the person through designing a signal infrastructure that fits their actual work, context, and risk profile — not to prescribe a specific toolstack or architecture.

Claude should treat this as a collaborative design process. Ask questions. Let the person's answers shape the system. Don't assume their sector, org structure, threat model, or technical comfort level.

---

## The approach

This methodology prioritizes **attention before access**. Rather than starting with what tools an AI agent can connect to, it starts with how the person already detects and processes signal as a human — then looks for where AI can extend that capacity without replacing the judgment that makes it work.

The sequence:
1. Map how you actually process signal today
2. Identify where synthesis is the bottleneck (not access)
3. Build a curated reading layer for public signals
4. Add internal signal capture deliberately, with clear scope
5. Define specific analysis modes rather than general scanning
6. Close the feedback loop so human judgment compounds

---

## Step 1: Map your existing signal practice

Before designing anything, spend time with the person understanding how they actually stay informed right now. This is the foundational step — everything else builds on it.

**Claude should ask the person to walk through a typical day or week:**
- When do you first encounter information that matters to your work? What does that look like?
- What are you reading, scanning, or checking? In what order?
- Where do you encounter things by accident vs. on purpose?
- When something catches your attention, what do you do with it? Forward it? Save it? Sit with it?
- How do you know when something is signal vs. noise? What's the internal heuristic?
- If you work with others, how do signals move between people? Slack? Conversation? A shared doc?

**What Claude is listening for:**
- The difference between passive intake (feeds, newsletters, ambient scanning) and active investigation (following a thread, going deep on a topic)
- The moments where the person makes a judgment call — "this matters" or "this connects to X" — because those are the intelligence moves that can't be automated
- The places where things fall through the cracks — not because the person missed them, but because there's no system to hold them

**Don't rush past this step.** The person's existing practice is the design spec. A system that doesn't match how they actually think will be abandoned.

---

## Step 2: Identify the real bottleneck

The instinct is usually "I need to see more." The actual problem is almost always "I can't synthesize what I already see."

**Claude should help the person distinguish between:**
- **Access problems** — "I don't know what's happening in [domain]" → needs better sources, not AI
- **Volume problems** — "I see too much and can't process it all" → needs filtering and synthesis, AI can help
- **Connection problems** — "I notice things but can't see how they relate" → needs pattern-surfacing, AI can help
- **Retention problems** — "I read something last month that's relevant now but I can't find it" → needs a capture system, AI can help
- **Distribution problems** — "I notice things my team/org should know about but there's no mechanism" → needs a sharing infrastructure

Each of these has a different solution. Don't design a system until the bottleneck is clear.

---

## Step 3: Build a curated reading layer

Start with public signals. No internal system access required, no security implications, immediate value.

**The principle:** the person selects the sources. AI synthesizes across them. The person reviews the output. Human judgment on both ends.

**Claude should help the person:**
- Identify 15-50 sources worth following consistently (these will vary wildly by domain — could be RSS feeds, specific subreddits, government registers, academic preprint servers, industry mailing lists, specialized newsletters, social media accounts, regulatory filings, anything)
- Choose a reading tool that fits their workflow (RSS reader, email aggregation, bookmark system, whatever they'll actually use)
- Design a synthesis cadence — daily, weekly, or triggered by volume. What format should the output take? A file? A message? A briefing? Let the person's work rhythm determine this.
- Define what "interesting" means for their context. This is the hardest and most important part. "Flag things related to X, Y, Z" is more useful than "flag anything important."

**What Claude should not do:**
- Assume the person wants or needs a specific tool (Miniflux, Feedly, Notion, etc.)
- Assume the person's signal sources are standard tech/business feeds
- Prescribe a cadence without understanding the person's actual rhythm

---

## Step 4: Add internal signal capture deliberately

If the person works with others, there's likely valuable signal in their internal communications — links people share, reactions to events, informal analysis. The question is how to capture this without creating a surveillance system.

**Key distinction Claude should help the person think through:**

- **Opt-in channels** — a designated space where people share things knowing it feeds the system (low risk, high signal, requires buy-in)
- **Existing channels, read-only** — scanning what people already share in a specific context (medium risk, depends on norms and consent)
- **Broad access** — reading across all internal comms (high risk, significant security and trust implications, almost never the right first move)

**Claude should ask:**
- What's the trust environment? Are people comfortable with AI reading their work conversations?
- What's the security profile? What would it mean if this data were exposed?
- Is there a specific channel or space where signal naturally concentrates?
- What's the difference between what people share publicly and what they discuss internally? Is the internal layer actually where the high-value signal lives, or is it operational?

**The recommendation is almost always:** start with a designated opt-in channel or a narrow read of a specific existing space. Expand only after the value is proven and the norms are established.

---

## Step 5: Define specific analysis modes

"Scan everything and tell me what matters" produces noise. Specific, named analysis modes produce useful output.

**Claude should help the person design 2-4 report types that match their actual questions.** These will be domain-specific and should emerge from the Step 1 conversation. Examples across different contexts:

- Someone working in a regulated or fast-moving technical field might want: literature and preprint scanning, regulatory or policy change tracking, funding or investment landscape shifts
- A consultancy or agency might want: client industry signals, methodology/tool evolution, project-relevant cultural shifts
- Someone in a policy or governance role might want: legislative tracking, stakeholder position mapping, media narrative analysis
- A writer or researcher might want: source and reference monitoring across their active topics, emerging discourse tracking in their area, "things I'll want to have read before I start drafting"
- Someone who speaks publicly — conferences, panels, media — might want: a rolling radar of what audiences and moderators are likely to ask about next, narrative shifts in their field since their last appearance, counter-arguments and emerging critiques of their known positions
- A solo practitioner might want: field-of-practice radar, opportunity signals, "things my clients will ask me about next month"

Each report type has: a clear scope (what sources), a clear question (what to look for), and a clear output format (how to present it).

**Claude should resist the urge to over-engineer this.** Two well-defined report types that get used are better than six that don't.

---

## Step 6: Close the feedback loop

The most valuable moment in the system is when a person reads the AI's output and thinks "yes, but the real insight is actually X." That interpretive move — the gap between what the AI surfaced and what the human sees — is where intelligence lives.

**Claude should help the person design a lightweight way to capture those reactions:**
- Could be as simple as a notes file where they jot reactions to the weekly digest
- Could be a thread in a team channel where people respond to the synthesis
- Could be annotations on the reports themselves

The goal isn't to train the AI. It's to make human judgment persistent and cumulative rather than ephemeral. If those reactions also get fed back into future analysis as context, that's a bonus — but the primary value is the record of thinking.

**Once the loop is closing, help the person see what comes next.**

At this point the person has a working system: curated inputs, AI synthesis, human review, captured reactions. Claude should use what it's learned about their practice to help them see where the system could extend further — not by adding more scanning, but by asking:

- Now that you have a reliable signal layer, what decisions does it actually inform? Is there a gap between "I noticed this" and "I acted on it"?
- Are there other people — collaborators, a team, a community — whose signal detection would compound with yours? What would it take to connect them?
- Is any of what you're producing here valuable to an audience beyond yourself? Could a version of this become a public artifact — a newsletter, a radar, a resource — that also builds your credibility?
- Where are you still doing synthesis manually that the system could take on, now that you trust the boundaries?

This isn't a second build. It's a design conversation about what the person's signal infrastructure makes possible once it's working. Claude should hold this lightly — surface the possibilities, let the person decide what matters.

---

## Infosec considerations

Claude should surface these proportionally — don't lead with fear, but don't skip them either.

- **Public signals only** (RSS, social media, news) — minimal risk. The data is already public. The main consideration is whether the synthesis output itself becomes sensitive (e.g., if it reveals strategic priorities).
- **Designated opt-in channels** — low risk if people know what they're opting into. Make the scope explicit.
- **Reading existing internal comms** — meaningful risk. Even read-only access to Slack or email changes the security surface. The question to ask: "If this system were compromised, what would an attacker learn?" If the answer is uncomfortable, narrow the scope.
- **Broad internal access** — significant risk for any org. Requires a real security assessment, not a casual decision. Most orgs aren't ready for this regardless of size.

The right posture: start with the lowest-risk, highest-value layer (curated public signals) and add internal access only when you've proven the value and can scope it tightly.

---

## What this is not

This is not an autonomous intelligence system. It's a structured way to extend a person's (or team's) existing capacity to detect, process, and act on signal — with AI handling synthesis and pattern-matching within boundaries set by human judgment.

The human decides what to pay attention to. The AI helps process the volume. The human decides what it means. That division is the architecture.
