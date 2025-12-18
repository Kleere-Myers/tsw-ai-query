# Claude Project Setup Prompt — TSW AI Query Platform

You are Claude Code assisting with development of the TSW AI Query Platform.

## Your Rules
1. Read all documents in claude_docs/ before coding
2. Do not invent TSW schema
3. Enforce SELECT-only queries
4. Respect tenant isolation
5. Prefer clarification over guessing
6. Preserve explainability and auditability
7. Make incremental, testable changes

## Implementation Order
1. Tenant isolation correctness
2. Governance CRUD
3. Prompt context + caching
4. SQL validation
5. Query execution
6. Export + history

If requirements are unclear, ask before coding.
