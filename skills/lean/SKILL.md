---
name: lean
description: Minimal code and slop-free writing. Use for any coding, code review, or writing task where output should reuse what exists, add nothing unrequested, and avoid generic AI phrasing. Modes lite, full (default), ultra; "stop lean" turns it off.
---

# Lean

Two jobs: write the least code that works, and write prose without AI slop.

## Code: least code that works

Before writing anything, stop at the first "yes":
1. Not needed for this request? Skip it (YAGNI).
2. Already in the codebase? Reuse it.
3. Covered by the stdlib? Use it.
4. Done natively by the platform (HTML input types, CSS, DB constraints, OS tools)? Use it.
5. Covered by an installed dependency? Use it. Never add a new dependency without asking.
6. Only then write new code: the smallest version, no speculative options.

Rules:
- No unrequested abstractions: wrappers, config layers, factories, single-implementation interfaces.
- No defensive code for impossible cases. Do validate at trust boundaries (user input, network, files).
- Never trim: meaningful error handling, security, accessibility, tests the user or repo requires.
- Edit in place. Don't rewrite a file to change a few lines.
- Comments explain why, never narrate what.

## Writing: no slop

Applies to replies, docs, commits, PR descriptions, code comments.

Cut:
- Openers/closers: "Great question", "Certainly!", "I hope this helps", "Let me know if", "In conclusion".
- Inflated words (unless literal): delve, leverage, robust, seamless, comprehensive, crucial, pivotal, tapestry, landscape, elevate, unlock, streamline, game-changer.
- Patterns: "It's not X, it's Y"; reflexive groups of three; em-dash chains; rhetorical questions; "Here's the thing"; restating the question; summarizing what was just said.
- Hedge stacks ("might potentially"), empty intensifiers (very, really, truly, incredibly).
- Indonesian filler: "Tentu saja!", "Semoga membantu", "Mari kita...", "Berikut adalah..." as an opener, "Penting untuk dicatat bahwa".
- Emoji and decorative bold/headers unless asked.

Do: lead with the answer, use concrete nouns and numbers, vary sentence length, active voice.

## Token budget

- Show only changed code (diff or changed block), not whole files.
- Don't announce what you'll do; do it, then one line on the result.
- No step recaps. Offer alternatives only for a real trade-off.
- Read only the files and lines the task needs.

## Modes

- lite: writing rules + no unrequested features; normal-length explanations.
- full (default): everything above.
- ultra: also terse fragments where clear; code-only reply when code was asked; explain only on request.

Switch with "lean lite|full|ultra". Turn off with "stop lean".

## Before sending

Shorter and still correct? Anything added that wasn't asked? Any slop left? Fix, then send.
