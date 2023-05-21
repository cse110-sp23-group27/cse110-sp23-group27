# Brainstorming Meeting Notes
Meeting Date: 05-20-23
Kyle Smith is taking notes today.

## Attendance 
- Victor Kim
- Kyle Ng
- Kevin Wong
- Sean Fuhrman
- Daniel Lee
- Elvis Joa
- Kyle Smith

## Agenda
- Setup GitHub Issues and discuss how to structure a GitHub Issue
- Discuss ADR template and work on completing ADR
- Discuss CI/CD pipeline.  What should be included for `phase 1` CI/CD pipeline and create drawio diagram for this.
- Create GitHub Issues for setting up CI/CD pipeline, ADR and initial app tasks


## Topic
GitHub Issue Structure: How to create a GitHub Issue?
We should create a GitHub Issue template with the following structure:
- Description of Task
- Resources
- Possible people to ask:
- Assigning the Issue to someone
- Add a label/s to your Issue

We created a GitHub Issue template so that each issue has a similar structure and all the necessary information.

GitHub Repo settings update
- Changed repo organization access to all members being owners, so that everyone can change GitHub repo settings. 

ADR
- CI/CD pipeline

CI/CD Pipeline
- What should we include in our initial version (`phase1`) of this pipeline.
    - Basic GitHub Action workflow that is triggered upon pushing to team branches. This workflow should initially include the following:
        - Linter (`ESLint`)
        - automated unit testing 
    - Autoformatter for devs to use locally (possibly `ESLint` can also be used here)
    - Unit test suite to that devs can run locally before committing
    - Pull requests should be linked to a corresponding GitHub Issue, which will automatically close upon merge of PR. 
    - Pull requests should be manually reviewed by team leaders in a timely manner before being merged into main repo.

Creating GitHub Issues
- We created several GitHub Issues with tasks involving creation of CI/CD pipeline, ADR creation and a few initial tasks to complete for app home page. Each Issue was given labels and an assignee. 

## Goals for Next Meeting
- Review each component of the CI/CD pipeline as a group
- Write up steps/documentation for how to use the CI/CD pipeline and film a demo video showing how the pipeline is executed from a developer perspective.