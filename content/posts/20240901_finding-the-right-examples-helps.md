---
author: ["DefJM"]
title: "Finding the right examples helps"
date: 2024-09-01
draft: false 
tags: ["coding", "teaching", "version-control"]
---

**TLDR: I created the GitHub repo [contract-versions](https://github.com/DefJM/contract-versions) to show the importance of version control and diffs to non-developers.**

Sometimes finding the right example helps a lot. Even more so when it is visible. It makes things clear and people get it.

More than once I find myself explaining the importance of [version control](https://en.wikipedia.org/wiki/Version_control) and [diffs](https://dictionary.cambridge.org/dictionary/english/diff) to non-developers. The concepts are important not only for programming code but to many more areas such as datasets and machine learning models. More than once, unfortunately, business folks struggle to understand its value.

An explanation can fail big time when one opens the terminal and starts to run git commands. It seems last week I found a better way. I had a relative trying to understand the concept and I remembered that earlier he had complained about Microsoft updating its terms and that it was so much to read. 

![Screenshot of a diff between two versions of Microsoft's Service Agreements](../images/diff-ms-service-agreements.png)

So I [created a repo on Github](https://github.com/DefJM/contract-versions) to compare the two versions of Microsoft’s Service Agreements. I showed my relative the visual diff of those two versions and had him scroll through the coloured changes. He seemed excited so I showed him another [commit](https://github.com/home-assistant/home-assistant.io/commit/e5eff4be6e641f112e62df7cb1865659b613f52b) in the documentation of [Home Assistant](https://www.home-assistant.io) and [where it was](https://www.home-assistant.io/integrations/alexa.smart_home/#add-code-to-the-lambda-function) in the documentation. 

![Screenshot of the commit diff in Home Assistant](../images/commit-diff-home-assistant.png)

My relative appreciated these examples. He had previously been trying to pinpoint those contract changes in the docs manually! I also think he now has a (basic) understanding how version control and diffs are used when we build software as a team. Sometimes it is indeed very helpful to have relatable and visual examples!

