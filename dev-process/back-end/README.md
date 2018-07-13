# Frontend Development Process

## Step 0 - Project Setup
- Initialize README
- Initialize Linting
- Initialize Continuous Deployment environments 
  - Develop, Master branches
- Initialize Admin Dashbboard
  - Strapi.io for MongoDB/ MySql
  - X for Firebase
- Initialize / Document Endpoints
  - Swagger.io
- Initialize 3rd party tools
  - Error/Debug Logging
  - X


## Step 1 - Scaffolding & Features
Implement the intended functionality in the business logic for each feature according to requirements
- Git Branch: feature-branch
- Establish DB Connection & Querying for resource
- Define Data Models
- Controller Logic
- Create REST Resource Endpoint
- Use Postman to ensure correct functionality
- Write unit tests for features
- If any configuration should be done by the owner, inform the owner to complete this setup

### Step 2  Pull Request
- Does feature work according to requirements?
    - If yes: Write unit tests for view components
    - If no: Make necessary refactoring to meet requirements
- Create PR & invoke the correct reviewer(s)




## Backend Requirements

### Do the requirements specify any special backend platforms, such as Firebase, Strapi, or Sashido?
**Yes**; use [this guide](./dev-process/backend/platforms/README.md) for setting up your backend.

### Does this app require a custom backend?
**Yes**; use [this guide](./dev-process/backend/node-backend/README.md) for kicking off Node backend development.

## Frontend Requirements

### Does this project require a frontend user interface?
**Yes**; use [this guide](./dev-process/frontend/README.md) to get started with our frontend development guide.

## Do you need to review a Pull Request
**Yes**; use [this guide](./code-review/README.md) for our code review process.
