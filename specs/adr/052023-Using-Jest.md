--- File name should use MMDDYY-Decision-Name.md format
# Using Jest to test our JavaScript

## Context and Problem Statement
We need a way to test the code we write for our fortune telling project. 
We also need a way to automate our testing, so that when there is a push/pull request to
gitHub, a workflow will trigger the tests and make sure nothing broke.

What framework do we want to use to help test our JavaScript and help automate our testing?

<!-- This is an optional element. Feel free to remove. -->
## Decision Drivers

* We wanted to use a framework that everyone could easily use/learn
* We wanted a framework that covers all our needs to create unit tests

## Considered Options

* `Jest`
* `Mocha`
* `Cypress`

## Decision Outcome

Chosen option: `Jest`\
We decided to use `Jest` because it was the framework that most people were familiar with.
For lab 8, we will be using `Jest` as a testing framework, so it makes most sense to use it since we will all have
to learn it anyways. `Jest` is also a widly popular testing framework that is known to be good to use while also 
being easy to use.

<!-- This is an optional element. Feel free to remove. -->
## Pros and Cons of the Options
* `Jest` is easy to use and some group members already know how to use it
* `Jest` will cover all the needs of the testing we will do

## More Information

[Jest](https://jestjs.io/)
