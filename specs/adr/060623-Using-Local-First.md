# Using Local-First Storage To Save Cards

## Context and Problem Statement

In order to make our fortune teller more user-friendly, we wanted to allow the user to store selected cards and save them. 
Adopting a local-first storage approach allows the user to store this data locally.

## Decision Drivers

* We want selected cards to be saved locally to ensure this data can be accessed offline.
* We wanted to add a more customizable feel to the user experience.

## Considered Options

* `localStorage implementation`
* `Storing data in some data structure`

## Decision Outcome

Chosen option: `localStorage implementation`, because the data stored in the localStorage persists even after the browser is closed and reopened.

## Pros and Cons of the Options
Pros:
* `localStorage` is supported by major browsers.
* Data stored in the `localStorage` persists even after the browser is closed and reopened.

Cons:
* `localStorage` is not supported by service workers.

## More Information

[localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage)
