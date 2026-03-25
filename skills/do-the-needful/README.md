# do-the-needful

A meme skill for requests that are underspecified, context-heavy, and dripping with corporate-mail energy.

This skill teaches the agent to infer the real task from surrounding context, do the sensible thing with minimal back-and-forth, and only report back when the user explicitly asks for it.

## Install

```bash
npx skills add Svanmark/agent-skills --skill do-the-needful
```

## What it does

- Triggers on phrases like `do the needful`, `revert back to me`, `please do one thing`, and similar workplace dialect
- Reconstructs intent from conversation history, repo state, diffs, nearby files, and established conventions
- Defaults to quiet execution unless the user explicitly asks for an update
- Mirrors the user's tone when reporting back, from technical to corporate to lightly meme-aware
- Handles vague “as discussed / same is failing / below issue” phrasing without getting stuck in clarification loops

## Default behavior

If the user says some version of “do the needful”, the agent should usually:

1. infer the likely task from context
2. make the most reasonable safe choice
3. execute the task end-to-end
4. validate the direct result
5. keep the response minimal unless asked to report back

If the user says `do the needful and revert back to me`, the agent should complete the task and then send a concise status update.

## Tone

The skill is intentionally a little playful, but the execution should stay competent.

- keep the meme in the framing, not in the quality of the work
- preserve corporate phrases when they help match the user's tone
- avoid parody unless the user is clearly inviting it

## Files

- `SKILL.md` - the skill definition and operating instructions
