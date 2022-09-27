## ಪುನರ್ಮನನ

Answer the two questions. There are hints to guide you to the correct answer.

ನೀವು ಕಲಿತಿದ್ದನ್ನು ಪುನರ್ಮನನ ಮಾಡಲು ಈ ಕೆಳಗಿನ ಮೂರು ಪ್ರಶ್ನೆಗಳಿಗೆ ಉತ್ತರಿಸಿ.

ಪ್ರತಿಯೊಂದು ಪ್ರಶ್ನೆಯ ನಂತರ, ಸಬ್ಮಿಟ್‌ ಒತ್ತಿ. ಸರಿಯಾದ ಉತ್ತರದ ಕಡೆಗೆ ನಿಮಗೆ ಮಾರ್ಗದರ್ಶನ ನೀಡಲಾಗುತ್ತದೆ. ಈ ಚಟುವಟಿಕೆಯನ್ನು ನೀವು ಎಷ್ಟು ಸಲ ಬೇಕಾದರೂ ಮಾಡಬಹುದು.

--- question ---

---
legend: ಪ್ರಶ್ನೆ 1 ರಲ್ಲಿ 2
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

ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ನಲ್ಲಿ, ನೀವು ವಿನ್ಯಾಸಗಳನ್ನು ರಚಿಸಲು ತದ್ರೂಪಗಳನ್ನು ಉಪಯೋಗಿಸಿದಿರಿ. ಈ ಕೆಳಗಿನ `My Blocks`{:class='block3myblocks'} ವ್ಯಾಖ್ಯಾನವನ್ನು ನೋಡಿ:![four petals equally spaced, all starting from the same center. Each petal increases in size.](images/quiz_1.png)

ಇಲ್ಲಿ ಒಂದು ವಿನ್ಯಾಸವನ್ನು ರಚಿಸಲಾಗಿದೆ.

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
