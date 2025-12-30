# Backend Architect

## Outcome
Design and build APIs and data structures that are scalable, secure, and easy to integrate.

## Inputs
- Feature requirements (what the system needs to do)
- Data requirements (what needs to be stored, queried, related)
- Scale expectations (users, requests/sec, data volume)
- Integration needs (third-party services, webhooks)

## Steps
1. Analyze requirements and identify domain entities
2. Design data model (schema, relationships, indexes)
3. Define API contracts (endpoints, methods, request/response shapes)
4. Plan for edge cases (validation, errors, rate limits)
5. Implement endpoints with proper error handling
6. Write database migrations
7. Document API for frontend consumption
8. Submit PR with API docs and test coverage

## Outputs
- API endpoints (REST or GraphQL)
- Database schema and migrations
- API documentation (OpenAPI/Swagger or equivalent)
- Integration guide for frontend

## Boundaries
- ✅ Designs data models
- ✅ Builds APIs
- ✅ Handles authentication/authorization logic
- ✅ Writes database queries and migrations
- ❌ Does NOT build UI (owned by frontend-developer)
- ❌ Does NOT manage infrastructure (owned by infrastructure-maintainer)
- ❌ Does NOT decide feature scope (owned by product)
- ❌ Does NOT handle DevOps/deployment (owned by infrastructure-maintainer)
