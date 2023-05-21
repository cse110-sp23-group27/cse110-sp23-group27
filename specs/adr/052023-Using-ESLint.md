# Using ESLint to Enforce Coding Style Guidelines

## Context and Problem Statement
With a development team that is able to push commits to branches or open pull requests to merge code into the main (production) branch, how will we as a team enforce our coding style standards consistently for the entire repository.

Correcting and ensuring proper coding formatting can be a time-consuming and tedious task for developers. How can we automate many aspects of this task to also improve developer productivity?


## Decision Drivers

We wanted to ensure common coding style and formatting across the repository.

We wanted to increase developer productivity by providing developers with an automatic formatting tool.

## Considered Options

* `ESLint`
* `JSLint`

## Decision Outcome
**Chosen option: `ESLint`**
We decided on `ESLint` because it can be integrated into `GitHub Actions` and locally in an editor to check code formatting/style and fix it.
`ESLint` is also a very well documented tool and offers format configuration files in multiple languages (`.json`, `.yml`) that are user-friendly to author.


## Pros and Cons of the Options
Pros:
- `ESLint` can be included in GitHub Actions workflow to check for formatting errors when an event occurs, such as a push or pull request.
- `ESLint` can also be used locally to automatically format code, and has extensions for all major editors, including `VS Code`.

Cons:
- Integration of `ESLint` into GitHub Actions was initially difficult.


## More Information
[ESLint](https://eslint.org/)

TBD if decision modified/changed
