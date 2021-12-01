## Reflection

Well done, you have learned a lot! Now it's time to reflect - reflecting is an important part of learning because it helps make new connections in your brain.

Answer the three questions below to reflect on what you've learned.

After each question, press submit. You will be guided towards the correct answer. You can do this activity as many times as you want to.

Have fun!

--- question ---

---
legend: Question 1 of 2
---

In your project, you used clones to create patterns. Look at the following `My Blocks`{:class='block3myblocks'} definition:

```blocks3
define pattern (repeat) (size) (move) (turn)
repeat (repeat)
change size by (size)
move (move) steps
turn cw (turn) degrees
create clone of (myself v)
```

Here is a pattern that has been created. ![four petals equally spaced, all starting from the same center. Each petal increases in size.](images/quiz_1.png)

Which of the following calls would create the pattern above?

--- choices ---

- ( )
```blocks3
when flag clicked
pattern (3) (10) (0) (90)::custom
```
  --- feedback ---

This would only create three clones, and there are four shown in the image.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
pattern (4) (10) (100) (90)::custom
```

  --- feedback ---

This would make the clone move by `100` steps, but all the clones in the image have the same `x` and `y` coordinate.

  --- /feedback ---

- (x)

```blocks3
when flag clicked
pattern (4) (10) (0) (90)::custom
```

  --- feedback ---

Yes, this code creates 4 petals, each increasing in size by 10. Each petal has rotated 90 degrees.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
pattern (4) (10) (0) (360)::custom
```

  --- feedback ---

This would make the clones turn a full circle, so you would only be able to see a single large clone.

  --- /feedback ---

--- /choices ---

--- /question ---
