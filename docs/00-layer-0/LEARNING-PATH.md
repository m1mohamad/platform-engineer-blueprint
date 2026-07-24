# Layer 0 learning path

This learning path describes how to study Chapter 00: Layer 0 — Mental Models & Computing Foundations before moving into the rest of the Platform Engineer Blueprint.

Layer 0 should be studied alongside the chapter scope in [Blueprint v0.1](../BLUEPRINT-v0.1.md#00-layer-0--mental-models--computing-foundations) and the end-to-end delivery model in the [System Map](../SYSTEM-MAP.md).

## Recommended study order

Study the modules in sequence because each module introduces vocabulary used by the next one:

1. **Computing**: Build the base model for software, computers, data, hardware resources, operating systems, and execution.
2. **Programming**: Connect source code, languages, builds, dependencies, and libraries to the way software is created.
3. **Software Engineering**: Learn the concepts that shape application boundaries, interfaces, configuration, state, and secret handling.
4. **Networking**: Understand how systems communicate across hosts, services, and user-facing boundaries.
5. **Storage**: Learn how data is persisted, accessed, cached, and modeled through common storage primitives.
6. **End-to-End Journey**: Tie the foundations together by following a change from idea to production.

## Estimated duration

A steady pace for this chapter is **three to six weeks**, depending on prior experience:

- **Three weeks** for learners who already have basic programming or operations experience.
- **Four to five weeks** for learners who are new to infrastructure and production systems.
- **Six weeks** for learners who want extra review time before continuing to later chapters.

The goal is not to memorize every term. The goal is to build enough mental models to reason clearly about the later chapters on developer workflows, software delivery, cloud foundations, containers, Kubernetes, platform engineering, operations, security, reliability, and architecture.

## Daily study approach

Use short, consistent study sessions:

1. Read one planned lesson topic or one small cluster of closely related topics.
2. Write a brief explanation of the concept in your own words.
3. Draw the boundary between the concept and the systems around it.
4. Connect the concept to one stage in the [System Map](../SYSTEM-MAP.md#stage-reference-map).
5. Capture open questions for later lessons instead of trying to solve every detail immediately.

A practical daily target is **30 to 60 minutes** of focused study, with one longer weekly review session to revisit diagrams, definitions, and connections across modules.

## Hands-on expectations

Layer 0 should remain concept-first, but learners should still verify ideas with small experiments where possible. Examples of appropriate hands-on practice include:

- Inspecting files, processes, environment variables, ports, and local network behavior.
- Tracing how a simple program moves from source code to a runnable process.
- Observing requests with browser developer tools or command-line clients.
- Comparing local files, object-like storage concepts, database behavior, and cache behavior at a high level.
- Mapping a small application change onto the idea-to-production journey.

Hands-on work should support the mental model. It should not become a deep tool tutorial in this chapter.

## Interview preparation strategy

Use Layer 0 to build clear first-principles answers:

- Practice explaining each lesson title in two forms: a short interview answer and a deeper systems answer.
- Connect every answer to resource constraints, failure modes, ownership, and operational tradeoffs.
- Prefer simple diagrams when explaining flows such as a request path, a build path, or data moving through storage.
- Use the end-to-end module to practice narrating how a change becomes production software.
- Keep a personal glossary of terms that appear again in later Blueprint chapters.

A strong interview outcome for this chapter is the ability to explain unfamiliar platform topics by decomposing them into compute, networking, storage, software delivery, configuration, state, and operational behavior.
