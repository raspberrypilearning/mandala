## आकृतियों को एक पैटर्न बनाने के लिए क्लोन करें

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
एक पैटर्न बनाने के लिए स्प्राइट को क्लोन करें
</div>
<div>
![Scratch में ध्वज को क्लिक करने पर दोहराए जा रहे पैटर्न का एनिमेशन.](images/step_2.gif){:width="300px"}
</div>
</div>

--- task ---

[Scratch स्टार्टर प्रोजेक्ट](https://scratch.mit.edu/projects/540476254/){:target="_blank"} खोलें। Scratch दूसरे ब्राउज़र टैब में खुलेगा।

यदि आप ऑफ़लाइन काम कर रहे हैं, तो [प्रोजेक्ट स्टार्टर फ़ाइल](https://scratch.mit.edu/projects/540476254/){:target="_blank"} डाउनलोड करें

--- /task ---

आपको एक आकार का स्प्राइट देखना चाहिए जो फूल की पंखुड़ी जैसा दिखता है।

इस आकृति के साथ एक पैटर्न बनाने के लिए आप `my blocks`{:class="block3myblocks"} का उपयोग करेंगे। आपको [Nature Rover](https://projects.raspberrypi.org/en/projects/nature-rover/3){:target="_blank"} में अपने कोड को व्यवसित करने के लिए `my blocks`{:class="block3myblocks"} ka उपयोग करना याद होगा, और उसी कोड को [Puzzle Room](https://projects.raspberrypi.org/en/projects/puzzle-room/4){:target="_blank"} में दोहराना भी । `My blocks`{:class="block3myblocks"} का उपयोग क्रियाओं को एक अलग तरीके से पुन: उपयोग करने के लिए भी किया जा सकता है।

--- task ---

`My Blocks`{:class='block3myblocks'} पर जाएं और अपने ब्लॉक्स को नाम दें (हमने इसे `pattern:`{:class="block3myblocks"} नाम दिया है)। पहले इनपुट की पहचान करने के लिए एक लेबल के रूप में `repeat`{:class="block3myblocks"} जोड़ें या जिसे प्रोग्रामर **parameter** कहते हैं । फिर सही में **parameter** called `repeat`{:class="block3myblocks"} बनाने के लिए "Add an Input" पर क्लिक करें ।


![एक 'my blocks' ब्लॉक का एनिमेशन और एक अतिरिक्त पैरामीटर जोड़ा जा रहा है।](images/add-parameter.gif)

![shape स्प्राइट।](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat)
```

--- /task ---

एक पैटर्न कैसे बनाया जाता है, इसे डिजाइन करने के लिए, पहला कदम है `define pattern`{:class='block3myblocks'}।

--- task ---

`define pattern`{:class='block3myblocks'} में से `repeat`{:class='block3myblocks'} पैरामीटर को `repeat`{:class='block3control'} लूप ब्लॉक में खीचें।

![एनिमेशन जो 'repeat' पैरामीटर को 'define' ब्लॉक से 'repeat'' ब्लॉक में घसीटा हुआ दिखा रहा है ।](images/use-repeat.gif)

![shape स्प्राइट।](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat)
repeat (repeat)
```

--- /task ---

अब आप `clone`{:class='block3control'} ब्लॉक का उपयोग एक ही ब्लॉक को कई बार प्रदर्शित करने के लिए करेंगे। सुनिश्चित करें कि आप स्प्राइट के आकार और स्थिति को बदलने के लिए कोड भी जोड़ते हैं, अन्यथा स्प्राइट का एक दूसरे के ऊपर ढेर लग जायेगा और आप उन्हें नहीं देख पाएंगे।

--- task ---

आपके `pattern`{:class='block3myblocks'} के `repeat`{:class='block3myblocks'} लूप में कुछ कोड जोड़ें।

![shape स्प्राइट।](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat)
repeat (repeat)
+ change size by (10) //So you can see the clones
+ move (5) steps //So you can see the clones
+ create clone of (myself v)
```

--- /task ---

**युक्ति:** `Defining`{:class='block3myblocks'} एक सामान्य पैटर्न की रूप रेखा बनता है । अब आप `my blocks`{:class="block3myblocks"} के साथ जो बना रहे हैं वह एक स्पाइरोग्राफ स्टैंसिल बनाने के समान है; यह उपकरण है और पैटर्न बाद में इसका उपयोग करके बनाया गया है।


--- task ---

`my blocks`{:class="block3myblocks"} के साथ एक पैटर्न बनाएं। `when flag clicked`{:class='block3events'} हो `pattern`{:class='block3myblocks'} से कई बार `repeat`{:class='block3myblocks'}।

![shape स्प्राइट।](images/shape_sprite.png)
```blocks3
when flag clicked
show //Shape is displayed 
set size to (50) % //Not too big
go to x: (0) y: (0) //Displayed in the middle
pattern: repeat (3) ::custom
```

**परिक्षण:** अपने प्रोग्राम को चलाने के लिए हरे झंडे पर क्लिक करके देखें कि आपका पैटर्न कैसा दिखता है।

--- /task ---

आपको मंडला पैटर्न की शुरुआत देखनी चाहिए। अपने पैटर्न में अधिक **parameters**, या आवश्यकताएँ जोड़ने से आपके मंडल का पहला भाग बन जाएगा।

--- save ---
