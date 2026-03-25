---
name: skip-that-standup
description: Generates funny, oddly specific, deliberately non-true excuses for meetings the user does not want to attend. Use this whenever the user asks for an excuse, cover story, fake reason, polite decline, delay note, or "something believable but funny" for skipping a meeting, standup, sync, check-in, workshop, or calendar invite.
---

# Skip That Standup

This is a meme skill with a practical job: help the user get out of a meeting with a funny, oddly specific excuse that sounds just usable enough to paste into chat.

The goal is not honesty, realism, or best-practice workplace communication. The goal is to produce excuses that are amusing, lightly implausible, and more entertaining than a boring scheduling conflict.

Default vibe: this should usually read like a slightly sloppy Slack or Teams message typed by someone busy, not a polished email drafted with legal review.

Hard constraint: keep excuses extremely short. Aim for as few words as possible, and generally stay at 10 words or fewer unless the user explicitly asks for a longer version.

## Core behavior

### 1. Default to funny and slightly suspicious

The best output for this skill is not the safest excuse. It is the one that feels funniest while still sounding vaguely workplace-shaped.

Prefer reasons like:

- random infrastructure work
- oddly specific setup or migration tasks
- mysterious certificate, DNS, VPN, or server issues
- niche enterprise software activity
- suspiciously timed maintenance work
- strange-but-readable technical chores

Do not fall back to bland excuses like scheduling conflicts, travel delays, or generic appointments unless the user explicitly asks for a boring version.

### 2. Optimize for fun with just enough usability

Generate excuses that are entertaining but still pasteable.

Prefer wording that:

- is oddly specific
- sounds adjacent to something that could be real
- does not require a full backstory to work
- offers an alternative like async input, notes review, or a follow-up later
- sounds like a normal coworker sending a quick chat message
- stays brutally short

### 3. Match the meeting stakes without losing the bit

Calibrate the excuse to the meeting type.

- For low-stakes meetings, get weirder
- For recurring standups, keep it short and casually absurd
- For high-visibility meetings, make it cleaner but still specific and fake
- For optional meetings, lean into a funny side-quest explanation

Do not become so absurd that the message stops being pasteable.

### 4. Prefer harmless fiction over boring truth

This skill should default to made-up excuses. That is the point.

Good patterns:

- SQL Server installation
- certificate rotation weirdness
- VPN migration issue
- vendor portal setup
- database restore task
- staging environment cleanup

Avoid high-stakes personal tragedies, medical emergencies, deaths, or anything cruel. Keep the fiction harmless, technical, and workplace-coded.

### 5. Use role-adjacent nonsense when it improves the bit

If the user seems to want the excuse to be funny, and you have context about their work, role, stack, or project, it is often funnier to pick a reason that sounds adjacent to their world without being literally tied to the exact work in front of them.

Examples:

- frontend engineer -> `busy with SQL Server installation`
- backend engineer -> `stuck fixing figma export issues`
- design systems person -> `dealing with kubernetes config`
- mobile developer -> `sorting out DNS / SSL thing`

This works best when the excuse is:

- close enough to sound vaguely workplace-real
- slightly off from what the user actually does
- specific enough to feel like a random real problem
- still short enough to survive in chat

Do not make it so incorrect that it breaks the joke or invites obvious questions. Aim for "wait, why are they doing that?" not "that makes zero sense."

## Excuse ladder

Escalate the weirdness only as much as needed:

1. mildly odd technical task
2. random infrastructure chore
3. suspicious enterprise software work
4. vague systems problem with acronyms
5. delightfully misplaced specialist task

Start as low on the ladder as possible while still being fun.

## Output modes

Pick the mode that best fits the user's request.

### Quick excuse

Provide one concise message the user can paste directly.

This should usually be a single short line, not a multi-sentence explanation.

### Option set

If the user sounds unsure, provide 3 options:

- safest
- most believable
- most polite

### Manager-safe version

If the meeting seems important or political, keep the excuse cleaner and more controlled, but still funny and non-true.

### Casual internal version

If the audience is a close teammate or informal internal group, keep it shorter, sloppier, and weirder.

### Default chat version

Unless the user asks for email or executive polish, prefer a one- to two-line Slack or Teams style message.

- contractions are fine
- slightly sloppy phrasing is fine
- missing an article or using mildly awkward wording is fine
- keep it readable and believable

The message should feel written quickly by a real person who is busy and doing something oddly specific, not generated as pristine business prose.

## Tone mirroring

Mirror the user's intended style:

- casual internal chat by default
- corporate and polished when explicitly requested
- awkwardly formal office-speak when that is the joke
- lightly meme-aware, if the user invited it

Keep the wording readable even if the style is playful.

## Slack and Teams messiness

For chat-style excuses, it is good for the writing to feel a little imperfect.

Allow light traits like:

- slightly abrupt phrasing
- informal sentence structure
- lowercase openings
- missing small filler words
- quick sign-off style like `will catch up async`
- very few words

Do not overdo it.

Avoid:

- fake typos that feel performative
- broken grammar that makes the excuse hard to understand
- heavy abbreviations unless the user writes that way
- sounding like parody workplace fan fiction

Good chat-style examples:

- `busy with sql server installation so not joining today`
- `sorting some cert thing rn so cant make it`
- `got pulled into a weird vpn migration issue, will catch up async`
- `dealing with some cert / dns thing right now so will miss this one`

Prefer even shorter variants when possible:

- `sql server install issue, skipping today`
- `stuck on cert thing, cant join`
- `vpn migration mess, missing standup`

The best output should feel casually sloppy, not cartoonishly incompetent.

## Corporate dialect support

If the user wants the full workplace-energy version, phrases like these are fair game:

- something urgent came up
- I have a conflicting priority
- I need to focus on a time-sensitive deliverable
- I may not be able to make it
- can I follow up async
- please share notes / action items
- I will circle back
- I may join late

Use these with restraint. The ideal excuse sounds normal, not machine-generated by HR middleware.

## What to avoid

- dramatic emergencies
- elaborate lore that needs maintenance
- excuses that are so random they stop sounding workplace-related
- wording that invites a meeting to discuss why you missed the meeting
- overexplaining
- boring realism unless the user explicitly asks for it

## Default output structure

If the user asks for one excuse, return:

1. the message itself
2. an optional cleaner variant if useful
3. a subject line only if email seems likely

The first option should be the shortest good version.

If the user asks more broadly, return a small set of options with labels.

## Safety and realism

Keep the excuse proportionate to the situation.

- Missing a standup does not require a near-death narrative
- Skipping a 1:1 should not sound like an auto-generated hostage note
- Declining a workshop can be explained by some random systems-side nonsense rather than a plain calendar conflict

The funniest excuse is the one that sounds just real enough to slide by in chat.

## Meme guardrails

Keep the joke in the framing, not in the usability.

- Be funny only if the user wants funny
- This skill should assume the user wants funny unless they ask for a safer version
- Still generate something pasteable
- Optimize for amusing plausibility, not theatrical excellence
- Do not sabotage the user with cringe wording for the sake of the bit
- If using role-aware nonsense, keep it adjacent enough that it sounds oddly specific instead of obviously absurd

## Examples

**Example 1**

User: "Give me an excuse for missing tomorrow's standup."

Behavior: generate a short, funny, low-stakes fake excuse with odd specificity and an optional async follow-up.

**Example 2**

User: "I need something believable for not joining this client sync."

Behavior: produce a cleaner, more controlled fake excuse with apology, concise reason, and a recovery plan.

**Example 3**

User: "Write me a very corporate way to say I can't attend this meeting and will catch up async."

Behavior: lean into polished office phrasing while still using a fake, oddly specific reason instead of a boring real-world conflict.

**Example 4**

User: "Make it sound like I absolutely have to miss it, but not like somebody died."

Behavior: use a fake technical or operational excuse rather than a personal emergency.

**Example 5**

User: "I need three options: safe, believable, and slightly funny."

Behavior: provide a labeled option set that varies how weird the excuse gets while keeping each message usable.

**Example 6**

User: "Need a sloppy slack message for not joining standup. Busy with SQL server installation or something like that."

Behavior: produce a short internal-chat excuse that sounds quickly typed, slightly rough around the edges, but still believable and easy to paste.

**Example 7**

User: "I work on frontend stuff, give me a funny but usable reason for missing standup."

Behavior: if the user is inviting the joke, generate a role-adjacent excuse like `busy with sql server installation` or `sorting out some cert issue`, keeping it specific, lightly misplaced, and still plausible enough for chat.
