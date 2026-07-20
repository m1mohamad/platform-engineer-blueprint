# Blueprint v0.1

Blueprint v0.1 is the frozen architecture for the Platform Engineer Blueprint. It defines the chapters, their purpose, their learning goals, and the topics each chapter is responsible for covering. It does not define lessons, exercises, or implementation-specific content.

The blueprint is ordered from foundational mental models to advanced platform engineering judgment. Later content should fit into this structure without changing the meaning of the v0.1 chapters.

## Chapter Index

| Chapter | Title |
| --- | --- |
| 00 | Layer 0 — Mental Models & Computing Foundations |
| 01 | Developer World |
| 02 | Software Delivery |
| 03 | Cloud Foundations |
| 04 | Containers |
| 05 | Kubernetes |
| 06 | Platform Engineering |
| 07 | Operating Production Systems |
| 08 | Security |
| 09 | Reliability |
| 10 | Architecture |
| 11 | Staff Platform Engineer |
| 12 | Interview Playbook |
| 13 | Engineering Stories |
| 14 | History |
| 99 | Future Topics |

## 00. Layer 0 — Mental Models & Computing Foundations

### Purpose

Establish the foundational concepts required to reason about software systems before introducing delivery platforms, cloud infrastructure, or production operations.

### Learning Goal

Learners should be able to explain how computers, networks, processes, storage, protocols, and abstractions interact, and use those concepts to reason about higher-level platform systems.

### Main Topics

- Systems thinking and abstraction layers.
- Processes, memory, files, and operating system basics.
- Networking fundamentals, including IP, DNS, ports, routing, latency, and packet flow.
- HTTP, TLS, APIs, and common application protocols.
- Resource constraints such as CPU, memory, disk, network, and concurrency.
- Failure modes, queues, backpressure, retries, and timeouts.
- Tradeoffs between simplicity, performance, correctness, and operability.

## 01. Developer World

### Purpose

Explain the environment in which software engineers create, run, test, and collaborate on application code.

### Learning Goal

Learners should understand the developer workflow well enough to identify friction, design useful platform abstractions, and preserve fast feedback loops.

### Main Topics

- Local development environments.
- Editors, terminals, shells, package managers, and language runtimes.
- Application structure and dependency management.
- Testing during development.
- Configuration for local execution.
- Developer onboarding and productivity.
- Collaboration between application teams and platform teams.

## 02. Software Delivery

### Purpose

Describe how source code becomes a tested, versioned, releasable software artifact.

### Learning Goal

Learners should be able to trace a change from commit to release candidate and understand the systems that validate, build, package, and promote software.

### Main Topics

- Git concepts and collaboration workflows.
- Branching, pull requests, reviews, and merge strategies.
- Continuous integration.
- Automated testing and quality gates.
- Build systems and reproducible builds.
- Artifact repositories and release metadata.
- Versioning, promotion, and deployment readiness.

## 03. Cloud Foundations

### Purpose

Introduce the cloud primitives that platform engineers use to run and connect production systems.

### Learning Goal

Learners should understand core cloud services and be able to reason about infrastructure design, ownership, cost, security boundaries, and operational constraints.

### Main Topics

- Compute, storage, networking, identity, and regions.
- Virtual networks, subnets, routing, load balancers, and firewalls.
- Managed services and shared responsibility.
- Infrastructure as code.
- Environments, accounts, projects, and subscriptions.
- Cost management, quotas, limits, and governance.
- Cloud reliability and regional failure considerations.

## 04. Containers

### Purpose

Explain how applications are packaged, distributed, and executed using container technology.

### Learning Goal

Learners should understand container images, registries, runtimes, and operational implications well enough to design predictable application packaging workflows.

### Main Topics

- Container image layers and metadata.
- Dockerfiles and image build practices.
- Build context, caching, and reproducibility.
- Container registries and image promotion.
- Runtime isolation and process models.
- Configuration, secrets, volumes, and networking.
- Image security, scanning, and provenance.

## 05. Kubernetes

### Purpose

Describe Kubernetes as a common orchestration layer for running containerized workloads and building platform abstractions.

### Learning Goal

Learners should understand how Kubernetes schedules, configures, exposes, and reconciles workloads, and how platform teams use it as a substrate for higher-level capabilities.

### Main Topics

- Cluster architecture and control plane concepts.
- Nodes, pods, deployments, stateful sets, jobs, and daemon sets.
- Services, ingress, gateways, and network policies.
- ConfigMaps, secrets, storage, and service accounts.
- Controllers, reconciliation, scheduling, and desired state.
- Deployment strategies and workload health.
- Kubernetes operational risks and platform boundaries.

## 06. Platform Engineering

### Purpose

Define platform engineering as the discipline of building internal systems that improve software delivery and production operations for engineering teams.

### Learning Goal

Learners should be able to explain what platforms provide, how they are designed as products, and how they balance standardization with team autonomy.

### Main Topics

- Internal developer platforms.
- Golden paths, paved roads, and self-service workflows.
- Platform APIs, portals, templates, and automation.
- Developer experience and platform product management.
- Team topology, ownership, and operating models.
- Governance without unnecessary friction.
- Measuring platform adoption, reliability, and outcomes.

## 07. Operating Production Systems

### Purpose

Explain the practices required to run software safely after it is deployed.

### Learning Goal

Learners should understand how production systems are observed, changed, supported, and improved during normal operation and incidents.

### Main Topics

- Production readiness.
- Deployments, rollbacks, rollouts, and change management.
- Monitoring, logging, tracing, and alerting.
- Incident response, escalation, and communication.
- Runbooks, playbooks, and operational ownership.
- Capacity management and performance investigation.
- Post-incident review and continuous improvement.

## 08. Security

### Purpose

Integrate security into the full software delivery and platform lifecycle.

### Learning Goal

Learners should understand how platform systems reduce risk through identity, policy, secure defaults, supply chain controls, and runtime protections.

### Main Topics

- Identity and access management.
- Secrets management and key rotation.
- Secure software delivery and CI/CD hardening.
- Dependency, artifact, and container image security.
- Software supply chain integrity and provenance.
- Network segmentation and runtime controls.
- Policy, compliance, auditability, and threat modeling.

## 09. Reliability

### Purpose

Explain how engineering teams define, measure, and improve the dependability of production systems.

### Learning Goal

Learners should be able to reason about reliability goals, failure modes, service behavior, and the engineering practices that improve system resilience.

### Main Topics

- Service-level indicators, objectives, and agreements.
- Error budgets and reliability decision-making.
- Availability, latency, durability, and correctness.
- Capacity planning and load behavior.
- Resilience patterns, redundancy, graceful degradation, and failover.
- Chaos engineering and failure injection.
- Reliability reviews and learning from incidents.

## 10. Architecture

### Purpose

Develop the architectural judgment required to design, evolve, and operate complex software and platform systems.

### Learning Goal

Learners should be able to evaluate architecture through tradeoffs, boundaries, dependencies, failure modes, team ownership, and long-term operability.

### Main Topics

- Architectural principles and decision records.
- Distributed systems concepts.
- Service boundaries, APIs, data ownership, and integration patterns.
- Coupling, cohesion, dependency management, and migration strategy.
- Scalability, consistency, latency, and resilience tradeoffs.
- Platform architecture and capability design.
- Evolutionary architecture and technical debt management.

## 11. Staff Platform Engineer

### Purpose

Describe the expectations, behaviors, and judgment required of senior platform engineers operating beyond individual implementation tasks.

### Learning Goal

Learners should understand how staff-level engineers influence technical direction, align stakeholders, mentor teams, and improve systems across organizational boundaries.

### Main Topics

- Technical strategy and platform vision.
- Cross-team influence and stakeholder alignment.
- Written communication, proposals, and decision-making.
- Mentorship, standards, and engineering culture.
- Navigating ambiguity and constraints.
- Prioritization, sequencing, and risk management.
- Measuring impact beyond direct code contributions.

## 12. Interview Playbook

### Purpose

Provide a structured way to prepare for platform engineering interviews without reducing the field to memorized answers.

### Learning Goal

Learners should be able to communicate platform engineering experience clearly, solve system design problems, reason through operational scenarios, and present credible engineering stories.

### Main Topics

- Platform engineering interview formats.
- System design prompts and evaluation criteria.
- CI/CD, Kubernetes, cloud, security, reliability, and operations scenarios.
- Behavioral interview storytelling.
- Debugging and incident response exercises.
- Senior-level communication and tradeoff framing.
- Portfolio and resume alignment.

## 13. Engineering Stories

### Purpose

Use realistic engineering narratives to connect abstract concepts with practical decisions, constraints, and outcomes.

### Learning Goal

Learners should recognize how platform engineering problems appear in real organizations and how technical decisions interact with people, process, risk, and time.

### Main Topics

- Migration stories.
- Incident stories.
- Platform adoption stories.
- Delivery bottleneck stories.
- Reliability improvement stories.
- Security remediation stories.
- Tradeoff analysis and decision consequences.

## 14. History

### Purpose

Explain how historical practices and industry changes shaped modern platform engineering.

### Learning Goal

Learners should understand the evolution from traditional operations to DevOps, SRE, cloud-native systems, and internal developer platforms.

### Main Topics

- System administration and early operations practices.
- Build and release engineering.
- Agile, continuous delivery, and DevOps.
- Cloud computing and infrastructure automation.
- Containers and orchestration.
- Site reliability engineering.
- Internal developer platforms and platform engineering as a discipline.

## 99. Future Topics

### Purpose

Reserve space for emerging topics that are relevant to platform engineering but not yet stable enough to become part of the core blueprint.

### Learning Goal

Learners should understand which areas are evolving and how to evaluate new practices before adopting them as durable engineering principles.

### Main Topics

- AI-assisted software delivery and operations.
- Emerging runtime and deployment models.
- Evolving supply chain security practices.
- New infrastructure abstractions.
- Developer experience measurement techniques.
- Platform engineering research and industry trends.
- Candidate topics for future blueprint revisions.
