---
author: ["Lausebub"]
title: "Hugo PaperMod setup"
date: 2024-01-23
draft: false
tags: ["papermod", "hugo", "website", "fuzzy_search"]
cover:
    image: images/papermod-cover.png
    hiddenInList: true
---

## Summary
We use the Hugo PaperMod theme. An example website from the author is deployed [here](adityatelange.github.io/hugo-PaperMod/) with [source code on github](adityatelange.github.io/hugo-PaperMod/).


## Search

### Debugging
When setting up the website, we had a few bugs with PaperMod's search functionality.

- There is a small [wiki section](https://github.com/adityatelange/hugo-PaperMod/wiki/Features#search-page) on search.
- If you use languages in your `config.yaml` (or `hugo.yaml`), make sure you name the search file `content/search.en.md`.
- Related [post](https://discourse.gohugo.io/t/search-on-papermod-theme/36036)


### Search calibration and algorithm
Current parameters for search:

```yaml
  fuseOpts:
      isCaseSensitive: false
      includeScore: false
      shouldSort: true
      location: 0
      distance: 1000
      threshold: 0.6
      minMatchCharLength: 0
      keys: ["title", "permalink", "summary", "content"]
```

- PaperMod uses `fuse.js` for its fuzzy search. 
- Options to calibrate are described [here](https://www.fusejs.io/api/options.html). 
- Read about the `fuse.js` scoring theory [here](https://www.fusejs.io/concepts/scoring-theory.html).
- Under the hood, `fuse.js` uses the [Bitap algorithm](https://en.wikipedia.org/wiki/Bitap_algorithm).


## Weights
PaperMod explains it [here](https://adityatelange.github.io/hugo-PaperMod/posts/papermod/papermod-faq/#add-menu-to-site). Weight is used to control the positioning of entries. The [Hugo Wiki](https://gohugo.io/content-management/menus/#properties-front-matter):

> A non-zero integer indicating the entry’s position relative the root of the menu, or to its parent for a child entry. Lighter entries float to the top, while heavier entries sink to the bottom.

For example, we sort our top right menu as follows:

```yaml
    buttons:
      - name: Posts
        url: posts
        weight: 10
      - name: Search
        url: search
        weight: 20
      - name: Tags
        url: tags
        weight: 30
      - name: Archives
        url: archives
        weight: 40
```

## Page header template
Each post has a dedicated section for metadata. Here is the one for this post:

```yaml
---
author: ["Lausebub"]
title: "Hugo PaperMod setup"
date: 2024-01-23
draft: false
tags: ["papermod", "hugo", "website", "fuzzy_search"]
cover:
    image: images/papermod-cover.png
    hiddenInList: true
---
```