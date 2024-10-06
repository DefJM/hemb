---
author: ["DefJM"]
title: "Human-AI-Interaction: We need to think more about AI usability"
date: 2024-03-09
draft: false 
tags: ["UX-UI", "Human-AI-Interaction", "AI-security"]
---


## AI systems are different from conventional software systems. And this matters.

In my job to develop and implement machine learning and AI services for multiple industrial use cases. As we deal with related quality and security challenges, it has become clear to me that we need to spend more time thinking through the user experience (UX) of these systems. They are different from conventional software systems and this has implications for usability and design. 

**It is hard for developers to understand the effects of probabilistic model outputs.** For example, what impact has a chatbot answer if it contains a hallucination? This is highly dependent on the given use case. It may be no problem if the chatbot is used to brainstorm design ideas. It may become a big no-go if the chatbot is used to support doctors in the diagnosis of serious illnesses. We need to design product experiences with a non-perfect precision scores (and in the case of chatbots even hallucinations) in mind.

**Designing effective prompts and avoid fallacies is surprisingly hard** (see [here](https://dl.acm.org/doi/10.1145/3544548.3581388) and [here](https://people.eecs.berkeley.edu/~bjoern/papers/zamfirescu-aicats-dis2023.pdf)). This also extends to testing, monitoring and providing controls for a save and effective chatbot experience. We have yet to coin the terms for different threats (e.g. "jailbreaking" vs "prompt injection", see Simon Willison's post [here](https://simonwillison.net/2024/Mar/5/prompt-injection-jailbreaking/)).

**Understanding AI models and the reasons behind their output is hard.** "Explainable AI" usually focusses on researchers and their scientific understanding of AI models. The [AI Safety Fundamentals](https://course.aisafetyfundamentals.com/alignment?session=5) project by BlueDot Impact provides a good overview. But it is also important from the perspective of the end-user: How can humans understand AI systems better when interacting with them? There are interesting studies, for example [in the healthcare field](https://ieeexplore.ieee.org/document/9614151). 

**Usability is important for AI security and AI safety.** AI-security (i.e. protecting AI systems against malicious actors) and AI-safety (i.e. protecting people and the environment against often unintended outcomes from AI systems) need to be thought from the end-user perspective, just as we do for the general cybersecurity domain (see for example the [International Conference on HCI for Cybersecurity, Privacy and Trust](https://2023.hci.international/hci-cpt)).


## Human-AI Interaction: Human–Computer Interaction (HCI) for AI Systems
All their core, these are human-computer interaction (HCI) challenges. AI and GenAI-applications particularly are a new category of tools for our dear human end-users. It is thus important to gain a better understanding how we interact with them. **This field of research is called Human-AI-Interaction**.

For further research, the [Special Issue on Human-AI Interaction](https://www.sciencedirect.com/journal/data-and-information-management/vol/7/issue/3) (2023-09) of the Data and Information Management Journal seems a good starting point.  

There is also an online course [Human–Computer Interaction (HCI) for AI Systems Design](https://advanceonline.cam.ac.uk/courses/human-computer-interaction-hci-for-ai-systems-design?utm_medium=cpc&utm_source=google&utm_campaign=DSA_UK) (with a juicy fee) from the University of Cambridge. This course, taught by [Professor Per Ola Kristensson](https://advanceonline.cam.ac.uk/course-lead/per-ola-kristensson), focusses on methods for designing AI systems to "assist users in achieving their goals and improving user experience". 
