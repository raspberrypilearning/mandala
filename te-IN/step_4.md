## మీ sprite ని సెటప్ చేయండి

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
మీ mandala ని రీసెట్ చేయడానికి మీ spriteని సెటప్ చేయండి.
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

ప్రస్తుతానికి, మీరు ఉపయోగించే పారామీటర్ విలువలను బట్టి మీ mandala నమూనాలు ప్రతిసారీ మారుతున్నట్లు కనిపించవచ్చు. తర్వాత, మీరు కొత్త `my blocks`{:class="block3myblocks"}ని సృష్టిస్తారు, తద్వారా మీ **mandala** sprite ఎల్లప్పుడూ అదే స్థితిలో ప్రారంభమవుతుంది.

--- task ---

`setup`{:class="block3myblocks"} అనే కొత్త బ్లాక్‌ని సృష్టించడానికి `My Blocks`{:class="block3myblocks"} మెనుని ఉపయోగించండి. బ్లాక్‌లో నాలుగు పారామీటర్‌లు ఉండాలి: `size`{:class="block3myblocks"}, `ghost`{:class="block3myblocks"}, `y`{:class="block3myblocks"}, మరియు `move`{:class ="block3myblocks"}. చింతించకండి, మీరు వీటిని మార్చవచ్చు లేదా మరిన్నింటిని తర్వాత జోడించవచ్చు.

![Shape sprite.](images/shape_sprite.png)

```blocks3
define setup: size (size) ghost (ghost) y (y) move (move)
```

--- /task ---

మీరు తదుపరి దశలో mandala ని రంగురంగులుగా చేసినప్పుడు, `ghost`{:class="block3myblocks"} బ్లాక్ రంగులను పారదర్శకంగా చేస్తుంది కాబట్టి ఆకారాలు ఒకదానిపై ఒకటి అయినప్పుడు, మీరు కలర్ మిక్సింగ్ ప్రభావాన్ని పొందుతారు.

--- task ---

ఇప్పుడు మీ sprite యొక్క రూపాన్ని మరియు స్థానాన్ని సెట్ చేయడానికి కొన్ని బ్లాక్‌లను జోడించండి.

![Shape sprite.](images/shape_sprite.png)

```blocks3
define setup: size (size) ghost (ghost) y (y) move (move)
+ set size to (size) %
+ set [ghost v] effect to (ghost)
+ go to x: (0) y: (0)
+ point in direction (90)
+ change y by (y)
+ move (move) steps
```

--- /task ---

--- task ---

ప్రస్తుతానికి, మీ `my blocks`{:class="block3myblocks"} ఉపయోగించబడలేదు, కాబట్టి మీ నమూనాపై ఎటువంటి ప్రభావం ఉండదు. `setup`{:class="block3myblocks"}కి కోడ్‌ని జోడించండి, కాబట్టి ఫ్లాగ్‌ని క్లిక్ చేసిన వెంటనే కోడ్ రన్ అవుతుంది.

![Shape sprite.](images/shape_sprite.png)

```blocks3
when flag clicked
+ setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
```

--- /task ---

--- task ---

ఫ్లాగ్‌పై క్లిక్ చేసి, డ్రా చేయబడిన నమూనాను గమనించడం ద్వారా మీ కోడ్‌ను **పరీక్షించండి**. ఆ తర్వాత, మీకు నచ్చిన నమూనా వచ్చేవరకు పారామీటర్ ల విలువలను మార్చండి.

--- /task ---

--- task ---

Sprite (దాని క్లోన్‌లు కాదు) ఇప్పటికీ కనిపిస్తుంది; ఇది చివరిలో దాచబడుతుంది, కానీ ప్రారంభంలో చూపబడాలి.

![Shape sprite.](images/shape_sprite.png)

```blocks3
when flag clicked
+ show
setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
+ hide
```

--- /task ---

--- save ---
