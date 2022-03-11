## మీ mandala ను ఎంచుకోండి

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
అందరూ ఒకరికొకరు భిన్నంగా ఉంటారు. మీ mandala ప్రోగ్రామ్‌ని ఉపయోగించే వ్యక్తికి వారికి అత్యంత ప్రశాంతంగా అనిపించిన వాటి ఆధారంగా ఎంపికను ఇవ్వండి.
</div>
<div>
![](images/step_6.gif){:width="300px"}
</div>
</div>

మీరు ఇప్పుడు కనీసం రెండు వేర్వేరు mandala లను కలిగి ఉండాలి. మీరు స్టార్ట్ మెనుని సృష్టించడానికి `ask`{:class="block3sensing"} బ్లాక్‌ని ఉపయోగించవచ్చు, తద్వారా మీ mandala ప్రోగ్రామ్‌ను ఎవరు ఉపయోగిస్తున్నారో వారికి వారే ఎంపిక చేసుకోవచ్చు.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**స్టార్ట్ మెనులు**</span> తరచుగా గేమ్‌లు మరియు యాప్‌లలో కనిపిస్తాయి. అవి గేమ్ ఆడే లేదా యాప్‌ని ఉపయోగించే వ్యక్తిని అనేక ఎంపికల నుండి ఎంచుకోవడానికి అనుమతిస్తాయి, ఉదాహరణకు, వారు ఏ కారెక్టర్ ను ప్లే చేయాలనుకుంటున్నారు లేదా వారికి ఏ సెట్టింగ్‌లు కావాలి వంటివి.
</p>

మీ స్టార్ట్ మెనులో మీరు అడిగే ప్రశ్నను సృష్టించండి.

--- task ---

`when flag clicked`{:class="block3events"} బ్లాక్ కింద `ask and wait`{:class="block3sensing"} ను జోడించండి. మరియు కింది ఉదాహరణలో విధంగా, మీ ప్రశ్నకి వచనాన్ని ఎన్నుకోండి.

![Shape sprite.](images/shape_sprite.png)

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

`ask and wait`{:class="block3sensing"} ని ఉపయోగించే ముందు sprite ను దాచడానికి కారణం ఏమిటంటే, ప్రశ్న sprite నుండి స్పీచ్ బబుల్‌గా కాకుండా Stage దిగువన కనిపిస్తుంది.

![Stage దిగువన ఉన్న బాక్సు లో అడగబడిన ప్రశ్న యొక్క చిత్రం.](images/question.png)

సరైన mandala ని చూపించడానికి సరైన sprite తో సమాధానాన్ని సరిపోల్చండి.

--- task ---

`switch costume to`{:class="block3sensing"} ని `ask and wait`{:class="block3sensing"} బ్లాక్‌ కింద గల `answer`{:class="block3sensing"} బ్లాక్ కి జోడించండి.

![Shape sprite.](images/shape_sprite.png)

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

**పరీక్ష**: ఫ్లాగ్‌ని క్లిక్ చేసి, నంబర్‌ని ఎంచుకోవడం ద్వారా మీ mandala ప్రాజెక్ట్‌ను ప్రయత్నించండి.

--- /task ---

--- save ---
