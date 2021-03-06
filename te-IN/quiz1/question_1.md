## పునశ్చరణ

బాగా చేసారు, మీరు చాలా నేర్చుకున్నారు! ఇప్పుడు, విశ్లేషించే సమయం వచ్చింది — విశ్లేషించడం అనేది నేర్చుకోవడంలో ముఖ్యమైన భాగం, ఎందుకంటే ఇది మీ మెదడులో కొత్త కనెక్షన్‌లను ఏర్పరచడంలో సహాయపడుతుంది.

మీరు నేర్చుకున్న వాటిని పరిశీలించడానికి దిగువ మూడు ప్రశ్నలకు సమాధానం ఇవ్వండి.

ప్రతి ప్రశ్న తర్వాత, సబ్మిట్ నొక్కండి. మీరు సరైన సమాధానం వైపు మార్గనిర్దేశం చేయబడతారు. మీరు ఈ చర్యను మీకు కావలసినన్ని సార్లు చేయవచ్చు.

ఆస్వాదించండి!

--- question ---

---
legend: 2లో 1వ ప్రశ్న
---

మీ ప్రాజెక్ట్‌లో, మీరు నమూనాలను రూపొందించడానికి క్లోన్‌లను ఉపయోగించారు. కింది `My Blocks`{:class='block3myblocks'} నిర్వచనాన్ని చూడండి:

```blocks3
define pattern (repeat) (size) (move) (turn)
repeat (repeat)
change size by (size)
move (move) steps
turn cw (turn) degrees
create clone of (myself v)
```

ఇక్కడ తయారుచేయబడిన నమూనా ఉంది. ![నాలుగు రేకులు సమానంగా ఉంటాయి, అన్నీ ఒకే కేంద్రం నుండి ప్రారంభమవుతాయి. ప్రతి రేక పరిమాణం పెరుగుతుంది.](images/quiz_1.png)

కింది కాల్‌లలో ఏది ఎగువ నమూనాను సృష్టిస్తుంది?

--- choices ---

- ( )
```blocks3
when flag clicked
pattern (3) (10) (0) (90)::custom
```
  --- feedback ---

ఇది మూడు క్లోన్‌లను మాత్రమే సృష్టిస్తుంది మరియు చిత్రంలో నాలుగు చూపబడ్డాయి.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
pattern (4) (10) (100) (90)::custom
```

  --- feedback ---

ఇది క్లోన్‌ను `100` దశల ద్వారా తరలించేలా చేస్తుంది, అయితే చిత్రంలోని అన్ని క్లోన్‌లు ఒకే `x` మరియు `y` కోఆర్డినేట్‌ను కలిగి ఉంటాయి.

  --- /feedback ---

- (x)

```blocks3
when flag clicked
pattern (4) (10) (0) (90)::custom
```

  --- feedback ---

అవును, ఈ కోడ్ 4 రేకులను సృష్టిస్తుంది, ప్రతి ఒక్కటి పరిమాణంలో 10 లెక్కన పెరుగుతుంది. ప్రతి రేక 90 డిగ్రీలు తిరుగుతుంది.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
pattern (4) (10) (0) (360)::custom
```

  --- feedback ---

ఇది క్లోన్‌లను పూర్తి సర్కిల్‌గా మార్చేలా చేస్తుంది, కాబట్టి మీరు ఒక పెద్ద క్లోన్‌ను మాత్రమే చూడగలరు.

  --- /feedback ---

--- /choices ---

--- /question ---
