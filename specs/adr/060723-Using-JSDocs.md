# Using JSDocs To Generate Automated Documentation

## Context and Problem Statement
How do we want to write our documentation for our JS Code? We want our code to be easily maintanable and understood.

<!-- This is an optional element. Feel free to remove. -->
## Decision Drivers

* We need a way to generate automated documentation from the comments in our code
* We need to consistently write comments for our code, and have documentation outside of our files describing what each function does.

## Considered Options

* `JSDoc`
* `Slate`
* `Storybook`

## Decision Outcome

Chosen option: `JSDoc`\
We decided to use `JSDoc` because we believed it best suited our needs for documentation.
It also had support with `ESLint`, as `ESLint` would throw errors if JSDoc comments weren't included.

<!-- This is an optional element. Feel free to remove. -->
## Pros and Cons of the Options
* `JSDoc` generation can easily be handled by GitHub Actions
* Frequent `JSDoc` generation may result in a lot of time spent on fixing merge errors for the automated documentation (if the automated documentation generates a timestamp).

## More Information

[Jest](https://jestjs.io/)
