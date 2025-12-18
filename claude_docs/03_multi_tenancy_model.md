# Multi-Tenancy Model

Each Time Share company is an isolated tenant.

## Rules
- Users belong to exactly one tenant
- Subject areas are tenant-scoped
- Business rules are tenant-scoped
- Cached data is tenant-scoped

## Guarantees
- No cross-tenant reads
- No cross-tenant writes
- No shared cache keys across tenants

Tenant resolution occurs server-side using authenticated user context.
