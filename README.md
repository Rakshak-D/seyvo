# Seyvo

**Evidence-driven AI incident investigation**

Seyvo is a public engineering project exploring how software failures can be investigated using structured logs, retrieval systems, and evidence-grounded AI workflows.

The goal is to build an investigation platform that helps developers understand application failures, examine supporting evidence, and develop verifiable root-cause hypotheses.

## Project Status

**Early development — foundational architecture and documentation.**

The application is being developed incrementally. Core incident-analysis functionality has not yet been implemented.

## Planned Capabilities

- **Incident analysis:** Parse, validate, and correlate application logs.
- **LLM-assisted investigation:** Generate structured hypotheses grounded in evidence.
- **Knowledge retrieval:** Search technical documentation and incident runbooks.
- **Agentic workflows:** Perform controlled diagnostic operations.
- **Evaluation:** Measure investigation accuracy, evidence quality, and reliability.
- **Production engineering:** Implement testing, observability, security, and deployment practices.

## Engineering Principles

1. Evidence before conclusions.
2. Deterministic baselines before LLM-based reasoning.
3. Testable and maintainable components.
4. Explicit uncertainty and traceable findings.
5. Secure, permission-controlled operations.
6. Reproducible evaluation.

## Development Roadmap

| Version | Focus |
|---|---|
| v0.1 | Incident parsing and deterministic analysis |
| v0.2 | Backend APIs and persistence |
| v0.3 | LLM-assisted investigation |
| v0.4 | Retrieval and evidence grounding |
| v0.5 | Stateful investigation workflows |
| v1.0 | Evaluation, reliability, and deployment |

See the [Development Roadmap](docs/ROADMAP.md) for details.

## Architecture Decisions

Technical decisions and trade-offs are documented in the [Architecture Decision Log](docs/DECISIONS.md).

## Getting Started

Development setup and execution instructions will be added when the first runnable application milestone is implemented.

## Project Scope

Initial development uses synthetic incident data. Seyvo is not currently intended for autonomous remediation or unrestricted access to production infrastructure.

## License

A license has not yet been selected.