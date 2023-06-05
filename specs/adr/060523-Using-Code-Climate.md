# Using Code Climate for Code Quality Checking and Reporting

## Context and Problem Statement
As a development team, we currently operate in our repository using branches and pull requests for development, with our team leaders manually reviewing pull requests for correctness before merging code into the production branch (`main`).  We have several formatting and code correctness tools already built into our CI/CD pipeline, but we don't have an automated way to access the *quality* of the code in our repository, both at the time of submitting a pull request and post-hoc. As a development team that is constantly under time pressure to complete the next requirement for our application, how will we determine in a systematic way, where the *quality* in our codebase is lacking and thus needs refactoring?


## Decision Drivers

We wanted to have an automated tool to help us assess the quality of the code in our repository, and help us identify potential quality issues, such as code duplication, poor maintainability practices, lack of test coverage, and other code quality issues/objectives.

We hope that introducing a code quality tool to report on quality issues at the time of a pull request submission (through inline comments) and through the reporting dashboard will help encourage our development team to refactor low quality sections of the codebase.

## Considered Options

* `Code Climate`
* `Codacy`

## Decision Outcome
**Chosen option: `Code Climate`**
We decided on `Code Climate` because it offered the in-depth analysis of our repository we were looking for, including highlighting areas in the codebase with code duplication, too many lines, or low test coverage.  Another key feature that influenced our decision was that `Code Climate` provides detailed inline GitHub comments reguarding code quality after performing static analysis on any pull request that is submitted. We hope this will be a helpful feature for our development team and manual PR reviewers.


## Pros and Cons of the Options
Pros:
- `Code Climate` analysis is detailed and can be integrated into inline comments for a submitted pull request.
- `Code Climate` additionally offers a test coverage feature to assess the testing coverage across the repository.
- `Code Climate` provides a `Code Maintainability` grade and has a reporting dashboard for the code quality of the repository that is easily accessible by a badge button in our repository `README.md`.

Cons:
- Configuring `Code Climate` testing coverage feature into our GitHub Action workflow has been slightly challenging.

## More Information
[Code Climate Quality](https://codeclimate.com/quality)

TBD if decision modified/changed