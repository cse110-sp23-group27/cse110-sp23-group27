# Not Using Service Workers
parent: Decisions
nav_order: 100
title: ADR Template

## Context and Problem Statement
Originally, we were going to use service workers, but it yielded inconsistent results and believed it would better to not use service workers.

## Decision Drivers

* Service workers would work when run on some local machines, but not in others.
* Some of the images would load, but others would not when testing service workers.

## Considered Options

* `Downloading every image and resource into the repository`

## Decision Outcome
Chosen option: `Service Workers` We decided on just downloading the images and resources needed to the repository and access them from there.

## Pros and Cons of the Options
Pros
* Images and audio will still be loaded.

Cons:
* It risks not being usable without relying on internet connection.
### {title of other option}

Original decision: https://github.com/cse110-sp23-group27/cse110-sp23-group27/blob/main/specs/adr/06052023-Using-Service-Workers.md?plain=1
