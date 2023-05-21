# Pipeline Meeting Notes

Meeting Date: 05-21-23 Elvis Joa is taking notes today.

## Attendance 
- Daniel Lee
- Kyle Smith
- Elvis Joa

## Agenda
- Set up the pipeline
- Discuss Jest for unit testing
- Discuss autoformatter and style enforcement
- Discuss JSDocs
- Discuss code quality and how to implement into the pipeline

## Topic
Using ESLint for the style enforcement and Jest for unit testing:
- Using ESLint and Jest for the pipeline results in a lot of dependencies in the repo
- Run them locally or use containers
- Can make an ADR for ESLint and Jest
- Ask TAs about this

Using JSDocs for automated documentation:
- (Rough idea) Takes comments before function headers and converts them into an HTML file/page
- See whether it can be implemented into the pipeline, or it should be run locally after merging

Using Code Climate for code quality:
- It is open-source unlike Codacy
- It checks the files for unused variables, covarage issues, and evaluates the code.
- Can make an ADR about this

## Goals To Finish By Next Meeting
- Finish pipeline
- Start coding
