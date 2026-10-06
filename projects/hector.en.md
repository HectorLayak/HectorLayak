# HECTOR

**Describe the need. Build the mechanics.**

[All projects](../README.en.md#the-whole-workshop) · [Français](hector.md)

HECTOR starts with an idea: authors should express expected behavior, constraints and permitted transformations. Types, units, effects and contracts make that intent explicit. The language also targets agents, whose proposals become inspectable by the compiler.

The project combines a language, a native compiler written in Hector and libraries consumed natively or through WebAssembly. Collections, ledgers and numerical kernels provide concrete applications. A lookup rule can lead to a scan or an index according to declared freedoms and workload.

The ambition is to compare implementations of the same behavior by time, memory or simplicity. The compiler and its contracts exist; research into behavioral equivalence and implementation selection continues.

## Journeys

1. Describe data, behavior and constraints.
2. Declare permitted transformations.
3. Inspect types, effects and contracts with the native compiler.
4. Integrate and measure the compiled kernel in its application.

## Design choices

### Behavior before mechanics

Declare values, results and obligations, along with permitted changes to representation, fusion or independent ordering.

### For humans and agents

Types, effects and contracts make proposals inspectable. An agent proposes a change; the compiler reports the contradictions it can detect.

### Reusable kernels

The same sources produce native and WebAssembly libraries. Interfaces and compiler identities accompany their integration into applications.

**Stage :** Applied research · native compiler and WebAssembly kernels.

[Studio & services ↗](https://floriansola.fr/en/projects/hector)
