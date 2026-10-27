
# Seyvo — Development Roadmap

Seyvo is an evidence-driven AI incident investigation platform designed to help engineers investigate application failures using structured logs, technical documentation, and controlled diagnostic tools.

## Engineering principles
- Evidence before conclusions.
- Deterministic analysis before model-generated reasoning.
- Incremental, testable components.
- Explicit uncertainty and traceable findings.
- Safe, permission-controlled tool execution.
- Reproducible evaluation and documented limitations.

## v0.1 — Incident Analysis Core
Status: Planned

- Parse and validate structured application logs.
- Handle malformed records and timestamp inconsistencies.
- Group related events and construct incident timelines.
- Produce deterministic summaries with evidence references.
- Add automated tests for core parsing and analysis.

## v0.2 — Backend and Persistence
Status: Planned

- Expose incident analysis through a validated REST API.
- Introduce persistent storage for incidents and evidence.
- Implement consistent error handling and API tests.

## v0.3 — LLM-Assisted Investigation
Status: Planned

- Integrate a language model through a bounded interface.
- Generate structured incident hypotheses grounded in evidence.
- Handle model errors, timeouts, and invalid responses.
- Compare model-assisted results against deterministic baselines.

## v0.4 — Knowledge Retrieval
Status: Planned

- Ingest technical runbooks and deployment documentation.
- Implement lexical and semantic search.
- Explore hybrid retrieval and reranking.
- Evaluate evidence relevance and citation accuracy.

## v0.5 — Investigation Workflows
Status: Planned

- Introduce controlled diagnostic tools.
- Support stateful, resumable investigations.
- Enforce authorization and human approval boundaries.
- Record tool activity for auditability.

## v1.0 — Reliability and Deployment
Status: Planned

- Build reproducible synthetic incident scenarios.
- Establish evaluation benchmarks and regression checks.
- Add observability, security controls, and automated CI.
- Package and deploy a documented demonstration.

## Out of scope for initial releases
- Autonomous production remediation.
- Unrestricted access to real infrastructure.
- Complex multi-agent orchestration without demonstrated need.
- Custom foundation-model training.

## Release policy
Milestones represent intended capabilities, not completed work. A release is complete only after its behavior, tests, and limitations have been verified.