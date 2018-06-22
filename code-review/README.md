<p align="center">
  <img src="https://github.com/openforge/main-website/blob/master/src/assets/logo-openforge.png?raw=true"/>
</p>
<p align="center">
  <a href="http://www.openforge.io/">Official Website</a> |
  <a href="http://www.openforge.io/opportunities">Opportunities</a> |
  <a href="https://www.facebook.com/OpenForgeUS/">Facebook</a>
</p>

<h3 align="center">
  Leading By Example.
</h3>

<p align="center">
  Working with the latest technologies, designing the best products, and sharing our knowledge with the world wide community.
</p>

# Code Review

1. Does the code meet X standards?
2. Is there a simpler/easier way to accomplish this?
    -  Is it worth the time to refactor?
4. What to do if the code passes/fails review?


## Standards
Make sure the code being reviewed adheres to the relevant coding standards for the project. For example, if the code leverages a package or library, be sure to follow their standards when implementing.

## Refactor
Ensure that the code is not does not contain extraneous logic/changes. If importing a library/package, attempt to only import what's being used.

#### Technical Debt
Some refactors will not be time/cost efficient while the code is in review. If you believe the refactoring effort should be re-approved first, please refer to the *Dev Process Guide -- Scoping Work for Approval*. Either way, be sure to leave comments in the Pull Request about any enhancements that should be made.

## Definition of Done

Code reviewers should leave clear comments and descriptions of any issues found during review process.

#### Failed Review
If the reviewer believes the code needs changes, make a comment on the Pull Request. If applicable, leave comments on the relevant lines of code. Otherwise, create a checkbox list in the comments detailing the requested changes.
e.g.
```
- [ ] Fix bug
- [ ] Improve Code
```

#### Passed Review
- Re-assign the original developer to the Github issue
- Leave a general update stating any questions, concerns, technical debt, etc.
  - If code author does not have privileges, merge the Pull Request.