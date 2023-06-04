# General Meeting

Daniel is taking notes today

# Attendance 
- Elvis Joa
- Kyle Ng
- Kyle Smith
- Jason Bui
- Daniel Lee
- Kevin Wong
- Sean Fuhrman

# Agenda

- Fix tarot card bugs (disappearing cards, home page buttons, background color changes)
- Status of unit tests and e2e tests
- Fixed ESLint errors
- Branch pruning

# Topic

Current status of tarot page
- Most tarot card bugs have been fixed (regarding disappearing cards, home page button not working, wrong colors for background)
- Basic E2E and Unit tests have been added, E2E tests do not work on GitHub Actions
- We have most ESLint errors fixed (except for jsdoc comments)
- Still have bug where cards get shifted to the right and bunched up after shuffled twice

Bone tossing/Egg fortune telling
- Probably going to be ignored/scrapped unless we have time
- Maybe use them as feature flags

Goals for next meeting
- Start localstorage for tarot cards (local storage button to store cards)
- Create tarot card deck page for retrieving local storage stored cards
- Finish service workers for offline access
- Finish E2E testing and have it work on GitHub Issues
- Reformat UI - lower priority
- Work more on polishing animations - lower priority
- User end testing (more deployment related, user analytics and feedback), related to lab 10
