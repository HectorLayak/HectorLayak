![HectorLayak — Understand. Build. Bring to life.](assets/showcase/hero-en.svg)

<p align="center"><a href="#selected-projects">Six projects</a> · <a href="#the-workshop-map">The map</a> · <a href="#the-whole-workshop">33 projects</a> · <a href="https://floriansola.fr/en">Studio &amp; services ↗</a> · <a href="README.md">Français</a></p>

I build applied AI tools, .NET platforms and real-time systems. My projects explore agent orchestration, executable contracts, networking engines and simulation, with one recurring concern: keeping state, performance and component boundaries explicit.

**C# / .NET · Rust · Python · TypeScript · C / C++**

## Selected projects

[![AINDEX — Agents do the work. Humans oversee the project.](assets/showcase/aindex-en.svg)](projects/aindex.en.md)

AINDEX organizes agent work around the project: missions, repository context, changes and verification. A Rust engine owns the project authority; Studio gives humans a shared view for supervision and decisions.

<details>
<summary>Architecture and journey</summary>

**One project authority.** The Rust engine owns tasks, reservations, validation and provenance. Studio, the extension and the gateway present these contracts, keeping every interface aligned with the same authority.

**Context at the point of work.** A capsule combines the complete mission contract with selected current references. A host adapter can supply it on work events; aindex_context provides a reading entry point when a refresh is needed.

1. Connect an objective to a mission, its scope and the repository’s rules.
2. Give the agent useful context when work happens: contracts, dependencies, references and observed state.
3. Follow changes and agent activity through the supervision components shared by Studio and its viewers.
4. Inspect verification results, resolve contradictions and make the integration decision.

</details>

[Explore the project ↗](projects/aindex.en.md)

[![HECTOR — A language for expressing behavior, compiling it and inspecting contracts.](assets/showcase/hector-en.svg)](projects/hector.en.md)

HECTOR is a language and native compiler for human authors and agents. Types, effects and contracts accompany business kernels targeting native execution and WebAssembly.

<details>
<summary>Architecture and journey</summary>

**The compiler owns semantics.** The json, syntax, foundation, core and driver units are written in Hector. Bootstrap rebuilds the chain from its seeds; LLVM handles native emission. Launchers direct work to the same authority.

**Observable contracts.** Preconditions, postconditions, effects and source identities accompany analysis and execution. Checker facts feed selection and compatibility checks against a reference.

1. Express behavior in Hector with its types, effects and contract clauses.
2. Analyze sources with the native compiler and inspect facts produced by the checker.
3. Build a native or WebAssembly library for an external consumer.
4. Compare interfaces and publication properties, then qualify the workflow on its target host.

</details>

[Explore the project ↗](projects/hector.en.md)

[![OneRP — A SaaS foundation for operating FiveM roleplay worlds.](assets/showcase/onerp-framework-en.svg)](projects/onerp-framework.en.md)

OneRP brings a SaaS backend, administration and FiveM modules together. Characters, economy, inventory, vehicles, housing and activities share reactive business services and in-game React interfaces.

<details>
<summary>Architecture and journey</summary>

**Reactive business state.** Fusion tracks read dependencies. Mutations invalidate the relevant data, while player-scoped sentinels keep recomputation focused on the useful scope.

**Transactional economic operations.** Mutation templates open operation contexts and provide serializable isolation for concurrent writes. Instance filters and read guards support business services.

1. Create and configure a server instance in the administration panel.
2. Welcome players, select a character and guide their arrival.
3. Interact with jobs, inventory, banking, vehicles and housing.
4. Validate actions through server business services.
5. Follow state changes and manage instances through connected interfaces.

</details>

[Explore the project ↗](projects/onerp-framework.en.md)

[![StaffingOS — Connect assignments, time, expenses and financial preparation.](assets/showcase/staffingos-en.svg)](projects/staffingos.en.md)

StaffingOS connects client assignments, time, expenses and absences to approvals and financial preparation. Worker and management workspaces share records and access rules.

<details>
<summary>Architecture and journey</summary>

**Shared records, distinct responsibilities.** Workers, managers, HR and accounting act on shared records with explicit permissions and scopes. Assignment, time and absence rules are shared across interfaces.

**Traceable operations.** Assignment creation records a command fingerprint, versions, audit and durable events in one transaction. Recovery distinguishes new work from replay of an existing operation.

1. Record the client, site, requirement and assigned person.
2. Create the assignment with dates and versioned rates.
3. Submit time, expenses and absence requests through authorised workspaces.
4. Review requests and exceptions through approval workflows.
5. Prepare payroll and preinvoice batches, then record payment evidence.

</details>

[Explore the project ↗](projects/staffingos.en.md)

[![RoadTripper — A shared itinerary, a map and a copilot for travelling together.](assets/showcase/roadtripper-en.svg)](projects/roadtripper.en.md)

A shared travel notebook for planning each day, exploring places on a map, organising the group and tracking expenses. The copilot proposes changes for travellers to review before adopting them.

<details>
<summary>Architecture and journey</summary>

**Keep the day as the anchor.** The overview, itinerary and map share the selected day and stop identifiers. On mobile, the next action comes before secondary tools, and a stop opens for reading before editing.

**Share calculations across client and server.** The notebook domain is independent of the interface. Hector, compiled to WebAssembly, provides deterministic planning, budget and progress calculations; the gateway validates incoming data again.

1. Build the trip — Create a notebook with dates and preferences, organise stops by day, and add places, breaks and overnight stays.
2. Move between itinerary and map — Select a day, inspect a stop and find it on the map without losing the selection. Calculate or refresh a route when a provider is configured.
3. Prepare together — Invite members with a role, assign travellers to cars, review departure preparation and collect reservations, documents and the budget.
4. Adapt the itinerary — Suggest a place to the group or ask the copilot for a detour. Review changes against the current notebook before adopting them, and share location only with consent.
5. Keep expenses clear — Record expenses, their shares and declared reimbursements, while keeping committed, estimated and recorded amounts distinct.

</details>

[Explore the project ↗](projects/roadtripper.en.md)

[![Poisson Engine — A living ecosystem simulated in the browser.](assets/showcase/poisson-engine-en.svg)](projects/poisson-engine.en.md)

Poisson simulates schooling, predation, metabolism and mutations in the browser. The engine separates WebGPU/CPU compute from WebGL/Canvas2D rendering and supports observation, sandbox and gameplay modes.

<details>
<summary>Architecture and journey</summary>

**Compute and rendering adapt independently.** WebGPU accelerates simulation compute, with a CPU path when unavailable. Rendering chooses WebGL or Canvas2D. This separation adapts both workload and presentation to browser capabilities.

**Organize data for parallel execution.** Typed arrays, SoA data, spatial grids, prefix sums and reordering bring neighboring agents closer in memory. The GPU pipeline handles schooling and hunting forces before physics integration.

1. Choose a mode and observe schools, predators and ecosystem resources.
2. Adjust parameters and follow their effects on movement, energy and reproduction.
3. Explore genetics, mutations and relationships between species.
4. Play with progression, abilities, missions and the economy, or inspect the simulation.

</details>

[Explore the project ↗](projects/poisson-engine.en.md)

## The workshop map

![Code, products, worlds and operations; Hector provides RoadTripper’s WASM engine.](assets/showcase/ecosystem-en.svg)

**A concrete connection between areas:** RoadTripper uses Hector through WebAssembly for planning, budget and progress calculations.

## The whole workshop

**33 projects**, organized into four areas. Products, research, tools and collaborations.

<details>
<summary><strong>Languages, AI & agents</strong> · 9 projects</summary>

| Project | Domain |
| :--- | :--- |
| [AINDEX](projects/aindex.en.md) | Agents do the work. Humans oversee the project. |
| [HECTOR](projects/hector.en.md) | A language for expressing behavior, compiling it and inspecting contracts. |
| [Continuum](projects/continuum.en.md) | Learn to navigate, then measure decisions in a reproducible laboratory. |
| [PromptVault](projects/promptvault.en.md) | Turn a team’s prompts into reusable tools |
| [Matchr](projects/matchr.en.md) | One offer, a targeted CV and a tracked application dossier. |
| [ModelRisk Observatory · GeopolAI](projects/geopolai.en.md) | Compare AI-model responses under controlled scenarios |
| [AISelector](projects/ai-selector.en.md) | One contract for multiple AI providers |
| [Vouch](projects/vouch.en.md) | Prepare security answers from traceable sources |
| [Vision Security Lab](projects/vision-security-lab.en.md) | Observe automated behaviour from visual input. |

</details>

<details>
<summary><strong>Business products & collaboration</strong> · 6 projects</summary>

| Project | Domain |
| :--- | :--- |
| [OneRP](projects/onerp-framework.en.md) | A SaaS foundation for operating FiveM roleplay worlds. |
| [SaleCast](projects/salecast.en.md) | Connect sales channels and plan the next replenishment. |
| [StaffingOS](projects/staffingos.en.md) | Connect assignments, time, expenses and financial preparation. |
| [RoadTripper](projects/roadtripper.en.md) | A shared itinerary, a map and a copilot for travelling together. |
| [PartyFlow](projects/partyflow.en.md) | Create a room, gather players and move through timed challenges |
| [Racine](projects/racine.en.md) | A family space for connections and shared memories |

</details>

<details>
<summary><strong>Worlds, games & simulation</strong> · 13 projects</summary>

| Project | Domain |
| :--- | :--- |
| [FantasyOnline](projects/fantasy-online.en.md) | A persistent fantasy world, from generated terrain to server rules. |
| [FantasyOnline.Shared](projects/fantasy-online-shared.en.md) | Share contracts and rules through explicit adoption by each game. |
| [Nexus / Reclaim City](projects/nexus.en.md) | Recover wrecks and rebuild a district of your own. |
| [SurvivalKingdom](projects/survival-kingdom.en.md) | Connect survival, a multiplayer world and the services that sustain it. |
| [SurvivalUnreal](projects/survival-unreal.en.md) | A survival world connected to its own game services. |
| [REWORLD](projects/reworld.en.md) | Build an atlas, connect its territories and write their story. |
| [MANDATE EARTH](projects/mandate-earth.en.md) | Prepare a plan, commit resources and track the consequences. |
| [Symbiont](projects/symbiont.en.md) | Grow a colony without exhausting the world that feeds it. |
| [Poisson Engine](projects/poisson-engine.en.md) | A living ecosystem simulated in the browser. |
| [Ultra RP](projects/ultra-rp-sbox.en.md) | A s&box roleplay world, from player jobs to operations tooling |
| [Development Tycoon](projects/development-tycoon.en.md) | Design the growth of a software studio as a management game. |
| [Red Dead Roleplay](projects/red-dead-roleplay.en.md) | Compose a roleplay world around characters and interactions. |
| [V-Multi / SARP](projects/gaming-platform.en.md) | A formative journey through multiplayer and community worlds. |

</details>

<details>
<summary><strong>Infrastructure, tools & background</strong> · 5 projects</summary>

| Project | Domain |
| :--- | :--- |
| [VPS Command Center](projects/vps-command-center.en.md) | Connect service health to operational decisions. |
| [Self-hosted Infrastructure](projects/self-hosted-infrastructure.en.md) | Organise product hosting, delivery and recovery. |
| [Portfolio Engineering](projects/portfolio-engineering.en.md) | Turn recurring problems into reusable components. |
| [Gecko IoT](projects/gecko-iot.en.md) | Professional experience close to embedded software. |
| [Integrations & Archives](projects/integrations-archives.en.md) | Preserve adapters, experiments and early versions. |

</details>

---

[Studio & services](https://floriansola.fr/en) · [Notes and articles](https://floriansola.fr/en/blog) · [Français](README.md)
