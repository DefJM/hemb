---
author: ["DefJM"]
title: "Finding the right example helps"
date: 2024-09-01
draft: false 
tags: ["coding", "teaching", "version-control"]
---

**TLDR: I created the GitHub repo [contract-versions](https://github.com/DefJM/contract-versions) to show the importance of version control and diffs to non-developers.**

Sometimes finding the right example helps a lot. Even more so when it is visible. It makes things clear and people get it.

More than once I find myself explaining the importance of version control to non-developers. The concept is important not only for programming code but to many more areas such as datasets and machine learning models. More than once, unfortunately, business folks struggle to understand its value. 

An explanation can fail big time when one opens the terminal and starts to run git commands. It seems last week I found a better way. I had a relative trying to understand the concept and I remembered that we had just talked about social media companies constantly updating lengthy data clauses. 

![Screenshot of the diff between two versions of Microsoft's Service Agreements](../images/diff-ms-service-agreements.png)

So I [created a repo on Github](https://github.com/DefJM/contract-versions) to compare two versions of Microsoft’s Service Agreements. It sounds too simple, but showing non-programmers the diff of those two contract versions and scrolling through changes was a great show-case. Especially when my counterpart was desperately trying to find those changes manually!
