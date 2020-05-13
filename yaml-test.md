---
layout: csv
title: test of yaml front-matter 
date: 2020-05-13
---
Anything above this is yaml frontmatter.
Anything below this is in-line yaml "code"

```yml
version: "2"
services:

  php:
    volumes:
      - your-app-files:/app:nocopy

  nginx:
    volumes:
      - your-app-files:/app:nocopy

volumes:
  your-app-files:
    external: true
```
