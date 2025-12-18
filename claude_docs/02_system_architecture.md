# System Architecture

## High-Level Components

### Frontend
- Angular application
- Session-based authentication
- Business-friendly UX
- No direct database access

### Backend
- Django + Django REST Framework
- Tenant-aware services
- Query lifecycle management
- Governance enforcement

### AI Layer
- Prompt-driven SQL generation
- Clarification-first behavior
- Deterministic fallbacks for testing

### Databases
- **Platform DB**: users, tenants, rules, audit, query history
- **TSW DB**: read-only TimeShareWare database

All access to TSW is mediated by backend services.
