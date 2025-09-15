 #Part 1: Blocks Scavenger Hunt!
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

**STOP! FIND YOUR INSTRUCTOR**
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

#Part 2: Renaming variables
### @explicitHints true


## Renaming sprites @showdialog

GREAT JOB! Looks like you found the blocks we needed but our job isn't done yet! Our code says "mySprite" but Codey has a name!

Let's learn how to change the name
of a sprite. Follow these instructions to change the
name of your sprite from **mySprite** to **codey**.

Let's change the name of your sprite to **codey**.

**Note**: Scroll down to see a video of the following steps.

---

1.   In any of the red ovals with the name **mySprite**,
select the **down arrow**. A menu appears.
1.   In that menu, select **Rename variable...**.
1.   In the dialog that appears, enter the new name, **codey**.
1.   Select **OK** or press **Enter** on your keyboard to close the dialog.

Now, in every block where that sprite is used, the name has changed!

In all future programs, make sure to give your sprites meaningful names!

![Renaming a variable in MakeCode](https://alex-kulcsar.github.io/introcs-tutorials/assets/images/S01.L01.01.P02.rename_variable.gif)



#### ~ tutorialhint

```blocks
// @highlight
let codey: Sprite = sprites.create(sprites.food.smallTaco, SpriteKind.Player)
codey.setPosition(80, 80)
controller.moveSprite(codey, 50, 0)
codey.say(":)", 1000)
```

```template
let mySprite: Sprite = sprites.create(sprites.food.smallTaco, SpriteKind.Player)
mySprite.setPosition(80, 80)
controller.moveSprite(mySprite, 50, 0)
mySprite.say(":)", 1000)
```


> Open this page at [https://austinmara.github.io/sprites/](https://austinmara.github.io/sprites/)

## Use as Extension

This repository can be added as an **extension** in MakeCode.

* open [https://arcade.makecode.com/](https://arcade.makecode.com/)
* click on **New Project**
* click on **Extensions** under the gearwheel menu
* search for **https://github.com/austinmara/sprites** and import

## Edit this project

To edit this repository in MakeCode.

* open [https://arcade.makecode.com/](https://arcade.makecode.com/)
* click on **Import** then click on **Import URL**
* paste **https://github.com/austinmara/sprites** and click import

#### Metadata (used for search, rendering)

* for PXT/arcade
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
