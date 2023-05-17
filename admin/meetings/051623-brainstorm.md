# Title 

Kevin is taking notes today

## Attendance 
- Kevin Wong
- Elvis Joa
- Trisha Tong
- Kathy Chen
- Kyle Smith
- Daniel Lee
- Kyle Ng
- Jason Bui

## Agenda
- Want to go over how we want to style our code
- Figure out how we want to implement our CI/CD
- Submit a question for the midterm(?)
- Decide on team style for coding (camel case, snake case, etc.)
- Figure out how we want to implement our ADR
- Draw a basic diagram about how our main page/project will look.
- 

## Topic
CI/CD
- IDEAS:
  - everyone works on their respective teams and we set up automated testing suites and automated style checkers.
  - We would also want to add automated unit testing (same unit testing for everyone).
  - We should be able to run the unit testing locally in order to check for ourselves, but if we forget/don't do it for some reason, then we have a Github actions running the same unit test to check our code before we commit to the main branch.
    - This will block us from committing until our code passes the unit tests.

Diagram of website:
- We're going to (at the moment) have 3 different options on the home page to choose which fortune telling app you want. They will be Tarot Cards, Oomancy (eggs), and Bone Tossing. Clicking on each of those will go to a separate screen where it will be main screen of that chosen fortune telling medium. (Associated with diagram from today)

Standups:
- We're planning on doing the bulk of our standups just through text on slack, although we could do short standups (tbd within owns teams).

Sprint:
We're going to be on a sprint basically through this week and the next

Issue Tracking:
- Figure out adding issue labels unique to each team
  - Labels for the specific part it's for (egg animation, tarot animation, bone animation, text animation, text feature).
- Fault tolerance:
  - will be done by unit testing before pushing to repo.
  - Maybe a 404 page to be displayed if something goes wrong.

Team Breakdown:
- Text team reasponsible for text animation and website functionality
- Animation team responsible for animations of tarot cards, and other stuff.

ADR:
DON'T COMMIT TO AN IDEA FOR NEW FEATURE WITHOUT DISCUSSING IT WITH THE OTHER TEAM. 
Libraries: 
- Focus on getting the main page up and running before using libraries

Team Style: (will use an automatic style formatter)
- USE CAMEL CASE
- TRY TO AVOID RECURSION
- Function guidelines:
  - characters per line: ~80
  - Same line brackets
- Comments:
  - Place comments above affected area, and make sure to date your comments.
  - For guidelines: https://cseweb.ucsd.edu/classes/fa20/cse8B-a/styleguide.html
- Variable should describe what it's being used for (no var a, var b, etc.)
  - Put a comment for each variable describing what it's doing.
  - Don't make the variable obtusely long.
  - For Constants:
    - Hard coded = ALL CAPS
    - Soft coded = not all caps
- Commit messages:
  - Think of them like variable names, trying to portray a lot of information with clarity with a short amount of space.
  - 


