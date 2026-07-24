# Layer 0: Mental Models & Computing Foundations

Chapter 00 establishes the baseline mental models needed before studying developer workflows, delivery systems, cloud infrastructure, containers, Kubernetes, platform engineering, production operations, security, reliability, architecture, and staff-level platform judgment.

This chapter follows the scope defined in [Blueprint v0.1](../BLUEPRINT-v0.1.md#00-layer-0--mental-models--computing-foundations) and provides the foundation for understanding the idea-to-production flow in the [System Map](../SYSTEM-MAP.md).

## Chapter purpose

Layer 0 helps learners reason about software systems from first principles. It introduces the core concepts behind computers, programs, operating systems, networks, storage, protocols, configuration, state, and production execution.

The purpose is not to teach every implementation detail. The purpose is to make later platform engineering topics easier to understand because the learner can identify the lower-level concepts underneath each abstraction.

## Why Layer 0 exists

Platform engineering sits on top of many layers of abstraction. A container depends on process isolation, filesystems, networking, image metadata, and runtime configuration. A deployment pipeline depends on source code, builds, artifacts, dependencies, credentials, and environments. A production system depends on compute, memory, storage, network paths, protocols, observability, and failure handling.

Layer 0 exists so learners do not treat these systems as magic. It creates a shared vocabulary for the rest of the Blueprint and helps learners ask better questions when a system is slow, broken, insecure, hard to operate, or difficult for developers to use.

## Expected outcome

After completing this chapter, learners should be able to:

- Explain how software runs on computers at a practical conceptual level.
- Describe how source code becomes a running program or service.
- Identify the roles of CPU, memory, storage, operating systems, processes, and threads.
- Explain how systems communicate using networks, DNS, HTTP, TLS, and load balancing.
- Distinguish common storage models such as filesystems, block storage, object storage, databases, and caches.
- Connect foundational concepts to the full path from idea to production.
- Use foundational mental models to reason about later Blueprint chapters.

## Prerequisites

This chapter assumes:

- Basic comfort using a computer, terminal, text editor, and web browser.
- Curiosity about how software systems work beneath high-level tools.
- Willingness to learn vocabulary gradually and connect concepts across modules.

No prior production engineering, cloud, Kubernetes, or platform engineering experience is required.

## Related Blueprint chapters

Layer 0 prepares learners for the rest of the Blueprint, especially:

- [01. Developer World](../BLUEPRINT-v0.1.md#01-developer-world)
- [02. Software Delivery](../BLUEPRINT-v0.1.md#02-software-delivery)
- [03. Cloud Foundations](../BLUEPRINT-v0.1.md#03-cloud-foundations)
- [04. Containers](../BLUEPRINT-v0.1.md#04-containers)
- [05. Kubernetes](../BLUEPRINT-v0.1.md#05-kubernetes)
- [06. Platform Engineering](../BLUEPRINT-v0.1.md#06-platform-engineering)
- [07. Operating Production Systems](../BLUEPRINT-v0.1.md#07-operating-production-systems)
- [08. Security](../BLUEPRINT-v0.1.md#08-security)
- [09. Reliability](../BLUEPRINT-v0.1.md#09-reliability)
- [10. Architecture](../BLUEPRINT-v0.1.md#10-architecture)

## Chapter files

- [Lesson roadmap](LESSONS.md)
- [Learning path](LEARNING-PATH.md)
- [Resources](RESOURCES.md)

## Lesson roadmap

### Module 1: Computing

1. What is Software?
2. What is a Computer?
3. Binary, Data and Information
4. CPU, Memory and Storage
5. Operating Systems
6. Processes and Threads

### Module 2: Programming

7. Source Code
8. Programming Languages
9. Compilation vs Interpretation
10. Build Systems
11. Dependencies
12. Libraries

### Module 3: Software Engineering

13. Software Architecture
14. Monolith vs Microservices
15. APIs
16. State
17. Configuration
18. Secrets

### Module 4: Networking

19. Networks
20. TCP/IP
21. DNS
22. HTTP
23. TLS
24. Load Balancing

### Module 5: Storage

25. Filesystems
26. Block Storage
27. Object Storage
28. Databases
29. Caching

### Module 6: End-to-End Journey

30. From Idea to Production
31. Developer Workflow
32. Git
33. CI/CD
34. Containers
35. Kubernetes
36. Production Systems
