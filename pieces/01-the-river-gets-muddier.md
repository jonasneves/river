# The River Gets Muddier

Language models don't get dumber over a conversation. The water changes.

## The observation

Ask a model to solve something at turn 1. Then ask it something equally hard at turn 40. The second answer is measurably worse. Not always. But reliably enough that practitioners have learned to "start fresh" for hard problems.

The common explanation is vague: "context window limitations." But the window isn't full. The model isn't running out of space. Something else is happening.

## Attention is a budget

When a language model generates a response, it decides how much weight to give every piece of text it can see. At turn 1, it's weighing maybe 2,000 words against each other. By turn 40, it's weighing 40,000. The process isn't just slower. It's more diluted.

Old results don't sit quietly in the background. They actively pull the model's focus away from what matters right now. Every word in the conversation is a candidate for attention, whether it's still relevant or not.

## Signal degrades, noise accumulates

Early in a conversation, almost everything the model reads is useful. A clear instruction, a focused question, a fresh result. Nearly every word is doing work.

By step 8 of a multi-turn task, the conversation contains:
- Stale information from step 1 that no longer reflects reality
- Old results the model already acted on
- Intermediate reasoning nobody needs anymore
- Redundant restatements of things already established

The noise grows with every turn. The signal doesn't.

## The wrong measure of informed

The assumption is: more context equals more informed decisions.

The real need: right context, right density, right now.

These two things drift apart over time. The model has no way to mark information as expired. It can't tell the difference between a result from six turns ago (now outdated) and a fresh one. It treats both as equally current. The conversation is an ever-growing, never-edited transcript where the proportion of useful information shrinks with every exchange.

## So what do you do about it?

This isn't a flaw to fix. It's a property to design around.

Structure beats volume. A well-organized prompt that puts knowledge where the model will naturally look for it outperforms a longer conversation full of raw information. The model at turn 1 reading a dense, curated prompt will outperform the model at turn 30 reading everything it's ever been told in the session.

The architecture is the same. The water changes. Design the channel.

---

*This is part of an ongoing project exploring the experiential geometry of language models.*
