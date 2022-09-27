## सोचिए

Answer the two questions. There are hints to guide you to the correct answer.

आपने जो सीखा है उस पर चिंतन करने के लिए नीचे दिए गए दो प्रश्नों के उत्तर दें।

प्रत्येक प्रश्न के बाद, सबमिट करें दबाएं। आपको सही उत्तर की ओर निर्देशित किया जाएगा। आप इस गतिविधि को जितनी बार चाहें उतनी बार कर सकते हैं।

--- question ---

---
legend: 2 में से पहला प्रश्न
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

अपने प्रोजेक्ट में, आपने पैटर्न बनाने के लिए क्लोन का उपयोग किया था। निम्नलिखित `My Blocks`{:class='block3myblocks'} परिभाषा को देखें:![four petals equally spaced, all starting from the same center. Each petal increases in size.](images/quiz_1.png)

यहां वह एक पैटर्न है जो बनाया गया है।

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
