# dev-standards-template
Development standards for frontend web applications at Openforge

## General Project Reference Template

### Outline
- Architecture Level
- Project Level
- Library Level
- Code Authoring Level
- Generalized Code Standards & Best Practices
- PR Reviews
- Bug/Issue Tracking
- Other Standards

### Architecture Level
- File structure
- Module file structure
- Module naming rules
- Service file structure
- Interface/data models file structure
- Shared Component file structure
- General Unit Testing
- Integration Testing & Pipelines
- E2E Testing

### Project Level
- General Dependencies
- Package JSON specifics
    - What dependencies are dev dependencies?

### Library Level
- Routing
- Async Operations with RxJS
- Unit Testing
- State management
    - State

### Code Authoring Level
- Imports
- Constructors
- Comments
- Strings
- Working with Types
    - Declaration
    - Initialization
    - Instantiation
- Type Casting
- Naming Rules (variables)
    - General variables
    - Library based conventions
    - Reserved words: simple, don’t use them
- Lint Rules
- Prettier

### Generalized Code Standards & Best Practices
- Naming conventions
- ??? (Research other topics)

### PR Reviews
- Look into a few recent projects
- Review recently approved PRs
- Review current unapproved PRs
- Define process for PR reviews

### Bug/Issue Tracking
- How to report issues (how to format report)
- Where to report issues
- Creating issue branches
- Creating issue PRs
- Reviewing & closing

### Other standards
- Multilingual support
- Accessibility

### Project Specific README Templates
- Angular
- Ionic
- Stencil
- PWAessibility

### Project Specific README Templates
- Angular
- Ionic
- Stencil
- PWA

####################################################################################

# Project Level
- General Dependencies
- Install Continuous Integration
- General App File structure
- Module file structure
- Module naming rules
- Service file structure
- Interface/data models file structure
- Shared Component file structure
- General Unit Testing
- Integration Testing & Pipelines
- E2E Testing
- Package JSON specifics
    - What dependencies are dev dependencies?

# General Dependencies
## Code & Compiling
- Node
- Typescript
## Formatting
- linting
- husky
## Styling
- scss

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