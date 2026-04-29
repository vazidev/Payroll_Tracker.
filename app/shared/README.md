# Shared Libraries

This directory contains shared utilities, models, and code used across microservices.

## Contents
- Common data models and types.
- Utility functions for logging, validation, etc.
- Shared middleware and helpers.
- Reusable components for services.

## Structure
- `src/` - Shared source code.
  - `models/` - Common data models.
  - `utils/` - Utility functions.
  - `types/` - TypeScript type definitions.
- `tests/` - Tests for shared code.

## Next Steps
- Add shared dependencies and build scripts.
- Publish as a private package if needed.
- Ensure all services import from here for consistency.