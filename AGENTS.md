# Agent Notes

This file records issues encountered and their resolutions when working with this project via AI agents.

---

## Issue: CI Build Failure - Missing Frontmatter

**Date**: 2026-03-27

**Error**:
```
[InvalidContentEntryDataError] blog → why-write-skillmd-carefully data does not match collection schema.

  title**: **title: Required
  description**: **description: Required
  pubDate**: **pubDate: Invalid date
```

**Root Cause**:
The blog post file `src/content/blog/why-write-skill.md-carefully.md` was missing the required YAML frontmatter (title, description, pubDate) that Astro's content collection schema expects.

**Fix**:
Added the following frontmatter to the file:

```md
---
title: "Why Skill Directory Structure Matters"
description: "A memory management lesson for AI agent Skills: why structured context beats bloated single files."
pubDate: "Mar 27 2026"
tags: ["ai", "skill", "context"]
---
```

**Lesson**:
All blog posts in this Astro project must include frontmatter with at least:
- `title`: string
- `description`: string  
- `pubDate`: date string in format "MMM DD YYYY"

Reference: https://docs.astro.build/en/guides/content-collections/

---
