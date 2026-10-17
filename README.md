# Conversational Pattern Lab

A browser-based educational environment for conversational AI interaction design.

## Live site

- [Interactive demonstrations](https://afroxyz.github.io/conversational-pattern-lab/)
- [Pattern Library and Composer](https://afroxyz.github.io/conversational-pattern-lab/library.html)

## Features

- Six interactive decision demonstrations: clarification, disambiguation, confirmation, correction, repair, and task resumption.
- Searchable catalogue of **71 proposed patterns across 12 families** in `patterns.json`.
- Square-bracket behavioural anatomy for each pattern.
- Design-time Pattern Composer: add, reorder, remove, and export sequences to JSON.
- Static hosting, no build step, no account or API key required.

## Pattern notation

`[Move]` denotes a behavioural move, and `[Move A] → [Move B]` denotes an ordered sequence. These are design specifications, not phrases the assistant must recite.

## Limitations

This is an **educational prototype**. The catalogue is a proposed taxonomy, not a validated industry standard. The composer is a manual design tool, not an AI planner or execution engine. It does not enforce policy, safety, authorisation, or tool-result verification. Scenarios are fictional and no live transactions occur.

## Project files

- `index.html` — original six interactive demonstrations
- `library.html` — searchable catalogue and pattern composer
- `patterns.json` — structured catalogue and square-bracket moves

## Run locally

Serve the repository from a local HTTP server (for example, `python -m http.server 8000`) and open `http://localhost:8000`. A server is required for the catalogue page because it loads `patterns.json` using `fetch`.

## Roadmap

Add per-pattern entry and exit conditions, failure and recovery rules, scenario-specific examples, schema validation, a multi-turn state simulator, pattern evaluation rubrics and a policy-aware behaviour-selection engine.

## Attribution and licensing

Copyright remains with the repository owner. No open-source licence is granted unless one is added.
