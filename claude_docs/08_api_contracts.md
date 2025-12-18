# API Contracts

All APIs are tenant-aware via server-side session context.

Key endpoints:
- POST /api/ai-query/start
- POST /api/ai-query/clarify
- POST /api/ai-query/execute
- GET  /api/ai-query/export
- GET  /api/ai-query/history

The frontend never passes tenant identifiers.
