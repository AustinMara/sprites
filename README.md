# CODEY IN THE HOUSE
### @explicitHints true

## Codey's Block Scavenger Hunt! @showdialog

OH NO! Codey deleted his programming and needs help putting it back together! The only problem ishe lost his memory and can't remember where to find the blocks he needs!

## First block!

---

1.   Find the  
``||variables(sprites):set [mySprite] to sprite [] of kind [Player]||``<br/>
block and add it to the  <br/>
``||loops(noclick):on start||`` <br/>
container already in the workspace.
1.   Select an image from the gallery (or draw one) that looks like Codey.

---


#### ~ tutorialhint

```blocks
// @highlight
let mySprite: Sprite = sprites.create(sprites.food.smallTaco, SpriteKind.Player)
```

## Next block!

1.   Find the<br/>
``||sprites:set [mySprite] position to x [0] y[0]||``<br/>
 block.
1.   Add the block to **the bottom** of your ``||loops(noclick):on start||`` container.

Try different values for **x** and **y**.

---

#### ~ tutorialhint

```blocks
let mySprite: Sprite = sprites.create(sprites.food.smallTaco, SpriteKind.Player)
// @highlight
mySprite.setPosition(80, 80)
```

## Let's move!

1.   Find the<br/>
``||controller:move [mySprite] with buttons (+)||``<br/>
 block.
2.   Add the block to **the bottom** of your ``||loops(noclick):on start||`` container.

---

#### ~ tutorialhint

```blocks
let mySprite: Sprite = sprites.create(sprites.food.smallTaco, SpriteKind.Player)
mySprite.setPosition(80, 80)
// @highlight
controller.moveSprite(mySprite)
```

## Move some more!

1.   In your<br/>
``||controller(noclick):move [mySprite] with buttons (+)||``<br/>
block, click the **expand** button.


~hint What is the "expand" button?

---

-   The *expand* button is the plus sign at the end of the block.
hint~

---

## STOP! FIND YOUR INSTRUCTOR
Call your instructor over to talk about these questions:
-   What new items appear when you press the + button?
-   What happens when you change the values of **vx** and **vy**?
-   How can you use those values to make the sprite **only** move
**horizontally** (left and right)?
-   How can you use those values to make the sprite **only** move
** vertically** (up and down)?
-   Are there any numbers that are **not** allowed for **vx** and **vy**?

~hint What numbers should I try? 🤷‍♂️

---

-   Try some negative numbers.
-   What happens when you try zero?
hint~


#### ~ tutorialhint

```blocks
let mySprite: Sprite = sprites.create(sprites.food.smallTaco, SpriteKind.Player)
mySprite.setPosition(80, 80)
// @highlight
controller.moveSprite(mySprite, 50, 0)
```

## Sprites can talk?

1.   Find the<br/>
``||sprites:[mySprite] say [":)"] (+) ||``<br/>
block.
2.   Add the block to **the bottom** of your ``||loops(noclick):on start||`` container.

---


#### ~ tutorialhint

```blocks
let mySprite: Sprite = sprites.create(sprites.food.smallTaco, SpriteKind.Player)
mySprite.setPosition(80, 80)
controller.moveSprite(mySprite, 50, 0)
// @highlight
mySprite.say(":)")
```

## Sprites CAN talk!

1.   In your<br/>
``||sprites(noclick):[mySprite] say [":)"] (+) ||``<br/>
block, select the **expand** button.


#### ~ tutorialhint

```blocks
let mySprite: Sprite = sprites.create(sprites.food.smallTaco, SpriteKind.Player)
mySprite.setPosition(80, 80)
controller.moveSprite(mySprite, 50, 0)
// @highlight
mySprite.say(":)", 1000)
```


### @explicitHints true


## Part 2: Renaming sprites

GREAT JOB! Looks like you found the blocks we needed but our job isn't done yet! Our code says "mySprite" but Codey has a name!

Let's learn how to change the name
of a sprite. Follow these instructions to change the
name of your sprite from **mySprite** to **codey**.

--- 

## Rename mySprite

1.   In any of the red ovals with the name **mySprite**,
select the **down arrow**. A menu appears.
1.   Select **Rename variable...**.
1.   Enter the new name, **codey**.
1.   Select the big, green **OK** button to close the menu.

Now, in every block where that sprite is used, the name has changed!

![Renaming a variable in MakeCode](https://alex-kulcsar.github.io/introcs-tutorials/assets/images/S01.L01.01.P02.rename_variable.gif)



#### ~ tutorialhint

```blocks
// @highlight
let codey: Sprite = sprites.create(sprites.food.smallTaco, SpriteKind.Player)
codey.setPosition(80, 80)
controller.moveSprite(codey, 50, 0)
codey.say(":)", 1000)
```


---

## CODEY HUNGRY!

Codey is hungry after watching you do all this work! Let's get him something to eat!

---

## Add a Food
1.   Add another sprite to your project for some sort of food.

1.   Give your new sprite an appropriate name.

1.   Change the sprite kind to **Food**.<br/>
(Watch the animation to see how to do this.)
1.   Place your food sprite in one of the empty corners of the screen.
Use a <br/>
``||variables(sprites): set [foodSprite] position to x [0] y [0]||`` <br/>
block.

![An animation showing how to change a sprite kind.](/static/courses/csintro/S01.L01.02.change_sprite_kind.gif)

---

## CODEY BORED!

Codey is jealous that you get to have sooo much fun coding! Let's add an enemy for him to play with!

---

## Add an enemy

1.   Add another sprite to your project for cody to play with.

1.   Give your new sprite a good name.

1.   Change the sprite kind to **Enemy**.<br/>
(Go back to the last step if you forgot!)
1.   Place your enemy sprite in one of the empty corners of the screen.
Use a <br/>
``||variables(sprites): set [enemySprite] position to x [0] y [0]||`` <br/>
block.

---

## THIS ENEMY STINKS!

We added a friend for codey but it doesn't really do anything. Let's fix that! 

---

1.   From the **Sprites** drawer, add a <br/>
``||sprites:set [myEnemy] follow [codey]||`` <br/>
block.
1.   Make the enemy chase the hero.
    *   In this new block, make the first variable your enemy sprite.
    *   In this new block, make the second variable your hero sprite.
1.  Wait for the simulator to restart.
1.  Move your hero sprite around the screen.
1.  How does the enemy sprite react? 

#### ~ tutorialhint

```blocks
let codey: Sprite = sprites.create(img`1`, SpriteKind.Player)
codey.setPosition(40, 30)
controller.moveSprite(codey)
codey.setStayInScreen(true)
let enemySprite: Sprite = sprites.create(img`2`, SpriteKind.Enemy)
enemySprite.setPosition(120, 90)
// @highlight
enemySprite.follow(codey)
let foodSprite: Sprite = sprites.create(img`3`, SpriteKind.Food)
foodSprite.setPosition(120, 30)
```

## COME BACK CODEY!
You probably noticed that Codey likes to run away where we can't see him. If we lose Codey then the Coding Club will have to close!
Let's fix this!

---

1.   From the **Sprites** drawer, add a <br/>
``||sprites:set [mySprite] stay in screen <ON>||``<br/>
block.
1.   In this new block, click on the down arrow to change the
name of the sprite to Codey.
1.   Wait for the simulator to restart.
1.   Move the hero sprite around the screen. <br/>It stays on the screen now!

#### ~ tutorialhint

```blocks
let codey: Sprite = sprites.create(img`1`, SpriteKind.Player)
codey.setPosition(40, 30)
controller.moveSprite(codey)
// @highlight
codey.setStayInScreen(true)
let enemySprite: Sprite = sprites.create(img`2`, SpriteKind.Enemy)
enemySprite.setPosition(120, 90)
let foodSprite: Sprite = sprites.create(img`3`, SpriteKind.Food)
foodSprite.setPosition(120, 30)

```

---

## GREAT JOB!
You finished helping Codey! Call your instructor over to check your work!
In the next part we are going to make a game for Codey to play!