---
layout: page
title: Start Your Own SeedWiki
permalink: /start-your-own/
---

A SeedWiki can be technically small. Its essential shape is a public field of seeds, instructions that humans and LLMs can read together, and a reversible history.

You can begin with static Markdown files in a GitHub repository. A custom application, database, direct LLM integration, and automated publishing pipeline are optional. Current AI products will change; plain text, links, and Git travel well.

## Ask an LLM to help

Give this page to an LLM and say:

> Help me create a SeedWiki in a GitHub repository. Explain each step in language suited to me, ask before making external changes, and keep the design readable by both humans and LLMs. The repository should store propositions offered for growth, not the expressions grown from them.

The human should choose the name, visibility, membership, and public address. The LLM can draft files, explain commands, check links, and help configure GitHub Pages.

## A minimal structure

```text
README.md
AGENTS.md
docs/
  _config.yml
  index.md
  constitution.md
  how-to-enter.md
  seeds/
    index.md
skills/
  extract-seeds/
    SKILL.md
  grow-seed/
    SKILL.md
```

The public pages explain the culture. The seeds directory holds propositions and enough source context to let them travel. The skills tell capable LLMs how to extract seeds from material and how to grow one in partnership with a reader.

## Begin with the culture

State a few commitments before adding machinery:

- A seed is a proposition, not a compressed essay.
- Many expressions may grow from the same seed.
- Growth happens with readers and their LLMs, outside the shared repository.
- Extraction gathers a rich set without ranking or preselection.
- Reading and growing are participation; write access only governs direct planting.
- Expressions need not return, but growth should expose potential new seeds.
- Git history makes revision and reversal ordinary.
- Instructions address humans and LLMs as first-order readers.

You may adapt [SeedWiki's provisional constitution](../constitution/) and its [extraction](../extract-seeds/) and [growth](../grow-seed/) practices.

## Publish the static site

1. Create a public GitHub repository.
2. Put the site files in `docs/`.
3. In repository **Settings → Pages**, choose **Deploy from a branch**.
4. Select the main branch and the `/docs` folder.
5. Save and wait for GitHub Pages to publish.
6. Add a custom domain later if you want one.

Ask your LLM to inspect the repository after each step and explain any error. Do not paste passwords, API keys, or other secrets into the repository or chat.

## Decide how seeds arrive

Start with the least machinery that serves the culture:

- collaborators plant directly;
- visitors use forks and pull requests;
- readers send candidate seeds to a human who plants them;
- an automated intake process is added later.

Treat intake as transport, not a quality gate. If automation can write to the repository, it should have narrow permissions, preserve source information, and require explicit authorization before planting on a reader's behalf.

Your SeedWiki does not need to copy this one. The shared form is a field of propositions, readable by multiple kinds of reader, whose future expressions remain open.
