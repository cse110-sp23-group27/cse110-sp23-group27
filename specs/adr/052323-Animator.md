let’s briefly discuss what kind of thing we want to work on and how we are gonna divide up the work.
I think we will begin with just the tarot cards and their general functionality. As mentioned before we will work on how to animate them and whatnot.
So here is my general view of how we will structure the code. It would be ideal if we could just create a js class called TarotCard through which we will probably drive most of the interaction. We will then hopefully be able to just call things in something similar to the following:

```
let myTarotCard = new TarotCard("Some Card Name", "./images/some-card-image.jpg", "./images/card-back.jpg");
myTarotCard.instantMove(0, 0); // move to 0, 0 (x, y) instantly
myTarotCard.move(20, 30, 500); // move to 20, 30 (x, y) in 500 ms
myTarotCard.flip(); // flips the card over
```
and etc.
The hope is that this will make it easy to make scripted sequences and will give us freedom on what we want to represent.
At the moment I have following methods in mind:
```
TarotCard.move();
TarotCard.moveInstantly();
TarotCard.rotate();
TarotCard.rotateInstantly();
TarotCard.flip();
TarotCard.setFlip();
```
If you guys have any other method ideas, or features we should add in let me know and we can discuss how to implement them or how to add them in.
For how the animation component itself will work, what I had in mind is that we can create an interval that some X ms. We can then make a list of objects that describe some animation that animates some value from A, to B. The object then also holds two methods. one to get the current value of the value we are animating, and then another method to set that value.
So for example for rotation, the value we are animating is the degree of rotation. Lets call it r
We then make an object like so:
```
let animationObj = {
    getter: ()=>myTarotCard.getRotation, // method that gets the current value of the rotation
    setter: (x)=>myTarotCard.setRotation(x), // method that sets the rotation to some new value
    from: 0, // some starting value of the animation. In this case start with rotation of 0
    to: 90, // some end value of the animation. In this case by the end the animation should rotate it to 90 degrees
    time: 500 // some time the animation should take. In this case set to 500 ms
}
```
we can then make a separate manager that holds an array of these objects, and then on some interval moves the values between from  and to .
I think this is a flexible system. If you are curious to find out more about the specifics of animation such as animation curves (which I think we will make a stretch goal), here are some cool youtube videos:  
https://www.youtube.com/watch?v=Nc9x0LfvJhI (animation curves)  
https://www.youtube.com/watch?v=_KRb_qV9P4g (animation interpolation, the thing of getting the inbetween position given time and two points)

### Update May 25th

## Some details we missed
* Accessibility of the class and possible modification/deletion of the animation after it began running
* Animation curves
* Animation callbacks

## Accessibility of the class
The class needs to idealy be callable from anywhere. One way to do it is to just make a new Animator everytime, but this presents scoping issues. 

For example what if we want to later edit or somehow delete some animation once it started running.

 If we make a new object every time we lose the pointer to the list of the animation objects. 

It would be better if there was only one object which manages all of them.

Aditionally if we do that then we need to constantly make and clear intervals which could be its own problem, and instead of running multiple intervals we could just run all the animation on the same frame which would reduce jitter (as in they would jitter together).

## Animation curves
If we animate everything linearly it will look strange. This can be retrified by using Animation curves. How fast we are moving from point A to point B in a non linear fashion depends on the equaltion we use. After talking to some of the team members it was decided to just use "ease in out" curve since it is the most general purpose one.

## Animation Callbacks  
The animations often need to be played in sequence one after another, and so there were two ways of achieving this that we discussed.
1. Promises
2. Callbacks

While both can result the same thing, promises will result in a cleaner implementation, but might be overcomplicated in when to use async calls especially since we only ever need two animations at most sequenced.

Thus we decided to use callbacks since they might just be more intuitive despite slightly more confusing code in instances of longer animations.
