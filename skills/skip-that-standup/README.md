# skip-that-standup

A meme skill for generating funny, fake, oddly specific excuses for meetings the user does not want to attend.

It is optimized for amusing workplace-coded nonsense, usually with a slightly sloppy Slack or Teams chat feel rather than polished email prose.

## Install

```bash
npx skills add Svanmark/agent-skills --skill skip-that-standup
```

## What it does

- Generates funny fake excuses for skipping meetings, standups, syncs, check-ins, and workshops
- Calibrates how weird the excuse gets to the stakes of the meeting
- Prefers oddly specific technical nonsense over boring scheduling conflicts
- Keeps the excuses extremely short, usually 10 words or fewer
- Offers async follow-up language so the user still sounds responsible
- Defaults to quick, slightly sloppy internal chat wording unless the user asks for something more polished
- Mirrors the requested tone, from polished corporate to casual internal chat to lightly meme-aware
- Can use role-adjacent oddly specific excuses for extra meme value when the user invites that style

## Default behavior

When the user asks for a meeting excuse, the skill should usually:

1. infer the audience and stakes from the prompt
2. choose a funny fake reason that still sounds chat-pasteable
3. write a pasteable chat message
4. add a short fallback or async line if helpful
5. avoid excuses that create so many questions that the joke stops working

## Tone

The skill is playful in concept but should stay useful in practice.

- keep the joke in the framing, not in the actual excuse quality
- prefer usable office chat language with fake technical specificity
- avoid soap-opera excuses unless the user explicitly asks for absurdity
- when going for funny, slightly misplaced role-related excuses are better than full nonsense

## Files

- `SKILL.md` - the skill definition and operating instructions
