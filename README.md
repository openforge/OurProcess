# dev-standards-template
Development standards for frontend web applications at Openforge

## General Project Reference Template

### Outline
- Process
    - Scaffolding Angular Projects
        - App
        - Services
        - NGRX
        - Modules
        - Components
        - Other
- Standards
    - Architecture Level
    - Project Level
    - Library Level
    - Code Authoring Level
    - Generalized Code Standards & Best Practices
    - PR Reviews
    - Bug/Issue Tracking
    - Other Standards

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

# Project Level
- Dependencies
- File structure
- Module naming rules
- Service file structure
- Interface/data models file structure
- Shared Component file structure
- General Unit Testing
- Integration Testing & Pipelines
- E2E Testing
- Package JSON specifics
    - What dependencies are dev dependencies?

# Dependencies
## General Dependencies
### Code & Compiling
- Node
- Typescript
### Formatting
- linting
- husky
### Styling
- scss
### Testing & Continuous Integration
#### Testing
- Jasmine/Karma configured by default in Angular Projects
- Protractor e2e testing configured by default in Angular Projects
#### Continuous Integration
- Install TravisCI
    - Add app via TravisCI admin dashboard
    - Add .yml file to project
    - Ensure that it is working as expected
## Dev Dependencies
## Project Specific Dependencies
- Based on requirements document



# File Structure
## App Structure
```
my-app/
  README.md
  package.json
  e2e/
  public/
    index.html
    favicon.ico
  src/
    assets/
        logo.svg
    environments/
        environment.ts
        environment.prod.ts
    models/
    app/
        app.module.ts
        app-routing.module.ts
        app.constants.ts *
        auth.guard.ts
        app.component.ts
        app.component.html
        app.component.scss
        app.component.spec.ts
        mocks/
        state/
        shared/
        feature-1/
        feature-2/
        feature-3/
```

## App State
```
state/
    app.actions.ts
    app.actions.spec.ts
    app.facade.ts
    app.facade.spec.ts
    app.reducer.ts
    app.reducer.spec.ts
```

## Shared Module
```
shared/
    shared.module.ts
    api.interceptor.ts
    components/
        shared-modal/
            shared-modal.component.ts
            shared-modal.component.html
            shared-modal.component.scss
            shared-modal.component.spec.ts
    pipes/
        app-pipe.pipe.ts
        app-pipe.pipe.spec.ts
```

## Feature Modules
```
feature-1/
    feature.module.ts
    feature-routing.module.ts
    containers/
        container-1/
            container-1.component.ts
            container-1.component.html
            container-1.component.scss
            container-1.component.spec.ts
        container-2/
    components/
        component-1/
            component-1.component.ts
            component-1.component.html
            component-1.component.scss
            component-1.component.spec.ts
        component-2/
        component-3/
        component-4/
        component-5/
    services/
        feature.service.ts
        feature.service.spec.ts
    state/
        feature.actions.ts
        feature.actions.spec.ts
        feature.reducer.ts
        feature.reducer.spec.ts
        feature.facade.ts
        feature.facade.spec.ts
feature-2/
feature-3/
```

