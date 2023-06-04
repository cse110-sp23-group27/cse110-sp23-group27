# Using Stylelint to Enforce Coding Style Guidelines for HTML and CSS

## Context and Problem Statement
With a development team that is able to push commits to branches or open pull requests to merge code into the main (production) branch, how will we as a team enforce our coding style standards consistently for the entire repository,
regarding html and css?

Correcting and ensuring proper coding formatting can be a time-consuming and tedious task for developers. How can we automate many aspects of this task to also improve developer productivity?


## Decision Drivers

We wanted to ensure common coding style and formatting across the repository for HTML and CSS.

We wanted to increase developer productivity by providing developers with an automatic formatting tool.

## Considered Options

* `HTML Lint`
* `CSS Lint`
* `Style Lint`

## Decision Outcome
**Chosen option: `Style Lint`**
We decided on `Style Lint` because it can be integrated into `GitHub Actions` and locally in an editor to check code formatting/style and fix it.
`Style Lint` is also a very well documented tool and can integrate both css and html checkers in GitHub Actions


## Pros and Cons of the Options
Pros:
- `Style Lint` can be included in GitHub Actions workflow to check for formatting errors when an event occurs, such as a push or pull request.
- `Style Lint` can also be used locally to automatically format code
- `Style Lint` is trusted by companies worldwide like Google and GitHub

Cons:
- Configuring `Style Lint` initially was difficult

## More Information
[StyleLint](https://stylelint.io/)

TBD if decision modified/changed
