# Frontend Development Process

## Step 0 - Project Setup
- Initialize README
- Initialize Linting
- Initialize Continuous Deployment environments 
  - Develop, Master branches

## Step 1 - Scaffolding

Create basic boilerplate skeletons for the app's major parts & features
- App Controller
- Feature Controllers
- REST Endpoints
- App Module
- Feature Modules
- Routing
- Shared Components
- App State

## Step 2 - Develop Features
Implement the intended functionality in the business logic for each feature according to requirements
- Need: Requirements specific to this feature
- Need: Ensure all dependencies & external integrations are installed & configured properly
- Need: Necessary Configurations to correctly provide resource from API
- Git Branch: feature-branch

### Step 2.1 Services
- Create provider functions for all the resources in current feature
    - Pull in resoureces via API
    - Return correctly modeled data resources
- Console log to ensure correct implementation of provider functions
- Write unit tests for provider functions

### Step 2.2 State Management
Use the new @ngrx/entity methodology for creating actions based on CRUD methods & setting up selectors
- Distribute resources into feature state
    - Actions
    - Reducers
    - Effects
- Write unit tests for all state management files in feature

### Step 2.3 View Template
- Inject feature State into Containers
- Set container properties (resources pulled from feature state via selectors)
- Cut out template HTML & create components
- Input properties to compnents & emit UI events where needed

### Step 2.4  Pull Request
- Does feature work according to requirements?
    - If yes: Write unit tests for view components
    - If no: Make necessary refactoring to meet requirements
- Create PR & invoke the correct reviewer(s)

### Outline
- Process
    - Scaffolding Angular Projects
        - App
        - Services
        - NGRX
        - Modules
        - Components
        - Other

### Architecture Level
- Gathering requirements
- Backend dependency list
    - External API
    - Backend Platforms
    - Custom Backend
- Frontend dependency list

####################################################################################

# Process

## Scaffolding Angular Projects
Angular Version 6

### App
Creating a basic Angular Project via CLI

### Services
Adding services to existing Angular project via CLI

### NGRX
Installing NGRX to a project should be done prior to creating feature modules

### Modules
Adding shared & feature modules to existing Angular project via CLI

### Components
Adding components to existing Angular project via CLI

### Other
Other app scaffolds to add via CLI (if needed)
- Pipes
- Interceptors

####################################################################################
