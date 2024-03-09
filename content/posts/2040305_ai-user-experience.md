---
author: ["DefJM"]
title: "Human-AI-Interaction: We need to think more about AI usability"
date: 2024-03-05
draft: false 
tags: ["UX-UI", "Human-AI-Interaction"]
---


## AI applications are different from conventional software systems. And this matters.

AI applications are different from conventional software systems. This has implications for user experience and usability. 

Developers need to **understand the effects of probabilistic model outputs**. For example, what impact has a chatbot answer if it contains a hallucination? This is highly dependent on the given use case. It may be no problem if the chatbot is used to brainstorm design ideas. It may become a big no-go if the chatbot is used to support doctors in the diagnosis of serious illnesses. We need to design product experiences with non-perfect accuracies (and hallucinations) in mind.

**Designing effective prompts and detect and avoid fallacies is surprisingly hard** (see [here](https://dl.acm.org/doi/10.1145/3544548.3581388) and [here](https://people.eecs.berkeley.edu/~bjoern/papers/zamfirescu-aicats-dis2023.pdf)). This also extends to testing, monitoring and providing controls for a save and effective chatbot experience. We have yet to coin the terms for different threats (e.g. "jailbreaking" vs "prompt injection", see Simon Willison's post [here](https://simonwillison.net/2024/Mar/5/prompt-injection-jailbreaking/)).

## Human-AI-Interaction

All their core, these are human-computer-interaction (HCI) challenges. AI and GenAI-applications particularly are a new category of tools for our dear human end-users. It is thus important to gain a better understanding how we interact with them. **Let's call this field Human-AI-Interaction - HAII**. 

An important component for Human-AI-Interaction is AI Explainability. This does not only include the scientific understanding of AI models from research perspective (see a good overview [here](https://course.aisafetyfundamentals.com/alignment?session=5)), but from the perspective of the end-user: How can Humans understand AI systems better? There are interesting studies, for example [in the healthcare field](https://ieeexplore.ieee.org/document/9614151). Human-AI-Interaction is an important component of AI-security (i.e. protecting AI systems against malicious actors) and AI-safety (i.e. protecting people and the environment against often unintended outcomes from AI systems). They have to be thought from HCI perspective, just as we do for the general Cybersecurity domain (see e.g. [International Conference on HCI for Cybersecurity, Privacy and Trust](https://2023.hci.international/hci-cpt)).