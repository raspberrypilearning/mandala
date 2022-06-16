## Choose your mandala

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Everyone is different. Give the person using your mandala program a choice based on what they find most peaceful.
</div>
<div>
![](images/step_6.gif){:width="300px"}
</div>
</div>

You should now have at least two different mandalas. You can use an `ask`{:class="block3sensing"} block to create a start menu, giving a choice to whoever is using your mandala program.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**Start menus**</span> are often found in games and apps. They let the person playing the game or using the app pick from a number of options, for example, what character they want to play, or what settings they want.
</p>

Create the question you will ask in your start menu.

--- task ---

Add an `ask and wait`{:class="block3sensing"} block beneath the `when flag clicked`{:class="block3events"} and choose the text for your question, like the example below.

![The shape sprite.](images/shape_sprite.png)

```blocks3
when flag clicked
+ hide
+ ask [What feels most peaceful to you today? (1) abstract shapes (2) the earth (3) butterflies (4) love] and wait
show
setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
hide
```

--- /task ---

The reason for hiding the sprite before using the `ask and wait`{:class="block3sensing"} is so that the question appears at the bottom of the stage, rather than as a speech bubble from the sprite.

![Image of question being asked within a box at the bottom of the stage.](images/question.png)

Match the answer with the right sprite to show the right mandala.

--- task ---

Add a `switch costume to`{:class="block3looks"} `answer`{:class="block3sensing"} block underneath the `ask and wait`{:class="block3sensing"} block.

![The shape sprite.](images/shape_sprite.png)

```blocks3
when flag clicked
hide
ask [What feels most peaceful to you today? (1) abstract shapes (2) the earth (3) butterflies (4) love] and wait
+ switch costume to (answer)
show
setup: (60) (50) (10) (10) ::custom
pattern: (3) (10) (5) (60) ::custom
pattern: (5) (10) (45) (30) ::custom
pattern: (6) (10) (90) (30) ::custom
hide
```

--- /task ---

--- task ---

**Test**: Try your mandala project by clicking the flag and choosing a number.

--- /task ---

--- save ---
