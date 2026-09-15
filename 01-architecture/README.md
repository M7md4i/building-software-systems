# Architecture

Architecture is the set of decisions that shape boundaries, dependencies, data ownership, deployment, and change over time.

## Topics

- Modular monoliths
- Layered architecture
- Clean Architecture
- Vertical Slice Architecture
- Hexagonal architecture
- Domain boundaries
- Dependency direction
- Architecture Decision Records (ADRs)
- Coupling and cohesion
- Evolutionary architecture

## Questions to ask

- What is the unit of change?
- Which modules own which data?
- Which dependencies are allowed?
- Where do cross-cutting concerns live?
- Which decisions are difficult to reverse?
- Does deployment topology match logical boundaries?
- Is the architecture simpler than the problem it solves?

## Production rule

Do not introduce distributed-system complexity to solve an organizational or code-structure problem that can be handled inside a modular monolith.