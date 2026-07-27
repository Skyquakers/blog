# EdgeRunners Blog

This repository is the content source for the EdgeRunners blog at
`https://edgerunners.cn/blog`.

## Add a post manually

Create a lowercase, kebab-case Markdown file in `posts/`. The filename becomes
the article URL:

```text
posts/running-a-palworld-server.md
https://edgerunners.cn/blog/running-a-palworld-server
```

Every post starts with YAML frontmatter:

```md
---
title: Running a Palworld server
description: A short summary shown on the blog index.
date: 2026-07-28T00:00:00+09:00
author: EdgeRunners
tags:
  - Palworld
  - Guide
cover_image: https://example.com/optional-cover.webp
draft: false
---

Write the article in Markdown here.
```

Only `.md` files immediately inside `posts/` are published. Posts with
`draft: true` are hidden. Use ISO 8601 dates so ordering is deterministic.

Images managed by Decap CMS are stored in `images/uploads/`. For manually
authored posts, prefer absolute image URLs or use the raw GitHub URL:

```text
https://raw.githubusercontent.com/Skyquakers/blog/main/images/uploads/image.webp
```

The website refreshes its cached post list and article content every five
minutes.
