## अपना स्प्राइट सेट करें

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
अपने मंडला को रीसेट करने के लिए अपना स्प्राइट सेट करें।
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

इस समय, आपके द्वारा उपयोग किए जाने वाले पैरामीटर मानों के आधार पर, आपके मंडला पैटर्न हर बार बदलते हुए दिखाई दे सकते हैं। इसके बाद, आप एक नया `my blocks`{:class="block3myblocks"} बनाएंगे, ताकि आपका **mandala** स्प्राइट हमेशा उसी अवस्था में शुरू हो।

--- task ---

`setup`{:class="block3myblocks"} नामक एक नया ब्लॉक बनाने के लिए `My Blocks`{:class="block3myblocks"} मेनू का उपयोग करें। ब्लॉक में चार पैरामीटर होने चाहिए: `size`{:class="block3myblocks"}, `ghost`{:class="block3myblocks"}, `y`{:class="block3myblocks"}, और `move`{:class="block3myblocks"}। चिंता न करें, आप इन्हें बदल सकते हैं या बाद में और जोड़ सकते हैं।

![shape स्प्राइट।](images/shape_sprite.png)

```blocks3
define setup: size (size) ghost (ghost) y (y) move (move)
```

--- /task ---

जब आप अगले चरण में मंडला को रंग-बिरंगा बनाते हैं, तो `ghost`{:class="block3myblocks"} ब्लॉक रंगों को पारदर्शी बना देगा, ताकी जब आकार अतिछादित होते हैं, तो आपको एक रंग मिश्रण प्रभाव मिलेगा।

--- task ---

अब अपने स्प्राइट की उपस्थिति और स्थिति निर्धारित करने के लिए कुछ ब्लॉक जोड़ें।

![shape स्प्राइट।](images/shape_sprite.png)

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

इस समय, आपके `my blocks`{:class="block3myblocks"} का उपयोग नहीं किया गया है, इसलिए आपके पैटर्न पर कोई प्रभाव नहीं पड़ेगा। `setup`{:class="block3myblocks"} में कोड जोड़ें, ताकि झंडे क्लिक करते ही कोड चलने लगेगा ।

![shape स्प्राइट।](images/shape_sprite.png)

```blocks3
when flag clicked
+ setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
```

--- /task ---

--- task ---

झंडे पर क्लिक करके और तैयार किये गए पैटर्न को देख कर अपने कोड का **परिक्षण** करें । फिर, पैरामीटर के मानों को तब तक बदलें जब तक आपके पास वह पैटर्न न हो जो आपको पसंद हो।

--- /task ---

--- task ---

स्प्राइट (इसके क्लोन नहीं) अभी भी दिखाई दे रहे हैं; इसे अंत में छुपाया जा सकता है, लेकिन शुरुआत में दिखाना होगा।

![shape स्प्राइट।](images/shape_sprite.png)

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
