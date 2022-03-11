## నమూనాను రూపొందించడానికి ఆకారాలను క్లోన్ చేయండి

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
నమూనాలను సృష్టించడానికి Clone sprite.
</div>
<div>
![Scratch లో ఫ్లాగ్‌ని క్లిక్ చేసినప్పుడు పునరావృతమయ్యే నమూనా యొక్క యానిమేషన్.](images/step_2.gif){:width="300px"}
</div>
</div>

--- task ---

[Scratch స్టార్టర్ ప్రాజెక్ట్ ](https://scratch.mit.edu/projects/540476254/){:target="_blank"} ని తెరవండి. Scratch మరొక బ్రౌజర్ ట్యాబ్‌లో తెరవబడుతుంది.

మీరు ఆఫ్‌లైన్‌లో పని చేస్తుంటే, మీరు [స్టార్టర్ ప్రాజెక్ట్](https://scratch.mit.edu/projects/540476254/){:target="_blank"}ని డౌన్‌లోడ్ చేసుకోవచ్చు.

--- /task ---

మీరు పూల రేకులా కనిపించే shape sprite ని చూడగలగాలి.

ఈ ఆకృతితో నమూనాను రూపొందించడానికి మీరు `my blocks`{:class="block3myblocks"}ని ఉపయోగిస్తారు. [Nature Rover](https://projects.raspberrypi.org/te-IN/projects/nature-rover/3){:target="_blank"}లో మీ కోడ్‌ని నిర్వహించడానికి `my blocks`{:class="block3myblocks"}ని సృష్టించడం మరియు [Puzzle Room](https://projects.raspberrypi.org/te-IN/projects/puzzle-room/4){:target=blank"} లో అదే కోడ్‌ను పునరావృతం చేయడం మీకు గుర్తుండవచ్చు. `My blocks`{:class="block3myblocks"}ని వేరే విధంగా చర్యలను తిరిగి ఉపయోగించడానికి కూడా వినియోగించవచ్చు.

--- task ---

`My Blocks`{:class='block3myblocks'}కి వెళ్లి మీ బ్లాక్‌లకు పేరు పెట్టండి (మనము దీనిని `pattern:`{:class="block3myblocks"} అని పిలుస్తాము). మొదటి ఇన్‌పుట్‌ను గుర్తించడానికి `repeat`{:class="block3myblocks"}ని లేబుల్‌గా జోడించండి లేదా ప్రోగ్రామర్ లు పిలిచే విధంగా **parameter**. ఆపై `repeat`{:class="block3myblocks"} అనే **parameter** ని సృష్టించడానికి "Add an Input" పై క్లిక్ చేయండి.


!['My blocks' బ్లాక్ యొక్క యానిమేషన్ మరియు అదనపు పారామీటర్ జోడించబడుతోంది.](images/add-parameter.gif)

![Shape sprite.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat)
```

--- /task ---

నమూనా ఎలా తయారు చేయబడుతుందో రూపొందించడానికి, మొదటి దశ `define pattern`{:class='block3myblocks'}.

--- task ---

`define pattern`{:class='block3myblocks'} నుంచి `repeat`{:class='block3myblocks'} పారామీటర్ ను `repeat`{:class='block3control'} లూప్ బ్లాకు లోనికి డ్రాగ్ చేయండి.

!['Repeat' పారామీటర్ ని 'define' బ్లాక్ నుండి మరియు 'repeat' బ్లాక్‌లోకి లాగినట్లు చూపుతున్న యానిమేషన్.](images/use-repeat.gif)

![Shape sprite.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat)
repeat (repeat)
```

--- /task ---

మీరు ఇప్పుడు ఒకే బ్లాక్‌ను అనేక సార్లు కనిపించేలా చేయడానికి `clone`{:class='block3control'} బ్లాక్‌లను ఉపయోగిస్తారు. Sprite పరిమాణం మరియు స్థానాన్ని మార్చడానికి మీరు కోడ్‌ను కూడా జోడించారని నిర్ధారించుకోండి, లేకుంటే sprite లు ఒకదానిపై ఒకటి పేర్చబడి ఉంటాయి మరియు మీరు వాటిని చూడలేరు.

--- task ---

మీ `pattern`{:class='block3myblocks'} యొక్క `repeat`{:class='block3myblocks'} లూప్‌లో కొంత కోడ్‌ని జోడించండి.

![Shape sprite.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat)
repeat (repeat)
+ change size by (10) //కాబట్టి మీరు క్లోన్లను చూడవచ్చు
+ move (5) steps //కాబట్టి మీరు క్లోన్లను చూడవచ్చు
+ create clone of (myself v)
```

--- /task ---

**చిట్కా:** `Defining`{:class='block3myblocks'} సాధారణ నమూనా రూపురేఖలను ఇస్తుంది. మీరు ఇప్పుడు `my blocks`{:class="block3myblocks"}తో సృష్టిస్తున్నది స్పిరోగ్రాఫ్ స్టెన్సిల్‌ని సృష్టించడం లాంటిది; ఇది ఒక సాధనం మరియు దానిని ఉపయోగించడం ద్వారా నమూనా తరువాత సృష్టించబడుతుంది.


--- task ---

మీ `my blocks`{:class="block3myblocks"}తో నమూనాను సృష్టించండి. `when flag clicked`{:class='block3events'} క్లిక్ చేసినపుడు, `pattern`{:class='block3myblocks'} ను అనేక సార్లు `repeat`{:class='block3myblocks'} కు తీసుకురండి.

![Shape sprite.](images/shape_sprite.png)
```blocks3
when flag clicked
show //ఆకారం ప్రదర్శించబడుతుంది 
set size to (50) % //చాలా పెద్దది కాదు
go to x: (0) y: (0) //మధ్యలో ప్రదర్శించబడింది
pattern: repeat (3) ::custom
```

**పరీక్ష:** మీ ప్రోగ్రామ్‌ని అమలు చేయడానికి ఆకుపచ్చ జెండాను క్లిక్ చేయడం ద్వారా మీ నమూనా ఎలా ఉందో చూడండి.

--- /task ---

మీరు mandala నమూనా యొక్క ప్రారంభాన్ని చూడాలి. మీ నమూనాకు మరిన్ని **parameters**, లేదా కావల్సినవి జోడించడం వలన మీ mandala లోని మొదటి భాగం సృష్టించబడుతుంది.

--- save ---
