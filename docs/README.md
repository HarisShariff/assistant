# Documentation

The `docs/` directory is the project documentation wiki and source of truth for product intent, technical design, and important engineering decisions.

## Document Types

### PRD

A Product Requirements Document defines what we are building and why.

It should cover:

- Problem and target user
- Desired outcome
- Scope and non-goals
- User flow
- Product requirements
- Acceptance criteria
- Constraints and open questions

The PM owns the PRD. It should not prescribe implementation details.

### Technical Design

A Technical Design explains how the approved product scope will be built.

It covers the system flow, components, interfaces, data, security, reliability, testing, rollout, risks, and relevant alternatives.

The EM or engineer owns the Technical Design. It may begin as a draft during architecture exploration.

### RFC

A Request for Comments explores one consequential technical question.

Use an RFC when there are meaningful alternatives, trade-offs, or risks. Keep it focused on the decision rather than the entire product.

An RFC should cover the problem, context, options, evaluation criteria, recommendation, and decision.

### ADR

An Architecture Decision Record permanently records an accepted technical decision.

It should cover the context, decision, alternatives considered, and consequences.

An RFC may produce an ADR, but an important decision can also receive an ADR directly.

## Workflow

```text
Business requirement
    ↓
PRD
    ↓
Technical Design draft
    ↓
RFC, if a major decision is unresolved
    ↓
ADR, once the decision is made
    ↓
Final Technical Design
```

This workflow is iterative. A Technical Design may reveal the need for an RFC. Do not create RFCs for routine implementation choices.

## Structure

Organize documentation by product:

```text
docs/
├── README.md
├── templates/
│   ├── prd.md
│   ├── technical-design.md
│   ├── rfc.md
│   └── adr.md
├── products/
│   └── <product-name>/
│       ├── README.md
│       ├── prds/
│       ├── technical-design.md
│       ├── rfcs/
│       ├── adrs/
└── architecture/
    ├── rfcs/
    └── adrs/
```

Create a product folder at:

```text
docs/products/<product-name>/
```

Keep product-specific documents there. Put cross-product decisions in `docs/architecture/`.

## Conventions

- Use lowercase kebab-case filenames.
- Number RFCs and ADRs within their scope.
- Link related documents.
- Keep one authoritative version of each document.
- Update documents when scope or decisions change.
- Mark status clearly: `Draft`, `In Review`, `Approved`, `Superseded`, or `Rejected`.
- Prefer small, focused documents over large universal documents.
