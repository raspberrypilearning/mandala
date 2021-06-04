## Clone shapes to make a pattern

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Clone sprites to create a circular pattern.
</div>
<div>
Image, gif or video showing what they will achieve by the end of the step. ![](images/image.png){:width="300px"}
</div>
</div>

--- task ---

Open [the Scratch starter project](https://scratch.mit.edu/projects/CHANGE/editor/){:target="_blank"}. Scratch will open in another browser tab. 

If you are working offline, you can download the starter project at [](https://rpf.io/p/en/puzzle-room). <mark>check links and change</mark>

--- /task ---

You should see a shape sprite that looks a little bit like a flower petal.

You will use **functions** (`my blocks`{:class="block3myblocks"}) to create a pattern with this shape. You may remember creating functions to organise your code in [Nature Rover](https://projects.raspberrypi.org/en/projects/nature-rover/3), and repeat the same code in [Puzzle Room](https://projects.raspberrypi.org/en/projects/puzzle-room/4). Functions can also be used to optimise your programs/projects.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**Optimisation**</span> makes computer programs as efficient as possible using as little memory (or lines of code, or blocks) as possible. An easy way to think about this would be when you are planning your journey to save as much time and energy as possible:

<mark>image here</mark>
</p>

--- task ---

Go to `My Blocks`{:class='block3myblocks'} and name your function (we have called it "pattern"). Click "Add an Input" to create your first pattern requirement, called "repeat",

![](images/patternfunction)


--- /task ---

To design how a pattern is made, the first step is to `define pattern`{:class='block3myblocks'}, adding blocks to get the code to repeat.

--- task ---

Add a `repeat`{:class='block3control'} block with a `repeat`{:class='block3myblocks'} parameter inside, by dragging a `repeat`{:class='block3myblocks'} from `define pattern`{:class='block3myblocks'} into the `repeat`{:class='block3control'} block.

<mark>GIF probably necessary as it is hard to explain this..</mark>

```blocks3
define pattern (repeat)
repeat (repeat)
change size by (10)
move (5) steps
create clone of (myself v)
```

--- /task ---

**Tip:** The function makes a general pattern outline. What you are creating now with this function is similar to creating a spirograph stencil; it is the tool and the pattern is later created using it. 

<mark>GIF of spirograph??</mark>

--- task ---

Create a pattern with your function. Get the `pattern`{:class='block3myblocks'} to `repeat`{:class='block3myblocks'} a number of times `when flag clicked`{:class='block3events'}. 

```blocks3
when flag clicked
pattern (3)
```

**Test:** See what your pattern looks like by clicking the green flag to run your program.

--- /task ---

You should see some shapes stacked on top of each other. Because a mandala is circular, adding to the code will make it look more like a mandala pattern

--- task ---

```blocks3
define pattern (repeat)
repeat (repeat)
change size by (size)
move (5) steps
create clone of (myself v)

```

 "size", "move", and "turn"


```blocks3
define pattern %repeat %size %move %turn
repeat (repeat :: reporter :: custom)
change size by (size :: reporter :: custom)
move (move :: reporter :: custom) steps
create clone of (myself v)
change size by ([0] - (size :: reporter :: custom))
move ([0] - (move :: reporter :: custom)) steps
turn right (turn :: reporter :: custom) degrees
move (move :: reporter :: custom) steps
create clone of (myself v)
move ([0] - (move :: reporter :: custom)) steps
turn right (turn :: reporter :: custom) degrees
end
```

--- /task ---

--- task ---

--- /task ---

--- task ---

--- /task ---

--- task ---

--- /task ---

--- task ---

--- /task ---

--- task ---

--- /task ---

--- task ---

--- /task ---

--- task ---

--- /task ---

--- task ---

--- /task ---

--- save ---