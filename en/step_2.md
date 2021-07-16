## Clone shapes to make a pattern

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Clone sprites to create a circular pattern.
</div>
<div>
![animation of a pattern ebing repeated when the flag is clicked in Scratch](images/step_2.gif){:width="300px"}
</div>
</div>

--- task ---

Open [the Scratch starter project](https://scratch.mit.edu/projects/540476254/){:target="_blank"}. Scratch will open in another browser tab. 

If you are working offline, you can download the starter project at [](https://rpf.io/p/en/puzzle-room). <mark>check links and change</mark>

--- /task ---

You should see a shape sprite that looks a little bit like a flower petal.

You will use **functions** (`my blocks`{:class="block3myblocks"}) to create a pattern with this shape. You may remember creating functions to organise your code in [Nature Rover](https://projects.raspberrypi.org/en/projects/nature-rover/3), and to repeat the same code in [Puzzle Room](https://projects.raspberrypi.org/en/projects/puzzle-room/4). Functions can also be used to optimise your programs/projects.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**Optimisation**</span> means doing things in the most efficient way. Look at the diagram below. You could get from A to E by following the path A-->B-->C-->D-->E. An optimisation would be to go A-->D-->E, which contains less steps and a shorter distance.
<img src="images/map.png">
</p>

--- task ---

Go to `My Blocks`{:class='block3myblocks'} and name your function (we have called it `pattern:`{:class="block3myblocks"}) and added `repeat`{:class="block3myblocks"} as a label to identify the first input or what programmer call a **parameter**. Then click "Add an Input" to actually create the **parameter** called `repeat`{:class="block3myblocks"}.

![animation of a my blocks being added and an additional parameter being added](images/add-parameter.gif)

![shape sprite](images/shape_sprite.png)
```blocks3
define pattern: repeat (repeat)
```

--- /task ---

To design how a pattern is made, the first step is to `define pattern`{:class='block3myblocks'}.

--- task ---

Drag the `repeat`{:class='block3myblocks'} parameter from `define pattern`{:class='block3myblocks'} into a `repeat`{:class='block3control'} loop block.

![animation showing the repeat parameter being dragged from the define block and into to repeat block](images/use-repeat.gif)

![shape sprite](images/shape_sprite.png)
```blocks3
define pattern: repeat (repeat)
repeat (repeat)
```

--- /task ---

You will now use `clone`{:class='block3control'} blocks to make the same block appear a number of times. Make sure you also add code to get the sprite to change size and move, otherwise the sprites will be stacked on top of each other and you will not be able to see them.

--- task ---

Add some code into the `repeat`{:class='block3myblocks'} loop of your `pattern`{:class='block3myblocks'} function.

![shape sprite](images/shape_sprite.png)
```blocks3
define pattern: repeat (repeat)
repeat (repeat)
+ change size by (10) // so you can see clones
+ move (5) steps // so you can see clones
+ create clone of (myself v)
```

--- /task ---

**Tip:** `Defining`{:class='block3myblocks'} the function makes a general pattern outline. What you are creating now with this function is similar to creating a spirograph stencil; it is the tool and the pattern is later created by using it. 

--- task ---

Create a pattern with your function. Get the `pattern`{:class='block3myblocks'} to `repeat`{:class='block3myblocks'} a number of times `when flag clicked`{:class='block3events'}. 

![shape sprite](images/shape_sprite.png)
```blocks3
when flag clicked
pattern (3) ::custom
```

**Test:** See what your pattern looks like by clicking the green flag to run your program.

--- /task ---

You should see the beginning of a mandala pattern. Adding more **parameters**, or requirements, to your pattern function will create the first part of your mandala.

--- save ---
