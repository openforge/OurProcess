<p align="center">
  <img src="https://github.com/openforge/main-website/blob/master/src/assets/logo-openforge.png?raw=true"/>
</p>
<p align="center">
  <a href="http://www.openforge.io/">Official Website</a> |
  <a href="http://www.openforge.io/opportunities">Opportunities</a> |
  <a href="https://www.facebook.com/OpenForgeUS/">Facebook</a>
</p>

<h3 align="center">
  Leading By Example
</h3>

<p align="center">
  Working with the latest technologies, designing the best products, and sharing our knowledge with the world wide community
</p>

# What to do

If you're reading this, it means you're part of our team or simply curious about our process.  Thank you for that :)  Let's dive into the dev process!

** Insert Infographic **

## Discovery Phase (Business Requirements)

The first step in scoping a project is understanding the requirements.   At OpenForge, we involve both design and developers equally in our process.  In a typical project, a dev is responsible for:

- Send client **The Dev Questionaire**
- Reviewing App requirements & Questionare w/ Design Team


## Design Phase

- Iterate over design & functional requirements w/ designers 
- Send client questions / receive clarifications on functionality
- Annotated the designs from developer standpoint

## Development Phase

- Send **Request for Accounts / Instruction Templates**
- Initialize Repository w/ Appropriate Template Apps
- Copy README from README.md
- Setup OF Standards (Commitizen, Gitflow, etc)
- Setup Github/Heroku/TravisCI Continuous Integration Strategy
- Scaffold App & Setup Routing for Team contributions
- Install Dependencies

# Mobile & Web App

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


# Backend Process

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
