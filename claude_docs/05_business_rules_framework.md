# Business Rules Framework

Business rules define how each tenant interprets TSW data.

## Rule Types
- **Definition**: business meaning or terminology
- **Filter**: automatic WHERE clauses
- **Calculation**: computed or derived values

Rules are:
- Tenant-scoped
- Versioned
- Auditable
- Automatically applied

The same question may produce different SQL for different tenants.
