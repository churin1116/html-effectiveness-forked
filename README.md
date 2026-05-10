# html-effectiveness (Chameleon-fork)

A fork of [ThariqS/html-effectiveness](https://github.com/ThariqS/html-effectiveness) — 20 single-file HTML examples demonstrating Claude's HTML output capabilities (exploration sketches, code reviews, design systems, prototypes, slide decks, status reports, editor mockups, etc.).

**Live:** https://churin1116.github.io/html-effectiveness-forked/

## What's different in this fork

Every page is wired to the [Chameleon](https://github.com/churin1116/html-chameleon) theme contract:

- `<meta name="chameleon" content="v1">` for extension detection
- The hosted `theme.css` + `theme.js` are linked in `<head>`
- `<html data-theme="claude">` declares the page-preferred theme — when a reader has no stored preference, the artifact appears in the Claude (Anthropic warm) palette by default; once they pick any theme via the [Chameleon Chrome extension](https://github.com/churin1116/html-chameleon/tree/main/extension), that choice becomes sticky across all Chameleon-aware pages.

The original page colors (`<style>` blocks) remain intact and win over Chameleon's variables — installing the extension on this site adds the floating theme palette, but the on-page rendering stays as the author intended unless the page is fully retrofitted via the Chameleon `convert` Skill mode.

## Original credit

All HTML artifacts are by the original author at [ThariqS/html-effectiveness](https://github.com/ThariqS/html-effectiveness). This fork only adds the Chameleon detection signals.
