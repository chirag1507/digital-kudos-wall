# Digital Kudos Wall Implementation Plan

This document outlines the non-negotiable implementation plan for all new features in the Digital Kudos Wall project. This plan must be strictly followed for every new story implementation.

## Project Structure

```
digital-kudos-wall/              # Main repository
├── docs/                        # Documentation
│   └── user-story-map.md       # Source of story details
digital-kudos-wall-backend/      # Backend repository
digital-kudos-wall-frontend/     # Frontend repository
digital-kudos-wall-system-tests/ # System tests repository
```

## Implementation Steps

### 1. System Test Definition

- **Location**: `digital-kudos-wall-system-tests/src/acceptance/features/<story-name>.feature`
- **Tasks**:
  - Create feature file with Gherkin scenarios
  - Implement DSL layer (`src/acceptance/dsl/<story-name>.dsl.ts`)
  - Create required models (`src/acceptance/dsl/models/<model-name>.ts`)
- **Reference**: See `account_registration.feature` for example implementation
- **Approval Gate**: Feature file and DSL review

### 2. Backend Implementation

- **Location**: `digital-kudos-wall-backend/src/modules/<module-name>/`
- **Tasks**:
  1. Implement use case following Clean Architecture principles
  2. Implement sociable unit tests (Follow `SOP-SociableUnitTests.md`)
  3. Implement layers following Clean Architecture:
     - Domain layer
     - Application layer
     - Infrastructure layer
     - Interface layer
  4. Implement component tests (Follow `SOP-ComponentTests.md`)
  5. Implement narrow integration tests (Follow `SOP-NarrowIntegrationTests.md`)
- **Guidelines**:
  - Follow `SOP-TestDataManagement.md` for test data
  - Follow `SOP-TestDoubles.md` for test doubles
  - Reference implementation: `src/modules/user/`
- **Approval Gate**: Backend implementation review

### 3. Frontend Implementation

- **Location**: `digital-kudos-wall-frontend/src/features/<feature-name>/`
- **Tasks**:
  1. Implement frontend following Clean Architecture (Follow `SOP-Frontend-Clean-Architecture.md`)
  2. Add data test IDs to all components
  3. Implement component tests (Follow `SOP-ComponentTests.md`)
  4. Implement sociable unit tests (Follow `SOP-SociableUnitTests-FE.md`)
  5. Implement consumer-driven contract tests (Follow `SOP-ContractTests.md`)
- **Guidelines**:
  - Follow `SOP-TestDataManagement-FE.md` for test data
  - Reference implementation: `src/features/auth/`
- **Approval Gate**: Frontend implementation review

### 4. Contract Testing

- **Location**: Backend and Frontend repositories
- **Tasks**:
  1. Implement provider contract verifier tests in backend (Follow `SOP-ContractTests.md`)
- **Approval Gate**: Contract tests review

### 5. System Test Implementation

- **Location**: `digital-kudos-wall-system-tests/`
- **Tasks**:
  1. Implement step definition files
  2. Implement web driver layer with page objects
  3. Use test IDs in page objects for system interaction
- **Approval Gate**: System test implementation review

## Important Guidelines

1. Each step must be completed and approved before moving to the next step
2. Take small, incremental steps
3. Each step should be reviewed and committed separately
4. Follow all referenced SOPs strictly
5. Use existing implementations as reference (e.g., registration module)
6. All test data management must follow respective SOPs
7. Maintain consistent test IDs across frontend and system tests

## Reference Implementations

- Backend Module: `digital-kudos-wall-backend/src/modules/user/`
- Frontend Feature: `digital-kudos-wall-frontend/src/features/auth/`
- System Tests: Registration module acceptance tests and smoke tests

## Standard Operating Procedures (SOPs)

The following SOPs must be referenced and followed:

- `SOP-SociableUnitTests.md`
- `SOP-ComponentTests.md`
- `SOP-NarrowIntegrationTests.md`
- `SOP-TestDataManagement.md`
- `SOP-TestDoubles.md`
- `SOP-Frontend-Clean-Architecture.md`
- `SOP-SociableUnitTests-FE.md`
- `SOP-ContractTests.md`
- `SOP-TestDataManagement-FE.md`
- `SOP-ContractTests-FE.md`
- `SOP-ComponentTests-FE.md`
- `SOP-AcceptanceTests.md`
- `SOP-SmokeTests.md`
