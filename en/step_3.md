## Make a mandala

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Create more patterns to make a mandala!
</div>
<div>
![Animation showing a more complicated pattern beginning to form when the flag is clicked.](images/step_3.gif){:width="300px"}
</div>
</div>

--- task ---

Right click on your `define pattern`{:class="block3myblocks"} block and choose **Edit** to add more parameters.

--- /task ---

--- task ---

Start by adding a `size`{:class="block3myblocks"} text label and a `size`{:class="block3myblocks"} input. Then, add a  `move`{:class="block3myblocks"} label and input.

![Animation showing the editing of 'my blocks' to add in extra parameters.](images/edit-parameter.gif)

--- /task ---

--- task ---

Add the following blocks to your script:

![The shape sprite.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat) size (size) move (move)
repeat (repeat)
change size by (size)
move (move) steps
create clone of (myself v)

when flag clicked
pattern: repeat (3) size (10) move (5)
```

--- /task ---

--- task ---

**Test:** See what your pattern looks like by clicking the green flag to run your program. It doesn't look like a mandala yet! Can you think of how you might make the pattern circular?

--- /task ---

--- task ---

Add another input called `turn`{:class="block3myblocks"}. Then, as well as moving your clone, you can turn it as well.

--- /task ---

--- task ---

Add the new input to your code:

![The shape sprite.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat) size (size) move (move) turn (turn)
repeat (repeat)
change size by (size)
move (move) steps
create clone of (myself v)
+ change size by ([0] - (size))
+ move ([0] - (move)) steps
+ turn right (turn) degrees
+ move (move) steps
+ create clone of (myself v)
+ move ([0] - (move)) steps
+ turn right (turn) degrees
end
```

--- /task ---

--- task ---

Try playing around with different numbers in your `pattern`{:class="block3myblocks"}. You can reset the position and size of your sprite anytime you like.

![Image of the sprites' attribute box with the size, x coordinate, and y coordinate all set to zero.](images/reset-attributes.png)

```blocks3
when flag clicked
pattern repeat (3) size (0) move (0) turn (60) ::custom
```

--- /task ---

--- task ---

Beneath your `when flag clicked`{:class="block3events"} block, add in a few more **calls** to your `pattern`{:class="block3myblocks"}.

![The shape sprite.](images/shape_sprite.png)

```blocks3
when flag clicked
pattern repeat (3) size (0) move (0) turn (60) ::custom
pattern repeat (6) size (10) move (45) turn (30) ::custom
pattern repeat (6) size (10) move (90) turn (30) ::custom
```

--- /task ---

--- task ---

**Test:** Click the green flag, and see what pattern is produced. You can change the numbers to experiment with patterns that you like, or even add in more calls to your `pattern`{:class="block3myblocks"}.

--- /task ---

--- save ---
