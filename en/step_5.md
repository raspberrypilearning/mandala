## Mandala colouring

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Give  the user the opportunity to colour different parts of the mandalas.
</div>
<div>
![](images/step_7.gif){:width="300px"}
</div>
</div>

**Tip:** If you want to, you can print out your mandala before you add colour to it in this step, and use it as a colouring pattern to colour by hand.

--- task ---

Look at the current costumes for your **shape** sprite. You will see that there are two costumes, one white and the other filled in.

![Two costumes for the sprite.](images/costumes.png)

--- /task ---

To add colour to your mandala, each of the clone shapes should change its `costume`{:class="block3looks"} and then its `color effect`{:class="block3looks"} when the clone is clicked. The new costume will be **one** more than whatever the previous costume was, so it will change to the coloured version and then to the different colours.

--- task ---

Add a `when this sprite clicked`{:class="block3events"} block, and then use the `+`{:class="block3operators"} operator to change the costume number.

![The shape sprite.](images/shape_sprite.png)

```blocks3
when this sprite clicked
switch costume to ((answer) + (1))
```

--- /task ---

--- task ---

Add a `change color effect`{:class="block3looks"} block to this script, so that each time the sprite is clicked, the colour changes a little.

![The shape sprite.](images/shape_sprite.png)

```blocks3
when this sprite clicked
switch costume to ((answer) + (1))
change [color v] effect by (25)
```

--- /task ---
 
--- task ---

Create the kind of colouring effect you want by changing your `ghost`{:class="block3myblocks"} numbers. A lower `ghost`{:class="block3myblocks"} number will mean the colour is more saturated, like a permanent marker. A high `ghost`{:class="block3myblocks"} number will mean the colour is less saturated, like watercolours.

--- /task ---

--- task ---

**Test:** Click the flag, choose your costume, and then try clicking on the clones to change their colours. 

![A mandala made of hearts that have been coloured in a variety of different colours.](images/coloured_mandala.png)

You should get a kaleidoscope effect when colours are layered on top of each other.

--- /task ---

If you like the mandala you have created then you can **right-click** on the stage, and choose to save the image.

![The contect menu appears when the Stage is right-clicked, and the 'Save Image As' option is highlighted.](images/save_mandala.png)

--- save ---
