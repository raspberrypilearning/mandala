## استنسخ الأشكال لعمل نمط

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
استنسخ الكائنات لعمل نمط.
</div>
<div>
![رسم متحرك لنمط يتكرر عند ضغط العلم الأخضر في سكراتش.](images/step_2.gif){:width="300px"}
</div>
</div>

--- task ---

افتح [ مشروع المبتدئ لسكراتش](https://scratch.mit.edu/projects/540476254/){:target="_blank"}. سيتم فتح Scratch في علامة تبويب متصفح أخرى.

إذا كنت تعمل دون اتصال ، يمكنك تنزيل [مشروع المبتدئ](https://scratch.mit.edu/projects/540476254/){: target = "_ blank"}.

--- /task ---

يفترض أن ترى كائن شكل يشبه إلى حد ما بتلة زهرة.

ستستخدم `كتلتي`{: class = "block3myblocks"} لإنشاء نمط بهذا الشكل. ربما تتذكر ` كتلتي`{:class="block3myblocks"} لترتيب كودك في [ كشاف الطبيعة](https://projects.raspberrypi.org/en/projects/nature-rover/3){:target="_blank"}، و لتكرار نفس الكود في [غرفة الأحجية](https://projects.raspberrypi.org/en/projects/puzzle-room/4){:target="_blank"}. ` كتلي`{:class="block3myblocks"} يمكن أيضا استعمالها لإعادة استخدام حركات بطريقة مختلفة.

--- task ---

اذهب إلى `مجموعتي`{:class='block3myblocks'} و سم مجموعاتك ( سميناها `نمط`{:class="block3myblocks"}). أضف `كرر`{:class="block3myblocks"} كلصاقة لتعريف المدخل الأول أو أي مبرمج يسمى **خيار**. ثم اضغط "أضف مدخلا" لتخلق **خيارا** يدعى `كرر`{:class="block3myblocks"}.


![رسم متحرك ل مجموعة 'مجموعتي' و خيار إضافي أُضيف.](images/add-parameter.gif)

![الكائن الشكل.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat)
```

--- /task ---

لتصميم كيف يُخلق نمط، الخطوة الأولى هي `تعريف النمط`{:class='block3myblocks'}.

--- task ---

اسحب خيار `كرر`{:class='block3myblocks'} من`عرف نمط`{:class='block3myblocks'} إلى مجموعة `كرر`{:class='block3control'} الحلقية.

![رسم متحرك يعرض خيار "كرر" يُسحب من مجموعة "تعريف" ثم إلى مجموعة "كرر".](images/use-repeat.gif)

![الكائن الشكل.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat)
repeat (repeat)
```

--- /task ---

ستستخدم الآن كتل `استنساخ` {:class='block3control'} لجعل نفس الكتلة تظهر عدة مرات. تأكد إضافتك أيضا كودا لتغيير حجم و موضع الكائن، خلاف ذلك الكائنات سيعلق فوق بعضها و لن تتمكن من رؤيتها.

--- task ---

أضف بعض الأكواد لحلقة `كرر`{:class='block3myblocks'} تبع `نمط`{:class='block3myblocks'} خاصتك.

![الكائن الشكل.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat)
repeat (repeat)
+ change size by (10) //So you can see the clones
+ move (5) steps //So you can see the clones
+ create clone of (myself v)
```

--- /task ---

**نصيحة** `تعريف`{:class='block3myblocks'} تعمل نمطا عاما مختصرا. الذي تنشئه الآن بـ ` مجموعتي`{:class="block3myblocks"} مشابه لإنشاء مرسام سبيروغراف، هي الأدات و النمط الذي سينشأ باستخدامه.


--- task ---

خلق نمط ب `مجموعتي`{:class="block3myblocks"} خاصتك. اجعل `النمط`{:class='block3myblocks'} `يتكرر`{:class='block3myblocks'} عددا من المرات `عند نقر العلم الأخضر`{:class='block3events'}.

![الكائن الشكل.](images/shape_sprite.png)
```blocks3
when flag clicked
show //Shape is displayed 
set size to (50) % //Not too big
go to x: (0) y: (0) //Displayed in the middle
pattern: repeat (3) ::custom
```

**اختبار:** انظر لمظهر نمطك بالضغط على العلم الأخضر لجعل البرنامج يشتغل.

--- /task ---

يفترض رؤيتك بداية نمط ماندالة. إضافة **خيارات** أكثر، أو متطلبات، لنمطك سيخلق الجزء الأول لماندالتك.

--- save ---
