<p align="center">
  <img src="https://github.com/openforge/main-website/blob/master/src/assets/logo-openforge.png?raw=true"/>
</p>
<p align="center">
  <a href="http://wwwopenforgeio/">Official Website</a> |
  <a href="http://wwwopenforgeio/opportunities">Opportunities</a> |
  <a href="https://wwwfacebookcom/OpenForgeUS/">Facebook</a>
</p>

<h3 align="center">
  Leading By Example
</h3>

<p align="center">
  Working with the latest technologies, designing the best products, and sharing our knowledge with the world wide community
</p>

# Internal Dev Process
- Backend
- Frontend
- Accounts
- Design

##################################################################

# Backend
- Review Requirements
- Get Access to Repo
- Pull Starter App
- Add README Template
- Install Dependencies
- Scaffolding
- Features
- Making a PR
- Backend Configuration

## Gather Requirements
- Need: Finalized business requirements for the approved version

## Get Access to Repo
- Need: The repository for this app should already be created by the project owner (client) & exist under his/her ownership as a private repo (At what step do we do this?)
- Does the client account exist?
- If no, guide the project owner to create an account and a private repo for the backend code, and make sure that the project's dev point person has admin rights

##Pull Starter App
Pull in the the starter application, and push code into the project's repo
- Need: Backend Starter app
- Git Branch: master

### Edit README Template
- Need: Framework specific README requirements
- Git Branch: master
- Clean up the default README by removing all parts that don't apply to projects built with the required framework

## Install Dependencies
- Need: Requirements (When do we determine the dependency requirements for a project?)
- Need: Default project setup requirements (linting, commitizen, husky, etc)
- Git Branch: master
- Add all required dependencies in project manifest
- Implement Continuous Integration with TravisCI

## Scaffolding
Create basic boilerplate skeletons for the app's major parts & features
- Need: Requirements > App Features
- Git Branch: develop
- App Controller
- Feature Controllers
- REST Endpoints

## Features
Implement the intended functionality in the business logic for each feature according to requirements
- Git Branch: feature-branch
- Establish DB Connection & Querying for resource
- Define Data Models
- Controller Logic
- Create REST Resource Endpoint
- Use Postman to ensure correct functionality
- Write unit tests for features
- If any configuration should be done by the owner, inform the owner to complete this setup

## Pull Request
- Is each feature's business logic implemented?
- Does it work according to requirements?
    - API endpoints & responses?
- Does CI pass all tests?
- If yes to all the above:
    - Create a pull request to develop

## Finalizeing Version
- Are all features complete?
- Do all features function according to requirements?
- Does CI pass all the tests?
- If yes to all the above:
    - Merge develop branch into master

##################################################################

# Frontend

## Gather Requirements
- Need: Finalized business requirements for the approved version

## Get Access to Repo
- Need: The repository for this app should already be created by the project owner (client) & exist under his/her ownership as a private repo (At what step do we do this?)
- Does the client account exist?
- If no, guide the project owner to create an account and a private repo for the frontend code, and make sure that the project's dev point person has admin rights

## Pull Starter App
Pull in the the starter application, and push code into the project's repo
- Need: Backend Starter app
- Git Branch: master

### Edit README Template
- Need: Framework specific README requirements
- Git Branch: master
- Clean up the default README by removing all parts that don't apply to projects built with the required framework

## Install Dependencies
- Need: Requirements (When do we determine the dependency requirements for a project?)
- Need: Default project setup requirements (ngrx?, linting, commitizen, husky, etc)
- Git Branch: master
- Add all required dependencies in project manifest
- Implement Continuous Integration with TravisCI

## Scaffolding (on master branch)
- Need: List of all features
- Git Branch: develop
- App Module
- Feature Modules
- Routing
- Shared Components
- App State

## Develop Features
Implement the intended functionality in the business logic for each feature according to requirements
- Need: Requirements specific to this feature
- Need: Ensure all dependencies & external integrations are installed & configured properly
- Need: Necessary Configurations to correctly provide resource from API
- Git Branch: feature-branch

### Services
- Create provider functions for all the resources in current feature
    - Pull in resoureces via API
    - Return correctly modeled data resources
- Console log to ensure correct implementation of provider functions
- Write unit tests for provider functions

### State Management
Use the new @ngrx/entity methodology for creating actions based on CRUD methods & setting up selectors
- Distribute resources into feature state
    - Actions
    - Reducers
    - Effects
- Write unit tests for all state management files in feature

### View Template
- Inject feature State into Containers
- Set container properties (resources pulled from feature state via selectors)
- Cut out template HTML & create components
- Input properties to compnents & emit UI events where needed

### Pull Request
- Does feature work according to requirements?
    - If yes: Write unit tests for view components
    - If no: Make necessary refactoring to meet requirements
- Create PR & invoke the correct reviewer(s)
