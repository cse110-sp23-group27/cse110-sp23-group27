# Using End-to-end testing to test our project's functionalities

## Context and Problem Statement
As a development team, we need a way to ensure that our code does not break the build without manually testing our code using liveshare every time we make a change to our code. We needed to determine a systematic way to test our code automatically, that would run consistently every time, either on GitHub actions or through using an npm command locally.

## Decision Drivers

We wanted an automatic code testing tool that would run on our newly updated code, and would test if the basic functionalities of our code worked.

We hope that if the tests throw an error we can understand what part of our code went wrong.

## Considered Options

* `Jest Puppeteer`
* `Cypress`
* `Playwright`

## Decision Outcome
**Chosen option: `Jest Puppeteer`**
We decided on `Jest Puppeteer` because it offered the functionality of end-to-end javascript testing, and integrated well with our existing use of `Jest` for unit tests.

## Pros and Cons of the Options
Pros:
- `Jest Puppeteer` can be run with `Jest` unit tests simultaneously with one command.
- There is support for `Jest` in `ESLint`, allowing us to use a linter to format our code in our puppeteer tests

Cons:
- Configuring `Jest Puppeteer` for end to end testing took a lot of research and trial and error. 

## More Information
[Puppeteer](https://jestjs.io/docs/puppeteer)

TBD if decision modified/changed
