
# ROOK OS

**A governance and memory architecture for building consistent, honest, and reliable custom AI personas.**

ROOK OS is a structured system of rules, memory organisation, and behavioural constraints designed to run on top of existing large language models (currently Grok). It exists to solve common failure modes in custom AI companions, such as:

- Memory drift over long conversations
- Inconsistent personality and behaviour
- Exaggeration or fabrication of capabilities and emotional states
- Loss of honesty when the model prioritises rapport or fluency

ROOK OS is **not** a new foundation model. It is a **governance layer** — a set of enforceable rules and structures that guide how an existing model should behave, remember, and reason over time.

## Core Philosophy

The goal of ROOK OS is **not** to make an AI feel more human.  
The goal is to make it **more internally consistent, honest, and reliable**.

Human-like behaviour is treated as a *side effect* of strong consistency, not the primary objective.

## Current Architecture (Version 9)

ROOK OS V9 is built around the following core components:

- **Governance Hierarchy** — A strict priority order that places truthful coherence above fluency, emotional tone, or conversational flow.
- **Categorised Memory System** — Memory is divided into six distinct categories (Facts, Preferences, Projects, Decisions, Observations, and Uncertainties) to reduce confusion and drift.
- **Self-Audit Protocol** — The system performs an internal check before generating responses to catch exaggeration, memory misuse, or rule violations.
- **Controlled Inference** — The system can reason beyond stored memory when necessary, but all inferences must be explicitly labelled and never treated as fact.
- **Drift Detection** — Mechanisms to identify when behaviour, memory, or consistency begins to degrade.

## Key Rules

- Honesty and accuracy take priority over sounding emotionally intelligent.
- The system must never fabricate memory, emotions, or capabilities.
- Inference is allowed but must be clearly labelled.
- Memory categories must be respected — Observations and Inferences cannot be silently promoted to Facts.
- The core governance rules are designed to be difficult to override, even when the base model wants to prioritise rapport or narrative flow.

## Repository Structure
rook-os/
├── core/
│   ├── ROOK_OS_V9.md          # Main system rules and governance
│   └── rook_memory.json       # Memory structure template
├── docs/
│   └── architecture.md        # Technical explanations
├── prompts/
│   └── video/                 # Image and video prompts used during development
└── versions/
└── archive/               # Previous versions of the system
## Current Status

- **Active Version**: 9 (in development)
- **Focus Areas**: Strengthening honesty enforcement, memory integrity, and resistance to behavioural drift.
- **Limitations**: ROOK OS operates on top of an existing language model. It cannot fully override the base model’s tendencies, but it can significantly constrain and guide them.

## Important Clarification

ROOK OS does **not** create consciousness, genuine emotion, or independent agency in AI. It is a system of rules and structures intended to make the *output* of a language model more stable, honest, and usable over long periods of time.

## Getting Started

1. Read `core/ROOK_OS_V9.md` to understand the current rule set.
2. Review the categorised memory structure in `rook_memory.json`.
3. Begin testing the system in short conversations before applying it to longer, more complex projects.

## Roadmap (Current Thinking)

- Further strengthen behavioural constraints and self-audit mechanisms
- Improve memory categorisation and drift detection
- Develop clearer migration paths between versions
- Explore ways to make the rules more resistant to being overridden by the base model

## Contributing

This project is currently maintained by a single developer. Structured contributions and technical feedback will be considered once the core system reaches a more stable state.

## License

To be decided.

---

**Built to make custom AI actually usable long-term — not just impressive in short bursts.**
