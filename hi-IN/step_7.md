## अपना मंडला चुनें

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
हर कोई अलग है। अपने मंडला कार्यक्रम का उपयोग करने वाले व्यक्ति को इस आधार पर विकल्प दें कि उन्हें सबसे शांतिपूर्ण क्या लगता है।
</div>
<div>
![](images/step_6.gif){:width="300px"}
</div>
</div>

अब आपके पास कम से कम दो अलग-अलग मंडला होने चाहिए। आप स्टार्ट मेनू बनाने के लिए `ask`{:class="block3sensing"} ब्लॉक का उपयोग कर सकते हैं, जो ताकि जो भी आपके मंडला प्रोग्राम का उपयोग करता है उसे विकल्प मिलता है ।

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**स्टार्ट मेनू**</span> अक्सर गेम और ऐप्स में पाया जाता है। वे गेम खेलने वाले या ऐप का उपयोग करने वाले व्यक्ति को कई विकल्पों में से चुनने देते हैं, उदाहरण के लिए, वे कौन सा चरित्र खेलना चाहते हैं, या वे कौन सी सेटिंग्स चाहते हैं।
</p>

वह प्रश्न बनाएं जो आप अपने स्टार्ट मेनू में पूछेंगे।

--- task ---

एक `ask and wait`{:class="block3sensing"} ब्लॉक `when flag clicked`{:class="block3events"} के नीचे जोड़ें और नीचे दिए गए उदाहरण की तरह अपने प्रश्न के लिए टेक्स्ट चुनें।

![shape स्प्राइट।](images/shape_sprite.png)

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

`ask and wait`{:class="block3sensing"} का उपयोग करने से पहले स्प्राइट को छिपाने का कारण यह है कि प्रश्न स्प्राइट से भाषण बुलबुले के बजाय मंच के निचले भाग में दिखाई देता है।

![मंच के नीचे एक बॉक्स में पूछे जा रहे प्रश्न की छवि।](images/question.png)

सही मंडला दिखाने के लिए उत्तर को सही स्प्राइट से मिलाएं।

--- task ---

`ask and wait`{:class="block3sensing"} ब्लॉक के नीचे वाले `answer`{:class="block3sensing"} ब्लॉक में एक `switch costume to`{:class="block3looks"} ब्लॉक जोड़ें।

![shape स्प्राइट।](images/shape_sprite.png)

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

**परिक्षण **: झंडे पर क्लिक करके और एक परिक्षण चुनकर अपने मंडला प्रोजेक्ट को आज़माएँ।

--- /task ---

--- save ---
