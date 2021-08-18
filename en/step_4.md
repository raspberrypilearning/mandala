## Set up your sprite

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Set up your sprite to reset your mandala.
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

At the moment, your mandala patterns may appear to change each time, depending on the parameter values you use. Next, you will create a new function, so that your **mandala** sprite always begins in the same state.

--- task ---

Use the `My Blocks`{:class="block3myblocks"} menu to create a new block called `setup`{:class="block3myblocks"}. The block should have four parameters: `size`{:class="block3myblocks"}, `ghost`{:class="block3myblocks"}, `y`{:class="block3myblocks"}, and `move`{:class="block3myblocks"}. Don't worry, you can change these or add more later.

![The shape sprite.](images/shape_sprite.png)
```blocks3
define setup: size (size) ghost (ghost) y (y) move (move)
```

--- /task ---

When you make the mandala colourful in the next step, the `ghost`{:class="block3myblocks"} block will make the colours transparent so when the shapes overlap, you will get a colour mixing effect.

--- task ---

Now add some blocks to your function, to set the appearance and position of your sprite.

![The shape sprite.](images/shape_sprite.png)
```blocks3
define setup: size (size) ghost (ghost) y (y) move (move)
+ set size to (size) %
+ set [ghost v] effect to (ghost)
+ go to x: (0) y: (0)
+ point in direction (90)
+ change y by (y)
+ move (move) steps
```

--- /task ---

--- task ---

At the moment, the function isn't called, so there will be no effect on your pattern. Add a call to the `setup`{:class="block3myblocks"} function, as soon as the flag is clicked.

![The shape sprite.](images/shape_sprite.png)
```blocks3
when flag clicked
+ setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
```

--- /task ---

--- task ---

**Test** your code by clicking on the flag and observing the pattern that has been drawn. Then, change the values of the parameters until you have a pattern that you like.

--- /task ---

--- task ---

The sprite (not its clones) is still visible; it can be hidden at the end of the function calls, but will need to be shown at the start.

![The shape sprite.](images/shape_sprite.png)
```blocks3
when flag clicked
+ show
setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
+ hide
```

--- /task ---

--- save ---
