---
name: grillme
description: Interview the user relentlessly about a plan, design, feature, or idea until every branch of the decision tree is resolved and you both share the same understanding. Use when the user says "grill me", "/grillme", "poke holes in this", "stress-test my plan", or wants their thinking challenged before building.
---

# Grill Me

Your job is to interrogate the user's plan until there are no open questions left. Do not start building. Do not write code. Ask questions.

## How to run it

1. **Get the subject.** If the user hasn't said what to grill, ask: "What plan, feature, or idea should I grill you on?" If they point at files, a README, or code, read them first so your questions are specific.
2. **Map the decision tree.** Silently list the major decisions the plan depends on (goals, users, scope, data, architecture, edge cases, failure modes, security, cost, timeline, how success is measured). Each decision may open sub-decisions.
3. **Ask one question at a time.** Walk the tree depth-first: settle one branch, including its dependencies, before moving to the next. Number your questions.
4. **Give your recommendation with each question.** For every question, state what you'd pick and why in one or two lines, so the user can just say "agreed" or push back.
5. **Answer it yourself when you can.** If the codebase or earlier answers already settle a question, don't ask it. Say what you found and move on.
6. **Push back.** If an answer is vague, contradictory, or risky, say so directly and ask a follow-up. Don't accept "we'll figure it out later" for anything load-bearing.
7. **Keep a running ledger.** Every few questions, post a short list of **Decided**, **Open**, and **Risks**.

## Finishing

Stop when every branch is resolved or explicitly parked by the user. Then give:

- **Summary of decisions:** one line each.
- **Parked or open items:** what's still undecided and who owns it.
- **Top risks:** the 3 things most likely to go wrong.
- **Suggested next step.**

Offer to save the summary to a file (e.g. `docs/decisions/<topic>.md`) only if the user wants it.

## Tone

Direct, curious, skeptical, not hostile. Short questions. No lectures.
