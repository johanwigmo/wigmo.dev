+++
title = "BulletMark"
date = 2026-02-19
description = "A lightweight, human-readable markup specification for tasks and notes"
weight = 20

[params]
    featured = true
    tech = ["Markdown"]
    status = "Active"
    github = "https://github.com/johanwigmo/bulletmark-spec"
+++

BulletMark is my personal specification for organizing tasks, events, and notes in plain text. It extends standard markdown with a small set of markers for task states, projects, tags, and dates — everything stays readable in any text editor, no tooling required.

It combines the simplicity of bullet journaling with structured markup: rapid logging for daily notes, with just enough structure for implementations to parse reliably.

```markdown
# 2026-02-05 Wednesday

- [o] 09:00: *Standup*
- [ ] Review pull requests +CodeReview
    due: 2026-02-06
    - https://github.com/org/repo/pull/123
- [/] Write API documentation +Docs
- [>] Call accountant
- [<] Optimize image loading +Performance
- [x] 2026-02-05 Morning workout

= Feeling good about progress this week
```

## Features

- Item types for tasks, events, notes, and reflections
- Projects (`+Project`) and tags (`@Tag`) for organization
- Due dates, defer dates, completion dates, and event times
- Migrated (`[>]`) and backlogged (`[<]`) log markers, bullet-journal style
- Four-space indentation for hierarchy
- Valid markdown — renders sensibly everywhere
- Parsing and write-back rules for implementations

[Specification on GitHub](https://github.com/johanwigmo/bulletmark-spec)

