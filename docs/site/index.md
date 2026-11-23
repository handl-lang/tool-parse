# tool-parse

The parse-operation contract: `ParserEngine`, `ParserRequest`, `ParserContext`.

## What it is

The **abstraction crate** for the parse operation (ADR-0044 §3): the
`ParserEngine` trait, the `ParserRequest`/`ParserContext` an engine receives, and a
`Parser` cursor helper. **No grammar logic lives here** — the concrete engine is
`tool-parse-pratt`, which reads grammar rows from the language definition.

## Start here

- **Reference** — [public API](/tool-parse/reference/)
- **How-to** — [task recipes](/tool-parse/how-to/)
- **Explanation** — [design and rationale](/tool-parse/explanation/)

No tutorials: this repo is a building block used from Rust. End-to-end
walkthroughs live with the product that composes it — see the
[Handl platform](/handl/).
