# CLAUDE.md

Read the shared repository contract first:

@AGENTS.md

This file provides guidance to Claude Code (claude.ai/code) and adds only Claude-Code-specific
operating rules. Everything tool-neutral — project overview, development commands, architecture and
site structure, design system, collections configuration, content management, and key technical
details — lives in `AGENTS.md`.

## Default posture (trigger-taming)

For routine content and layout edits, implement directly: the smallest change that satisfies the
request and builds cleanly (`jekyll build`). **Do not auto-invoke discipline skills** (brainstorming,
planning, etc.) unless I ask or the task genuinely spans multiple areas of the site (e.g. layout +
config + data files together). Your instructions here outrank any skill pack's self-invocation rule
— so follow this default and reach for a skill only when it clearly earns its place. Do not add new
build tooling, abstraction layers, or gem-based themes without being asked (the site deliberately
uses a custom theme with all styling in the layout file).
