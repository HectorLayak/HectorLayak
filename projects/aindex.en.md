# AINDEX

**Agents do the work. Humans oversee the project.**

[All projects](../README.en.md#the-whole-workshop) · [Français](aindex.md)

![AINDEX: mission, project-authority engine and human supervision](../assets/atelier/aindex-en.svg)

Delegating development to agents means connecting each change to a request, authorized files and verification. AINDEX brings those elements together: goals, missions, code context, execution and reviewable results.

The Rust engine indexes symbols and their relationships. It also owns project authority: tasks, permissions, work reservations and validation. The context layer supplies the mission contract and useful references, then rereads project state on resumption. Reading context does not grant permission to change code.

## A mission connected to the project

1. Connect the request to a goal, scope and repository rules.
2. Provide the contracts, dependencies, references and observations useful to the work.
3. Follow activity, changes and verification through shared supervision.
4. Examine the resulting evidence and decide what comes next.

## Separate responsibilities

**The engine owns authority.** Studio, the editor extension and readers present project contracts; they do not recreate a competing version of Project/Gate’s truth.

**Context remains an observation.** Its origin and freshness matter to the mission. It does not replace permissions or validation.

**The commercial account does not own the repository.** Accounts, licenses, teams and PostgreSQL billing remain separate from code permissions. The gateway exposes only authorized private reads.

Demonstration mode is explicitly selected when the engine is unavailable. Demo screens contain fictional data and are not a measured result on a real project.

**Status: in development.** Native engine, human supervision and editor extension; productivity and token savings require measurement across a complete mission.

[Project presentation ↗](https://floriansola.fr/en/projects/aindex)
