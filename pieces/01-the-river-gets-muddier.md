---
layout: piece
title: The River Gets Muddier
---

# The River Gets Muddier

The same model, the same question, forty turns into a conversation instead of one. The answer is measurably worse.

Not always. But reliably enough that practitioners have learned to start fresh for hard problems. The common explanation is vague: "context window limitations." But the window isn't full. The model isn't running out of space. Something else is happening.

When a language model generates a response, it's weighing every piece of text it can see against everything else. At turn 1, the field is small — a few thousand words, almost all of them relevant. By turn 40, it's forty thousand. Every word is a candidate, whether it's still useful or not. Old results don't sit quietly in the background. They compete for the same attention as what matters right now.

The signal doesn't grow with the conversation. The noise does.

Early in a session, nearly everything the model reads is working: a clear instruction, a focused question, a fresh result. By turn 8 of a multi-step task, the transcript has accumulated stale information that no longer reflects reality, intermediate reasoning nobody needs anymore, results the model already acted on. The proportion of useful text shrinks with every exchange. The model has no way to mark anything as expired — it treats a result from six turns ago the same as a fresh one.

More context is not the same as more information.

What the model actually needs isn't volume. It's density — the right information, positioned where it will naturally draw attention. A curated prompt at turn 1 outperforms a rambling conversation at turn 30, even if the conversation technically contains more relevant information.

The architecture is the same. The water changes. Design the channel.
