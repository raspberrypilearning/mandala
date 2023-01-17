## Sefydla dy gorlun

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Sefydla dy gorlun i ailosod dy fandala.
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

Ar hyn o bryd, mae'n bosibl y bydd dy batrymau mandala yn newid bob tro, yn dibynnu ar y gwerthoedd paramedr rwyt ti'n eu defnyddio. Nesaf, byddi di'n creu `fy mlociau`{:class="block3myblocks"} newydd, fel bod corlun dy **mandala** bob amser yn dechrau yn yr un cyflwr.

--- task ---

Defnyddia'r ddewislen `Fy Mlociau`{:class="block3myblocks"} i greu bloc newydd o'r enw `sefydlu`{:class="block3myblocks"}. Dylai fod gan y bloc bedwar paramedr: `maint`{:class="block3myblocks"}, `ysbryd`{:class="block3myblocks"}, `y`{:class="block3myblocks"}, a `symud`{:class = "bloc3myblocks"}. Paid â phoeni, gelli newid rhain neu ychwanegu mwy nes ymlaen.

![Corlun siâp.](images/shape_sprite.png)

```blocks3
define setup: size (size) ghost (ghost) y (y) move (move)
```

--- /task ---

Pan fyddi di'n gwneud y mandala yn lliwgar yn y cam nesaf, bydd y bloc `ysbryd`{:class="block3myblocks"} yn gwneud y lliwiau'n dryloyw felly pan fydd y siapiau'n gorgyffwrdd, fe gei di effaith cymysgu lliw.

--- task ---

Nawr ychwanega rai blociau i osod ymddangosiad a lleoliad dy gorlun.

![Corlun siâp.](images/shape_sprite.png)

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

Ar hyn o bryd, nid yw dy `fy mlociau`{:class="block3myblocks"} wedi'i ddefnyddio, felly ni fydd unrhyw effaith ar dy batrwm. Ychwanega god at `sefydlu`{:class="block3myblocks"}, er mwyn i'r cod redeg cyn gynted ag y bydd y faner yn cael ei chlicio.

![Corlun siâp.](images/shape_sprite.png)

```blocks3
when flag clicked
+ setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
```

--- /task ---

--- task ---

**Profa** dy god trwy glicio ar y faner ac arsylwi'r patrwm a luniwyd. Yna, newidia werthoedd y paramedrau nes bod gen ti batrwm yr wyt yn ei hoffi.

--- /task ---

--- task ---

Mae'r corlun (nid ei glonau) i'w weld o hyd; gellir ei guddio ar y diwedd, ond bydd angen ei ddangos ar y dechrau.

![Corlun siâp.](images/shape_sprite.png)

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
