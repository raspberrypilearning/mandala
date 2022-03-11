## तुमचे मंडल निवडा

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
प्रत्येकजण वेगळा आहे. तुमचा मंडला प्रोग्राम वापरणार्‍या व्यक्तीला त्यांना सर्वात आनंददायी वाटत असलेल्या गोष्टींवर आधारित निवड द्या.
</div>
<div>
![](images/step_6.gif){:width="300px"}
</div>
</div>

तुमच्याकडे आता किमान दोन वेगळे मंडल असावेत. तुम्ही `ask`{:class="block3sensing"} ब्लॉक चा तुमचा मंडल प्रोग्राम वापरून एखाद्याला निवड देण्यासाठी start मेनू तयार करण्यासाठी वापर करू शकता.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**Start मेनू**</span> हे अनेकदा गेम आणि ऍप्स मध्ये आढळतात. यामुळे लोक अनेक पर्यायांमधून गेम खेळू शकतात किंवा ऍप पिक वापरू शकतात, उदाहरणार्थ, त्यांना कोणते कॅरेक्टर खेळायचे आहे, किंवा त्यांना कोणत्या सेटींग हव्या आहेत.
</p>

तुमच्या start मेनूमध्ये तुम्ही विचारणार असलेला प्रश्न तयार करा.

--- task ---

`ask and wait`{:class="block3sensing"} ब्लॉक हा `when flag clicked`{:class="block3events"} च्या खाली जोडा आणि खालील उदाहरणाप्रमाणे तुमच्या प्रश्नासाठी निवडा.

![shape स्प्राईट.](images/shape_sprite.png)

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

`ask and wait`{:class="block3sensing"} चा वापर करण्याआधी स्प्राईट लपविण्यासाठीचे कारण जेणेकरून प्रश्न stage च्या खाली दिसेल, स्प्राईट मधून स्पीच बबल पेक्षा निराळे.

![stage च्या खालील बॉक्स मध्ये विचारल्या जाणाऱ्या प्रश्नाची इमेज.](images/question.png)

योग्य मंडल दाखवण्यासाठी योग्य स्प्राईट सह उत्तर जुळवा.

--- task ---

`switch costume to`{:class="block3looks"} `answer`{:class="block3sensing"} ब्लॉक `ask and wait`{:class="block3sensing"} ब्लॉकच्या खाली जोडा.

![shape स्प्राईट.](images/shape_sprite.png)

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

**चाचणी**: झेंड्यावर क्लिक करून आणि संख्या निवडून तुमच्या मंडल प्रोजेक्टचा प्रयत्न करा.

--- /task ---

--- save ---
