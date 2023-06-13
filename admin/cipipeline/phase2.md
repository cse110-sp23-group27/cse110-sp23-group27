# Pipeline status

# Pipeline diagram:

![pipelineImage](https://github.com/cse110-sp23-group27/cse110-sp23-group27/blob/main/admin/cipipeline/phase2.png)

# Currently Functional Pipeline Elements

### Local Development and Testing
* Running Basic Unit Tests (`Jest`) Locally (w/ Test Coverage information generation `--coverage`)
* Running End-to-End (E2E) Tests Locally with `Puppeteer`
* Running autoformatter (`ESLint`) locally before committing
* Git Commit
* Git Push

### GitHub Action Workflow on Push to Feature Branch
* JS/CSS/HTML Style Enforcement using `ESLint`, `StyleLint` and `HTMLHint` with `Super-Linter` running in Github Actions
* Basic Unit Testing (`Jest`) through GitHub Actions
* Pull Request from Branch

### Pull Request to Main Branch Workflow
* Open pull request
* Assign reviewer/s to PR
* Link PR to an active GitHub Issue
* On pull request to main branch, a GH Action will run to automatically generate codebase documentation using `JSDocs` and the updated documentation will be automatically deployed to a live GitHub Pages documentation site, which is linked in our application.
* Automatic Static Analysis with inline Pull request comments using `Code Climate` is run through GH Action on initiation of pull request to main branch
* Assigned PR reviewer will go through a formal process for PR review, including checking out feature branch locally, viewing new changes in the application through live server,running tests locally, making sure all GH Actions checks pass, and also reviewing code quality comments automatically added to the PR. Reviewer will add review comments and decision for PR.
* If manual reviewer requests changes, or the automated checks don't pass, developer can add commits directly to the open PR to fix the issue/s.

### Deployment (After successful merge to main branch)
* If changes are approved by manual reviewer, PR can be merged into main production branch.
* Linked GitHub Issue will be automatically closed on PR merge, and feature branch should be closed by developer
* On successful merge to main branch, `Code Climate` is setup to check latest changes from pull request and update the `Code Maintainability` badge and score to report on code quality and code that should be refactored. 
* On successful merge to main branch, a GitHub Action will automatically run `Istanbul` and `Code Climate` test coverage reporter tools to gather test coverage information from `Jest` unit tests and update the `Test Coverage` badge and score, which informs our team on which areas in our codebase are missing unit test coverage.
* Automatic deployment of website with new changes to GitHub Pages

## Still in progress 

* Adding more `Jest` unit tests to improve `Code Climate` test coverage score

## Planned
* Minification of the code