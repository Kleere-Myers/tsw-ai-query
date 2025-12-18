# Backend Skeleton Guide (Django + DRF)

This document defines how the backend must be implemented.

## Core Principles
- Tenant isolation is mandatory
- TSW access is read-only
- Governance is enforced before execution
- Every query is auditable

## Required Apps
- core: tenant resolution, permissions
- accounts: users and roles
- governance: subject areas, columns, business rules
- ai_query: query lifecycle, validation, execution
- monitoring: health and metrics

## Database Strategy
- default DB: platform data
- tsw DB: read-only reporting

## Service Boundaries
Views must be thin. Business logic lives in services:
- prompt_service
- policy_service
- sql_service
- validators
- execution_service
- audit_service

## Caching
- Cache prompt context per tenant
- Invalidate on governance changes
- Never share cache keys across tenants

## Required Tests
- Cross-tenant access prevention
- SELECT-only enforcement
- Allowlist enforcement
