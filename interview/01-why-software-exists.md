# Why software exists interview questions

These questions assess whether a candidate can reason from human need to software behavior, then connect that reasoning to platform engineering abstractions. They progress from junior-level fundamentals to staff-level system judgment.

## 1. Junior: Why does software exist?

### Expected answer

Software exists to turn human needs into repeatable machine behavior. Humans define a problem, engineers describe the steps to solve it, and computers execute those steps through software.

### Deep dive

A strong answer separates the human goal from the machine execution. The goal might be communication, automation, calculation, storage, coordination, or control. Software provides the rules and sequence that make hardware useful for that goal.

### Follow-up questions

- What is an example of a human need that software solves?
- Why is repeatability important?

### Common mistakes

- Saying software exists only to make computers run.
- Defining software only as code without mentioning behavior or outcomes.

## 2. Junior: Why is hardware alone not enough?

### Expected answer

Hardware provides physical capability, but it does not understand human intent. A CPU, memory, disk, or network card can perform operations, but software decides which operations should happen, in which order, and under which rules.

### Deep dive

Hardware is general-purpose. The same machine can run a web server, database, game, compiler, or deployment system depending on the software installed. Software gives the hardware purpose.

### Follow-up questions

- What can a CPU do without a program?
- Why is a general-purpose computer valuable?

### Common mistakes

- Treating hardware as if it understands business concepts.
- Ignoring the role of instructions and state.

## 3. Junior: What is an algorithm?

### Expected answer

An algorithm is a sequence of steps and decisions used to solve a problem. It can be written in plain language, a diagram, pseudocode, or source code.

### Deep dive

Algorithms are not limited to math. A deployment rollout, password reset flow, incident escalation process, or retry policy can all be described algorithmically. The key idea is ordered behavior with conditions.

### Follow-up questions

- Give an algorithm for making a cup of tea.
- How does an algorithm become software?

### Common mistakes

- Defining algorithms only as complex equations.
- Forgetting that algorithms include decision points.

## 4. Junior to mid-level: Why do programming languages exist?

### Expected answer

Programming languages let humans express behavior at a higher level than machine instructions. They provide structure, syntax, libraries, and rules that make software easier to write, read, test, and maintain.

### Deep dive

Different languages expose different tradeoffs. Some prioritize low-level control and performance. Others prioritize safety, productivity, portability, or ecosystem. A language is an abstraction over machine behavior, not a replacement for systems understanding.

### Follow-up questions

- Why not write all software directly in machine code?
- How can language choice affect operations?

### Common mistakes

- Claiming one language is universally best.
- Focusing only on syntax instead of maintainability and runtime behavior.

## 5. Mid-level: Why do operating systems exist?

### Expected answer

Operating systems manage hardware resources and provide common abstractions for applications. They handle CPU scheduling, memory isolation, files, devices, networking, permissions, and system calls.

### Deep dive

Without an operating system, every application would need to manage hardware directly and coordinate with other programs. Operating systems make application development safer and more consistent by centralizing resource management.

### Follow-up questions

- What operating system features do containers rely on?
- How can operating system limits affect an application in production?

### Common mistakes

- Describing the operating system only as a user interface.
- Ignoring isolation, scheduling, permissions, and resource management.

## 6. Mid-level: What is abstraction, and what problem does it solve?

### Expected answer

Abstraction hides lower-level detail behind a simpler interface so humans can reason about complex systems. It reduces cognitive load and makes larger systems possible.

### Deep dive

Abstractions are useful when they preserve the important behavior while hiding unnecessary detail. They become dangerous when they hide failure modes, ownership boundaries, performance costs, or security responsibilities that engineers still need to understand.

### Follow-up questions

- Give an example of a useful platform abstraction.
- When can abstraction make debugging harder?

### Common mistakes

- Assuming abstraction removes complexity instead of moving or organizing it.
- Treating hidden details as irrelevant.

## 7. Mid-level: How does source code become machine behavior?

### Expected answer

Source code is translated by a compiler or interpreter into instructions the machine can execute. The running program then uses operating system services and hardware resources to produce observable behavior.

### Deep dive

The exact path depends on the language and runtime. Some code is compiled ahead of time, some is interpreted, and some uses virtual machines or just-in-time compilation. In all cases, human-readable instructions must eventually produce lower-level operations that hardware can execute.

### Follow-up questions

- What is the difference between source code and a build artifact?
- Why can code work locally but fail in production?

### Common mistakes

- Assuming source code is what the CPU directly executes.
- Ignoring runtime dependencies and environment differences.

## 8. Senior: How does CI relate to the purpose of software?

### Expected answer

Continuous integration is software that automates checks humans want applied consistently. It turns team expectations into repeatable validation, such as tests, linting, builds, scans, and policy checks.

### Deep dive

CI exists because manual validation does not scale well across teams, repositories, and frequent changes. A senior answer should mention feedback speed, reproducibility, trust, auditability, and the limits of CI. CI increases confidence, but it does not prove that a system is correct in every production condition.

### Follow-up questions

- What should CI validate before a change is merged?
- How can slow CI harm engineering behavior?

### Common mistakes

- Treating CI as only a tool configuration problem.
- Confusing passing CI with production readiness.

## 9. Senior: Why are containers and Kubernetes abstractions rather than destinations?

### Expected answer

Containers package software and dependencies into a more repeatable runtime unit. Kubernetes coordinates desired state for workloads across infrastructure. They are abstractions that help deliver and operate software, not the original reason the software exists.

### Deep dive

A senior answer should connect containers to operating system isolation and packaging, and Kubernetes to reconciliation, scheduling, health checks, rollout behavior, service discovery, and resource management. The value is not using Kubernetes itself; the value is reliable software delivery and operation.

### Follow-up questions

- What complexity does Kubernetes hide?
- What complexity does Kubernetes introduce?

### Common mistakes

- Describing containers as lightweight virtual machines without nuance.
- Treating Kubernetes adoption as automatically beneficial.

## 10. Staff: How should a platform engineer evaluate a new abstraction?

### Expected answer

A platform engineer should evaluate whether the abstraction reduces cognitive load, improves reliability or delivery speed, preserves necessary control, exposes the right failure signals, fits team ownership, and is worth its operational cost.

### Deep dive

A staff-level answer frames abstraction as an organizational design decision, not only a technical choice. Good abstractions create paved roads, clarify responsibilities, standardize safe defaults, and make common work easier. Bad abstractions hide important details, create dependency bottlenecks, increase incident blast radius, or force teams into workflows that do not match their needs.

### Follow-up questions

- How would you measure whether a platform abstraction is successful?
- When should a team be allowed to bypass a platform abstraction?
- How do you deprecate a harmful abstraction safely?

### Common mistakes

- Optimizing only for elegance or tool popularity.
- Ignoring ownership, migration cost, support load, and production failure modes.

## Staff engineer perspective

At staff level, the central question is not whether software, CI, containers, Kubernetes, or cloud services are interesting. The question is whether each layer helps the organization convert human needs into reliable production outcomes with acceptable cost, risk, security, and cognitive load.
