# Team T - Standup 05/19

Jason is taking notes today

## Attendance 
- Elvis Joa
- Daniel Lee
- Kevin Wong
- Kyle Ng
- Jason Bui

## Agenda
- General tasks to add
- ADRs
- General design of text and website
## Topic

### General tasks for Tarot Card:
- Spreadsheets and chatGPT to generate [card responses](https://docs.google.com/spreadsheets/d/14ThlNX7FN1wzMpI35uaOgloFzLrvEMEwbLvUOah7G8Q/edit#gid=0) (should match rider-waite tarot deck)
- Basic homepage layout/navigation (Goal 1 ADR)
- Displaying the card text when Tarot cards are clicked
- Switch card images when card is clicked (placeholder animation)
- Local first data saving (make sure website are accessible without internet)
- Expandable features (need to define this better)

### ADR: Goal 1 - Basic layout
- Create a basic homepage where we can only select the Tarot Cards option. (nothing fancy, just to test if we can navigate pages correctly).
- When on the tarot card page, it shows 3 evenly spaced boxes with a black border around them.
- When a card is clicked, highlight the card (red highlight) and list text at the bottom (flip card animation?)
    - Card fortune response is shown at the bottom by changing HTML innertext element to that response
    - Possible improvement: if card is clicked, puts a dim filter over background (like card games) and pulls clicked card to the center, if the background clicked again then card goes away
    - Keep responses in a const string array in the code
    - 0-21 indexes and assign to card
    - ***Use js objects, each card is an object with name, past, present, future and card image as fields (ADR)***
        - ***Makes code more readable and easier to modify/delete cards***
    - Shuffling animation when tarot cards are loaded in? (more animation team)
    - Cards are face down at the beginning
    - Unit tests and E2E (End to end) testing (after basic framework and some cards added)
        - Check for 22 card responses, and check if responses match with a text file kept in directory
    - Unit testing design sheet
### Design of text and website:
- Maybe add navigation bar (burger bar)
- Possible tarot card design: [here](https://www.thetarotlady.com/tarot-card-meanings/)
- Possible Settings: language, more bones for bone tossing
- Generating card images using AI? 
    - Considering [image generation](https://app.leonardo.ai/) 

# Next Meeting Goal
- Set up the pipeline and ADRs
- Working on the sprint

