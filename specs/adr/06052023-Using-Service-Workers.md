# Using Service Workers to provide the user with reliable offline access

## Context and Problem Statement

How can we ensure that users are able to access and use our web application even without reliable internet connection? How can we develop a local first application?

<!-- This is an optional element. Feel free to remove. -->
## Decision Drivers

* We want the user to be able to use our web application without internet connection.
* After the first time loading the page, the necessary elements and resources will be loaded and saved for future use

## Considered Options

* `Downloading every image and resource into the repository`
* `Service workers`

## Decision Outcome

Chosen option: `Service Workers` We decided on using service workers since they would be easier to maintain if we ever had to update any images or elements obtained from the web. Rather than having to clear the repository of unused images, we can simply change the links within the service worker files.

## Pros and Cons of the Options
Pros:
- `Service Workers` offer a reliable access to necessary elements that have to fetch from outside sources.
- `Service Workers` offer an easier access within the code and can be maintained with less effort than other options.

Cons:
- `Service Workers` it is a bit tricky to deal with at the start as we ran into the problem of the files not updating when needed.

## More Information
* [Service Workers](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API/Using_Service_Workers)
* [Caching](https://developer.chrome.com/docs/workbox/caching-strategies-overview/)

Updated decision: https://github.com/cse110-sp23-group27/cse110-sp23-group27/blob/main/specs/adr/061123-Not-Using-Service-Workers.md
