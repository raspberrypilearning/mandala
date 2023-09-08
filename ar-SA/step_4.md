## جهز كائنك

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
قم بإعداد الكائن الخاص بك لإعادة ضبط الماندالا الخاصة بك.
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

في الوقت الحالي، قد تبدو أنماط الماندالا الخاصة بك تتغير في كل مرة، اعتمادًا على قيم المعلمات التي تستخدمها. بعد ذلك، ستقوم بإنشاء `my block`{:class="block3myblocks"} جديد، بحيث يبدأ كائن **mandala** الخاص بك دائمًا في نفس الحالة.

--- task ---

استخدم قائمة `My Blocks`{:class="block3myblocks"} لإنشاء كتلة جديدة تسمى `setup`{:class="block3myblocks"}. يجب أن تحتوي الكتلة على أربع معلمات: `size`{:class="block3myblocks"}، `Ghost`{:class="block3myblocks"}، `y`{:class="block3myblocks"}، و `move`{:class = "block3myblocks"}. لا تقلق، يمكنك تغيير هذه العناصر أو إضافة المزيد لاحقًا.

![الكائن الشكل.](images/shape_sprite.png)

```blocks3
define setup: size (size) ghost (ghost) y (y) move (move)
```

--- /task ---

عندما تجعل الماندالا ملونة في الخطوة التالية، فإن الكتلة `شبح`{:class="block3myblocks"} ستجعل الألوان شفافة لذلك عندما تتداخل الأشكال، سوف تحصل على تأثير مزج الألوان.

--- task ---

أضف الآن بعض الكتل لتعيين مظهر وموضع الكائن الخاص بك.

![الكائن الشكل.](images/shape_sprite.png)

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

في الوقت الحالي، لم يتم استخدام `my blocks`{:class="block3myblocks"}، لذلك لن يكون هناك أي تأثير على النمط الخاص بك. أضف الكود إلى `setup`{:class="block3myblocks"}، بحيث يتم تشغيل الكود بمجرد النقر على العلم.

![الكائن الشكل.](images/shape_sprite.png)

```blocks3
when flag clicked
+ setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
```

--- /task ---

--- task ---

**اختبر** الخاص بك عن طريق النقر على العلم ومراقبة النموذج الذي تم رسمه. ثم قم بتغيير قيم المعلمات حتى تحصل على النمط الذي تريده.

--- /task ---

--- task ---

لا يزال الكائن (وليس نسخه) مرئيًا؛ يمكن إخفاؤه في النهاية، لكن يجب إظهاره في البداية.

![الكائن الشكل.](images/shape_sprite.png)

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
