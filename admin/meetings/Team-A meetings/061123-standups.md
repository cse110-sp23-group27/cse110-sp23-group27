# Team A Standups

## May 24, 2023
* Victor Kim  
**What did you work on since last standup?**  
I added some code for the Animator to run intervals and process animations  
**What are you planning to work on?**  
I am gonna test the feature and probably write some unit tests for it  
**Any blockers?**  
I am not sure if it is possible to unit test animations? We will see.  

* Trisha Tong  
**What did you work on since last standup?**  
I created a new branch and started working on the function headers for the TarotCard class.  
**What are you planning to work on?**  
I am planning on finishing the headers soon.  
**Any blockers?**  
Not exactly a blocker but hope to have a better understanding of the relationship between TarotCard and Animator.   

* Kathy Chen  
**What did you work on since last standup?**  
I created a new branch for the css style animations. I found some source code online for the fog animation which looks pretty good so I’ll probably just use that and clean it up a lil  
**What are you planning to work on?**  
Tweaking the fog style CSS and looking up glow CSS animation  
**Any blockers?**  
101 midterm tomorrow and my friend from home is coming to visit this weekend!  

* Sean Fuhrman  
**What did you work on since last standup?**  
I checked out the branch Kathy made and began thinking about how this would be implemented  
**What are you planning to work on?**  
Finding a good glow effect  
**Any blockers?**  
I'm wondering how the css will be integrated with the current page setup? We will dynamically load in the css pages with javascript?  I also will be gone this weekend on a family trip  

## May 25, 2023  
* Kyle Smith  
**What did you work on since last standup?**  
Working on getting code quality tool integrated into CI/CD pipeline.  Also reading up on animator class ADR in order to implement animator class.  
**What are you planning to work on?**  
Work on implementing animator class next.  
**Any blockers?**  
Not currently, but I might have questions as I’m working on the animator class.  

* Sean Fuhrman  
**What did you work on since last standup?**  
I implemented Kathy's fog CSS and added glow animations to the text in the tarot card page. I also added JS that uses templates to dynamically load in different html for this. This was mainly just so the webpage could load in new elements to style, but this required pretty big changes so I didn't push it to main. Although I think it could be a good solution for loading in new pages, but of course we can always change it. I kept all my changes to the css-animations branch.  
**What are you planning to work on?**  
I don't know to be honest, but I think it would be great if people could look at the css-animations branch and give feedback?  
**Any blockers?**  
I am gonna be gone this weekend for vacation! Also github is hard

* Trisha Tong  
**What did you work on since last standup?**  
I completed the function headers issue I was assigned.  
**What are you planning to work on?**  
I will make changes as necessary after my code gets reviewed.  
**Any blockers?**  
None at the moment, but next week is looking pretty busy for my other classes.  

* Victor Kim  
**What did you work on since last standup?**  
I finished most of the `Animator` class.  
**What are you planning to work on?**  
I think I will go around helping a bit and pair program with different people! @ me if you want to work on something together  
**Any blockers?**  
Need to ask TA about singleton behaviours  

## May 26, 2023  
* Kathy Chen  
**What did you work on since last standup?**  
The bulk of the CSS smoke and glow animations have been implemented so I have created a Figma project to get started on the design for the home page and implementing different backgrounds depending on which icon the mouse is hovering over.  
**What are you planning to work on?**  
Designing the home page with Trisha and Sean  
**Any blockers?**  
My friend is visiting this weekend so I probably won’t be able to work too much on it!  

## May 27, 2023  
* Victor Kim  
**What did you work on since last standup?**  
Updated some design files.  
**What are you planning to work on?**  
Planning to work on all the animations together tomorrow with Trish and Kyle  
**Any blockers?**  
None

## June 5, 2023  
* Kyle Smith  
**What did you work on since last standup?**  
Worked on getting several pipeline features, including integrating Code Climate into CI/CD pipeline, adding ADR for it, and writing some documentation to fix JSDocs errors.  
**What are you planning to work on?**  
I have setup a CSS/HTML linter that will run in our GH action CI/CD pipeline.  I will get this integrated today.  I also have some Tarot card animation code and styling that I have been working on that I will try to finish up and push today.  
**Any blockers?**  
No blockers currently.  

* Sean Fuhrman  
**What did you work on since last standup?**  
I changed the layout of the tarot card page to better match the figma design  
**What are you planning to work on?**  
I may start trying to add a local storage feature for selected cards, I also want to style the shuffle cards button  
**Any blockers?**  
None currently  

* Victor Kim  
**What did you work on since last standup?**  
Figuring out some bugs related to animations and animation curves  
**What are you planning to work on?**  
Finishing animation curves and beginning work on new features me and Elvis discussed at one point  
**Any blockers?**  
None  

## June 6, 2023  
* Trisha Tong  
**What did you work on since last standup?**  
Worked on implementing local-first storage of selected cards  
**What are you planning to work on?**  
Making an ADR for this feature  
**Any blockers?**  
None at the moment  

* Victor Kim  
**What did you work on since last standup?**  
Made some new animations for the pre shuffle, and redid how shuffle looks to make it feel a bit more like a real shuffle  
**What are you planning to work on?**  
Plan on setting up the reset button  
**Any blockers?**  
None  

## June 7, 2023  
* Trisha Tong  
**What did you work on since last standup?**  
I made an ADR for the local-first storage feature and increased the opacity of the fog animation.  
**What are you planning to work on?**  
Implementing localStorage by incorporating it into the flip methods  
**Any blockers?**  
None at the moment

* Victor Kim  
**What did you work on since last standup?**  
Updating some visual css stuff  
**What are you planning to work on?**  
Planning to work on more animations for more interesting experience  
**Any blockers?**  
None

## June 9, 2023
* Sean Fuhrman  
**What did you work on since last standup?**  
I opened a PR for cards moving up when clicked and styled the reset/ shuffle buttons  
**What are you planning to work on?**  
The video  
**Any blockers?**  
None  

* Trisha Tong  
**What did you work on since last standup?**  
I wrote what I could for the localStorage feature and worked on the fade-in animation for the text responses  
**What are you planning to work on?**  
localStorage feature  
**Any blockers?**  
I have a final tmrw so will be studying for that most of today and tmrw. Also, the timing for the fade-in animation can be improved but I’m not sure how.  

* Kathy Chen  
**What did you work on since last standup?**  
I worked on adding past, present and future labels to the display 3 cards function and changing the shuffle header to “Reveal Your” during display too  
**What are you planning to work on?**  
Help Trisha and Sean with the localStorage feature  
**Any blockers?**  
Not too many but definitely trying to start studying for finals and 140l labs  

## June 10, 2023
* Kyle Smith  
**What did you work on since last standup?**  
Added StyleLint integration to CI/CD pipeline and cleaned up style/formatting in several places. Working on getting card flipping feature and local first storage of cards feature integrated. I’m also working on Testing Coverage for CI/CD pipeline.  
**What are you planning to work on?**  
Finish testing card flipping and local first storage of cards and get PR merged.  Testing this feature. And code coverage integration.  
**Any blockers?**  
None  

* Kathy Chen  
**What did you work on since last standup?**  
I fixed the past present future labels to be above the cards so it wouldn’t interfere with response text  
**What are you planning to work on?**  
Help Trisha and Sean with the localStorage feature  
**Any blockers?**  
Not too many just studying for finals

## June 11, 2032
* Sean Fuhrman  
**What did you work on since last standup?**  
Making the cards face down and then face up when clicked, and the animation with kyle  
**What are you planning to work on?**  
The video  
**Any blockers?**  
I had a final yesterday night  

* Kyle Smith  
**What did you work on since last standup?**  
Got testing coverage for CI/CD pipeline integrated into the PR to main GH Action that works with `jest` coverage and `Code Climate` for reporting. Also worked on flipping animation and was able to get a cool flip animation working together with Sean (thanks Sean!!).  This was pushed to `card-flip` branch.  
**What are you planning to work on?**  
Adding more test coverage in places that need it, with information from test coverage reporting.  Editing a few ADRs and code cleanup.  
**Any blockers?**  
Finals and end of quarter projects  

* Trisha Tong  
**What did you work on since last standup?**  
Creating a markdown file for standups  
**What are you planning to work on?**  
The retrospective part of the public video (slides + recording)  
**Any blockers?** 
Finals  
