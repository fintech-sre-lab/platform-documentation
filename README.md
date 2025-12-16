# platform-documentation

The central knowledge base for the Fintech Sre Lab fraud detection platform. Contains Architecture Decision Records (ADRs), Runbooks, and SLAs.

# documentation-structure

Project structured to be rendered with MkDocs (Material Theme), a widely used standard that transforms Markdown files into a navigable website.

```
platform-documentation/
├── docs/
│   ├── index.md                     # Home page with the "Big Picture" (the diagram we created)
│   │
│   ├── architecture/                # SYSTEM DESIGN
│   │   ├── high-level-design.md     # C4 or architectural diagrams
│   │   ├── data-flow.md             # Detailed flows: ISO 8583 vs 3DS
│   │   └── network-topology.md      # Map of TCP/gRPC connections
│   │
│   ├── adr/                         # ARCHITECTURE DECISION RECORDS (Essential!)
│   │   ├── 001-adopt-polyrepo.md
│   │   ├── 002-use-circuit-breaker-fail-open.md
│   │   ├── 003-sync-vs-async-paths.md
│   │   └── 004-redis-for-velocity-checks.md
│   │
│   ├── runbooks/                    # OPERATIONS RUNBOOKS (SRE Focus)
│   │   ├── alert-high-latency-prm.md
│   │   ├── disaster-recovery-geo-service.md
│   │   └── database-restore-procedures.md
│   │
│   ├── specs/                       # TECHNICAL SPECIFICATIONS
│   │   ├── iso8583-field-mapping.md # Table of fields used (PAN, Amount, etc.)
│   │   └── api-contracts.md         # Protobuf/gRPC definitions
│   │
│   └── post-mortems/                # INCIDENT REPORTS (Simulated)
│       └── 2024-12-20-latency-spike.md
│
├── mkdocs.yml                       # Documentation site configuration
└── README.md                        # Instructions on how to contribute to the docs
```
