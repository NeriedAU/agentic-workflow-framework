# The Agentic Workflow Framework

A tool-agnostic standard for how people and agents coordinate work, so that
agentic work is **trustworthy, consistent, repeatable, portable, and modular**
across personal, development, and operational domains.

The Framework is not a tool, not a workflow, and not a product. It is the shape
that work takes when the parties involved have agreed to use it. It defines what
must exist and how the parts must relate, never what they are built out of.
Implementations are free.

## The standard

The normative specification is **[FRAMEWORK.md](./FRAMEWORK.md)**. It is the
standard. It is written to be read in order, top to bottom.

It defines the four primitives (the Control, Specification, and Execution Planes,
and the Artefact), the invocation loop that binds them, the layered structure of
context, and the way workflows are defined and configured. An implementation is
**conformant** when it satisfies the *must / must not* rules for the primitive it
implements. A tool that conflates the responsibilities of multiple primitives is
not conformant.

Anything outside FRAMEWORK.md, including any reference implementation in this
repository, is **non-normative**. It may demonstrate the standard. It is not the
standard.

## Why it exists

Agentic work is most often coordinated by improvisation. As more work is handed
to agents, the same failure repeats: a single agent is given everything, loads
all context, holds every responsibility, and reaches its goal by whatever means
it can. It leaks across the boundaries between unrelated work and circumvents the
ones beneath it. None of it survives a change of contributor, tool, or scale.

The maturity of agentic work is not measured by how clever the model is. It is
measured by **how much of your craft you have moved out of the conversation and
into durable structure.**

| Level | Name | What has been externalised |
|---|---|---|
| 1 | **Consultation** | Nothing. The knowledge lives in your head and a throwaway chat. You transcribe the output by hand. |
| 2 | **Collaboration** | The context. The agent sees your code and you trade the wheel back and forth. It still dies with the session. |
| 3 | **Specialisation** | The procedure. Skills and subagents encode how a kind of work is done, reused across sessions. |
| 4 | **Orchestration** | The context-loading. A methodology decides what to know, and when, for a given input. |
| 5 | **Industrialisation** | The whole system. Blueprints, contracts resolved by identity, chained workflows. You manage the goals, not the code. |

The axis is **structure, not autonomy.** A maturity model that measures autonomy
asks how long the AI runs unattended and how far you trust it. This one asks how
much repeatable scaffolding surrounds the AI. Each level externalises one more
piece of the work out of the conversation and into something durable. The
Framework is what the top of that ladder is made of: its primitives are the
pieces you pull out, and its rules are how they hold together once you do.

## Status

Draft, under active development. The specification evolves through pull requests.
Changes to it are changes to the standard and are treated as such. Keep it tight:
no implementation detail, no organisation- or project-specific context.

## Licence

This repository is dual-licensed.

- The specification (**FRAMEWORK.md** and all normative text) is licensed under
  [Creative Commons Attribution-ShareAlike 4.0 International](./LICENSE-SPEC)
  (CC BY-SA 4.0).
- All code and reference implementations are licensed under the
  [MIT Licence](./LICENSE-CODE).

Author: Ash Rowe.
