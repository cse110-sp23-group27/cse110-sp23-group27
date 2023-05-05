# Tarot Card js implementation (wip)

The card class will hold inside of it the link to the element which represents the class. 

The idea is that when you instantiate the class, it should create the visual html representation of itself which then automatically connects.

We then create a manager class. We will never instantiate the card classes directly, but instead we will ask the manager class to create cards and manage cards.

Some general specifications for class functionality:
```js
class Card{
    let x;
    let y;
    let scale;
    let rotationZ;
    let rotationY;

    this.instantMove(x, y);
    this.move(x, y, t);
    this.instantRotate(y, z);
    this.rotate(y, z, t);
    this.instantScale(s);
    this.scale(s, t);

    this.setBackImage(imageLink);
    this.setFrontImage(imageLink);
    
    this.whenHoverStart()
    this.whenHoverEnd()

    this.whenClicked();
}
```

```js
class CardManager{
    let allCards;

    this.createNewCard();
    this.deleteCard();
}
```