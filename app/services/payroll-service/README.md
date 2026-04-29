# Payroll Service

This microservice handles payroll calculations, pay periods, overtime rules, and compensation processing.

## Responsibilities
- Pay period management and scheduling.
- Payroll calculation for employees and multi-client batches.
- Overtime, double time, holiday pay, and premium calculations.
- Pay rate history and retroactive adjustments.
- Export to payroll processors like QuickBooks.

## Suggested Architecture
- Language: TypeScript
- Runtime: Node.js
- Framework: Express or NestJS
- Database: PostgreSQL for payroll data
- Libraries: Date manipulation, financial calculations

## Directory Layout
- `src/` - Service source code.
  - `controllers/` - API endpoints for payroll operations.
  - `services/` - Calculation engines for pay rules.
  - `models/` - Pay period, rate, and payroll data models.
  - `rules/` - Configurable pay rules and compliance logic.
- `tests/` - Unit and integration tests.

## API Endpoints
- POST /payrolls/calculate - Run payroll calculation
- GET /pay-periods - List pay periods
- PUT /pay-rates/{id} - Update pay rates
- POST /exports - Export payroll data

## Next Steps
- Initialize with Node.js and calculation libraries.
- Implement pay rule engines for overtime and holidays.
- Add audit logging for all calculations.
- Integrate with timecard-service for hours data.