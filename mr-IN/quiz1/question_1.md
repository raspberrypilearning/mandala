## परावर्तन

Answer the two questions. There are hints to guide you to the correct answer.

तुम्ही काय शिकलात याचे चिंतन करण्यासाठी खालील तीन प्रश्नांची उत्तरे द्या.

प्रत्येक प्रश्नानंतर submit दाबा. तुम्हाला योग्य उत्तराचे मार्गदर्शन केले जाईल. तुम्हाला हवे तेवढ्या वेळा तुम्ही ही कृती करू शकता.

--- question ---

---
legend: प्रश्न 2 पैकी 1
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

या प्रोजेक्टमध्ये, तुम्ही पॅटर्न तयार करण्यासाठी क्लोनचा वापर करता. खालील `My Blocks`{:class='block3myblocks'} व्याख्या बघा:![four petals equally spaced, all starting from the same center. Each petal increases in size.](images/quiz_1.png)

येथे तयार केलेले पॅटर्न आहे.

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
