+++
title = "bulletmark.nvim 1.0.0"
date = 2026-10-23
description = "The BulletMark reference implementation for Neovim: conformance-tested parser, task cycling, vault-wide search"
tags = ["announcement", "release"]
project = ["bulletmark"]
+++

I just tagged version 1.0.0 of [bulletmark.nvim](https://github.com/johanwigmo/bulletmark.nvim), the first implementation of [BulletMark](https://github.com/johanwigmo/bulletmark-spec), my plain-text specification for tasks and notes. It's positioned as the spec's reference implementation: the parser is conformance-tested against the spec repository's own fixtures, so anything not in the spec — a second `+Project`, an impossible date, non-ASCII marker characters — is a warning, never a guess.

In daily use it behaves like a bullet journal in Neovim. `<CR>` cycles `[ ]` → `[/]` → `[x]` and stamps a completion date; pressed on anything that isn't a task, it falls through to whatever your `<CR>` did before. Spec violations show up inline as warnings, and `:BulletMark` searches the whole vault with the same grammar the documents use — `+project`, `@tag`, `due_before:...` — with `+` and `@` completing while you type.

The spec promised that the format needs no tooling. That's still true. But if tooling exists, it should stay out of the way, and that requirement shaped the whole thing: the editor only ever rewrites the checkbox character and the completion date it owns, everything else on a line is untouchable. 130 tests, 18 of which are the spec's own fixtures.

Full details in the [release notes](https://github.com/johanwigmo/bulletmark.nvim/releases/tag/1.0.0).
