## Make a mandala

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Create more patterns to make a mandala!
</div>
<div>
![animation showing a more complicated pattern begin formed when the flag is clicked](images/step_3.gif){:width="300px"}
</div>
</div>

--- task ---

Right click on your `define pattern`{:class="block3myblocks"} block and choose **Edit** to add more parameters.

![animation showing the editing of a my blocks function to add in an extra parameter](images/edit-parameter.gif)

You can start by adding `size`{:class="block3myblocks"} and `move`{:class="block3myblocks"} and then use these parameters in the blocks below.

![shape sprite](images/shape_sprite.png)
```blocks3
define pattern (repeat) (size) (move)
repeat (repeat)
change size by (size)
move (move) steps
create clone of (myself v)

when flag clicked
pattern (3) (10) (5)
```

--- /task ---

--- task ---

To create a more complicated patern, you can add another parameter to your function called `turn`{:class="block3myblocks"}. Then as well as moving your clone, you can turn it as well.

![shape sprite](images/shape_sprite.png)
```blocks3
define pattern (repeat) (size) (move) (turn)
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

when flag clicked
pattern (3) (10) (5) (60)

```
--- /task ---

--- task ---

Try playing around with different numbers in your `pattern`{:class="block3myblocks"} function call. You can reset the position and size of your sprite anytime you like.

![image of the sprites attribute box with the size, x coordinate and y coordinate all set to zero](images/reset-attributes.png)

--- /task ---

Now that you have a basic pattern you can use your `pattern`{:class="block3myblocks"} function a number of times, to make a repeating pattern. By using the same code over and over again, you are making a program that has been **optimised**.

--- task ---

Beneath your `when flag clicked`{:class="block3events"} block, add in a few more **calls** to your `pattern`{:class="block3myblocks"} function.

![shape sprite](images/shape_sprite.png)
```blocks3
when flag clicked
pattern (3) (10) (5) (60) ::custom
pattern (5) (10) (45) (30) ::custom
pattern (6) (10) (90) (30) ::custom
```

--- /task ---

--- task ---

Click the green flag, and see what pattern is produced. You can change the numbers to experiment with patterns that you like, or even add in more calls to your `pattern`{:class="block3myblocks"} function.

--- /task ---

--- save ---
