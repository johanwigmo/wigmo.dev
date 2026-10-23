+++
title = "BulletMark 2.0.0"
date = 2026-10-22
description = "A simpler BulletMark: priorities removed, migration markers, defer dates"
tags = ["announcement", "release"]
project = ["bulletmark"]
+++

I just published version 2.0.0 of [BulletMark](https://github.com/johanwigmo/bulletmark-spec), my plain-text specification for tasks and notes.

The theme is simplification. Priorities are gone — I never used them. The `[>]` and `[<]` markers now mean what they mean in Bullet Journal: migrated (pushed to a later date) and backlogged (returned to a list). They record a movement decision in the daily log instead of pretending to be task states.

Smaller additions: `defer:` dates for tasks that aren't actionable yet, `---` section rules, and an explicit note that any other markdown is welcome in a document — parsers simply treat it as opaque.

Breaking for parsers, boring for humans: everything I actually write stayed the same.

Full details in the [release notes](https://github.com/johanwigmo/bulletmark-spec/releases/tag/v2.0.0).

