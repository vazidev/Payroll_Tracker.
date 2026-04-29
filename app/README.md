# App Monorepo

This directory contains the enterprise timecard and payroll application codebase.

## Structure
- `backend/` - Server-side services, API logic, authentication, payroll rules, HR workflows, and database migrations.
- `frontend/` - Web application UI for admins, HR, employees, and client managers.
- `mobile/` - Mobile app or PWA support for field time entry, clock-in/out, and employee self-service.
- `infra/` - Infrastructure definitions for Docker, Terraform, and deployment automation.
- `docs/` - Architecture, API, security, and design documentation.
- `docs/testing/` - QA strategy, test plans, and quality assurance guidance.
- `config/` - Environment config templates and shared application settings.
- `scripts/` - Utility scripts for project setup, migration, and deployment.
- `tests/` - Shared integration tests, end-to-end test scaffolding, and QA artifacts.
- `design/` - UI/UX wireframes, mockups, and design assets.

## Getting Started
1. Choose a stack for each project: backend, frontend, mobile.
2. Update the corresponding `README.md` in each folder with framework-specific commands.
3. Add package managers and dependency manifests once the technology choices are finalized.
