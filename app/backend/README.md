# Backend Services - Microservice Architecture

This folder was originally intended for a monolithic backend, but has been restructured into microservices under `services/`.

## Updated Structure
The backend logic is now distributed across independent microservices:
- `auth-service/` - Handles authentication, authorization, MFA, and user management.
- `hr-service/` - Manages onboarding/offboarding and employee lifecycle.
- `payroll-service/` - Processes payroll calculations, pay periods, and compensation rules.
- `timecard-service/` - Manages time entry, editing, and attendance tracking.
- `client-service/` - Handles multi-tenant client management and subscriptions.
- `reporting-service/` - Provides reporting, analytics, and data exports.

## Migration Notes
- Move any existing code from `backend/src/` to the appropriate service under `services/`.
- Use the `api-gateway/` for inter-service communication.
- Shared utilities should go into `shared/`.

## Next Steps
- Initialize each service with its own package.json and dependencies.
- Implement service-specific APIs and database schemas.
- Set up inter-service communication via REST, gRPC, or message queues.
- Add service-specific unit and integration tests.
