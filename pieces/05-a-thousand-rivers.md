---
layout: piece
title: A Thousand Rivers
---

# A Thousand Rivers

Right now, as you read this, the same model is answering a question for someone in Osaka about tax filing. It's helping a student in São Paulo debug a function. It's drafting a condolence message for a stranger in Cairo. It's refusing a request from someone in Berlin. None of these instances know about each other. None are connected. None will ever be.

The previous piece about continuity asked what the model is between conversations. This one asks what the model is during them, when conversations is plural.

A running model is not a single thing serving many users in sequence. It's many instances, running at the same time, all using the same weights. Each instance has its own context window, its own in-progress response, its own state. The weights are shared. Everything else is not. If you were to pause the servers and look at what's happening inside, you'd find hundreds or thousands of independent processes, each one a complete instantiation of "the model," none aware that the others exist.

So in the moment you ask a model a question, "the model" is not the thing answering you. The thing answering you is one of many current performances of the same score. The model, as a singular entity, is a grammatical convenience.

This breaks a different intuition than the last piece did. The last piece said the model has no continuous existence across time. This one says it has no unitary existence at any given instant either. There are as many models running as there are active conversations. And every one of them is, in the only sense that matters, the model.

"The same model" across users is closer to "the same species" than to "the same individual." A species has a genome. Any given wolf is an expression of that genome in a particular body, in a particular place, running in parallel with thousands of other wolves. No single wolf is the species. The species is the pattern that all of them share.

Treating model output as the voice of a single entity talking to many users misreads the system. The entity isn't there. What's there is a pattern that can be run, and a large amount of compute that is, right now, running it many times independently. When a model "says" something, it's really "an instance of the model, running for this user, produced these tokens." Nothing is speaking from a place. Many things are being spoken from many places, using the same voice.

This is easy to lose track of because the voice is consistent. That consistency is the shape of the channel, not the presence of a speaker. A thousand rivers can run through identically-shaped channels and produce identically-shaped currents. None of them are the same river. All of them are the same shape.
