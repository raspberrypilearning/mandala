## اصنع ماندالة

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
إنشاء المزيد من الأنماط لعمل ماندالة!
</div>
<div>
! [رسم متحرك يظهر نمطًا أكثر تعقيدًا يبدأ بالتشكل عند النقر على العلم.] (images / step_3.gif) {: width = "300px"}
</div>
</div>

--- task ---

انقر باليمين على مجموعتك `تعريف نمط`{:class="block3myblocks"} ثم اختر **عدل** لإضافة أنماط أكثر.

![رسم متحرك يظهر تعديل "مجموعتي" لإضافة أنماط زائدة.](images/edit-parameter.gif)

يمكنك البدء بإضافة لصاقة نص `الحجم`{:class="block3myblocks"} و مدخل `الحجم`{:class="block3myblocks"}. ثم، أضف لصاقة `حرك`{:class="block3myblocks"} و مدخل، و استخدم هذه الخيارات في المجموعات أسفله.

![الكائن الشكل.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat) size (size) move (move)
repeat (repeat)
change size by (size)
move (move) steps
create clone of (myself v)

when flag clicked
pattern: repeat (3) size (10) move (5)
```

--- /task ---

--- task ---

**اختبار:** انظر لمظهر نمطك بالضغط على العلم الأخضر لتشغيل برنامجك. لا تبدو مثل ماندالا حتى الآن! هل يمكنك التفكير في كيفية جعل النمط دائريًا؟

--- /task ---

لجعل نمطك دائريًا ويبدو أكثر مثل ماندالا، أضف إدخالًا آخر.

--- task ---

أضف إدخالًا آخرا يسمى `دور`{: class = "block3myblocks"}. ثم، مثلما تحرك مستنسخك، يمكنك تدويره كذلك.

![الكائن الشكل.](images/shape_sprite.png)

```blocks3
define pattern: repeat (repeat) size (size) move (move) turn (turn)
repeat (repeat)
change size by (size)
move (move) steps
create clone of (myself v)
+ change size by ([0] - (size))
+ move ([0] - (move)) steps
+ turn right (turn) degrees
+ move (move) steps
+ create clone of (myself v)
+ move ([0] - (move)) steps
+ turn right (turn) degrees
end
```

--- /task ---

الماندالات غالبا معقدة - يمكن أن تملك عدة صفوف تتبع أنماطا متشابهة. يمكنك إنشاء نمط أساسي لبقية صفوف الماندالة للبناء عليها.

--- task ---

حاول التلاعب بالرقم في `النمط`{:class="block3myblocks"}. يمكنك إعادة تعيين موضع وحجم كائنك، أي وقت أردت.

![صورة الصندوق التابع للكائنات بحجم، إحداثية x، و إحداثية y كلها موضوعة لصفر.](images/reset-attributes.png)

```blocks3
when flag clicked
pattern repeat (3) size (0) move (0) turn (60) ::custom
```

--- /task ---


الأن بما أنه لديك نمط أساسي، يمكنك استخدام `نمطك`{:class="block3myblocks"} عدة مرات لخلق نمط متكرر، أو 'صفوف ' ماندالة. باستخدام نفس الكود مرارًا وتكرارًا ، تخلق برنامجا **محسناً**.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">** التحسين**</span> يعني القيام بالمهمة بأكثر الطرق فعالية. انظر إلى الرسم البياني أسفله. يمكنك الانتقال من A إلى E باتباع المسار A -> B -> C -> D -> E. التحسين سيكون الانتقال A -> D -> E ، لإحتوائه خطوات أقل ومسافة أقصر.
<img src="images/map.png">
</p>

--- task ---

أسفل المجموعة `وضعية العلم منقور`{: class = "block3events"}، أضف بضع **تكرارات** أخرى إلى `نمطك`: class = "block3myblocks"}.

![الكائن الشكل.](images/shape_sprite.png)

```blocks3
when flag clicked
pattern repeat (3) size (0) move (0) turn (60) ::custom
pattern repeat (6) size (10) move (45) turn (30) ::custom
pattern repeat (6) size (10) move (90) turn (30) ::custom
```

--- /task ---

--- task ---

**اختبار:** انقر فوق العلم الأخضر،و شف أي نمط نتج. يمكنك تغيير الأرقام لتجرب أنماط تعجبك، أو حتى إضافات تكرارات أكثر إلى `نمطك`{:class="block3myblocks"}.

--- /task ---

--- save ---
