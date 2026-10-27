
# Seyvo — Architecture Decision Log

This document records important engineering decisions,
their rationale, alternatives, and trade-offs.

Decisions may be revised as requirements evolve.

## ADR-001: Deterministic Analysis Before LLM Integration

Status: Accepted

### Context
LLM-generated incident explanations can be inaccurate
and difficult to verify without reliable evidence.

### Decision
Build deterministic log parsing, validation, and
incident analysis before introducing LLM capabilities.

### Alternatives
- Start with an LLM-powered incident chatbot.
- Build a deterministic analysis foundation first.

### Rationale
A deterministic baseline provides testable behavior
and enables meaningful comparison with later AI systems.

### Trade-offs
Initial capabilities will be limited to structured
analysis rather than natural-language investigation.

---

## ADR-002: Evidence-First Investigation

Status: Accepted

### Context
An AI-generated explanation is not necessarily
a verified root cause.

### Decision
Investigation findings must reference supporting
evidence wherever possible.

The system must distinguish observations, hypotheses,
and confirmed conclusions.

### Rationale
Traceable evidence makes investigations easier
to review, reproduce, and evaluate.

### Trade-offs
Evidence tracking introduces additional data
modelling and validation requirements.

---

## ADR-003: Synthetic Incidents for Initial Development

Status: Accepted

### Context
Real production logs may contain credentials,
personal information, or confidential infrastructure data.

### Decision
Use synthetic application logs and controlled
failure scenarios during initial development.

### Rationale
Synthetic incidents support repeatable testing
without requiring access to production systems.

### Trade-offs
Synthetic scenarios may not capture the full
complexity of real-world incidents.

The evaluation dataset will need increasing
diversity as the project matures.

---

## Future Decisions

The following decisions remain open:

- Database and persistence architecture
- LLM provider and inference strategy
- Retrieval and reranking approach
- Agent orchestration
- Authentication and authorization
- Deployment architecture
- Evaluation methodology

Record these decisions only when their requirements
and alternatives have been investigated.

## ADR Template

### ADR-XXX: Decision Title

Status: Proposed / Accepted / Superseded

Context:

Decision:

Alternatives considered:

Rationale:

Trade-offs:

Review conditions:
