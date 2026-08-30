# Repository Instructions

## Documentation

The `docs/` directory is the project documentation wiki and source of truth for product requirements, technical designs, and engineering decisions.

Use the existing documentation before making decisions. Link related documents instead of duplicating content.

## Document Types

- **PRD:** Defines what to build, for whom, why, scope, requirements, and acceptance criteria.
- **Technical Design:** Defines how an approved scope will be built.
- **RFC:** Explores one important technical question with meaningful alternatives.
- **ADR:** Records an accepted technical decision and its consequences.

## Workflow

```text
Business requirement → PRD → Technical Design
                                      ↓
                         RFC, if a major decision is unresolved
                                      ↓
                         ADR, once the decision is made
```

A Technical Design may begin as an exploration. Create an RFC only when a decision is consequential, difficult to reverse, or has meaningful alternatives.

## Documentation Structure

Organize documentation by product:

```text
docs/
├── README.md
├── templates/
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

Product-specific documents belong under `docs/products/<product-name>/`.

Keep documents concise, current, linked, and proportional to the change.
