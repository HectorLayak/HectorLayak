# HECTOR

**The agent programs the problem. Hector explores its realization.**

[All projects](../README.en.md#the-whole-workshop) · [Français](hector.md)

![HECTOR NEXT: intent, proposal and examination; admission remains separate](../assets/atelier/hector-en.svg)

HECTOR NEXT researches a different division of work: the author expresses intent, facts and domain rules; the agent proposes a change; Hector examines its consequences and the obligations it can check. The goal is to reduce the technical decisions left to agents.

The program is a typed, versioned graph with identities that survive renaming. Proposals target a precise revision. Text and Studio are representations of that program; the agent interface supports reading, exploration and proposals. Admission remains a separate act owned by the project owner.

## From intent to realization

1. Express domain facts and constraints.
2. Derive obligations and surface the missing domain question.
3. Examine a proposal and its impact against an identified base.
4. Distinguish an established result, counterexample, refusal and unknown conclusion.
5. Explore a native realization and measure it within its scope.

## Choices shaping the research

**The contract precedes its realization.** Domain rules do not implicitly choose an algorithm, memory representation or backend. Those decisions belong to realization work.

**Proposing is separate from admitting.** The CLI, MCP server and Studio share the program model, but reading or an agent’s proposal does not authorize integration.

**A guarantee has a scope.** Derivation, verification, counterexample search and measurement produce distinct results. An unknown result retains that state.

The toolchain combines **Rust, Hector and LLVM**. The kernel, editing tools, proof and native realization advance in bounded stages; Studio exposes the graph and proposals.

**Status: active research.** Complete journeys, multiplatform qualification and performance gains remain to be established.

[Project presentation ↗](https://floriansola.fr/en/projects/hector)
