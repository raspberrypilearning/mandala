## Configurer ton sprite

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Configure ton sprite pour réinitialiser ton mandala.
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

Pour l'instant, tes motifs de mandala peuvent sembler changer à chaque fois, selon les valeurs de paramètres que tu utilises. Ensuite, tu vas créer un nouveau `Mes Blocs`{:class="block3myblocks"}, afin que ton sprite **mandala** commence toujours dans le même état.

--- task ---

Utilise le menu `Mes Blocs`{:class="block3myblocks"} pour créer un nouveau bloc appelé `configuration`{:class="block3myblocks"}. Le bloc doit avoir quatre paramètres : `taille`{:class="block3myblocks"},`fantôme`{:class="block3myblocks"}, `y`{:class="block3myblocks"}, et `déplacer`{:class="block3myblocks"}. Ne t'inquiète pas, tu peux les modifier ou les ajouter plus tard.

![Le sprite "Forme".](images/shape_sprite.png)

```blocks3
define setup: size (size) ghost (ghost) y (y) move (move)
```

--- /task ---

Lorsque tu rendras le mandala coloré à l'étape suivante, le bloc `fantôme`{:class="block3myblocks"} rendra les couleurs transparentes de sorte que lorsque les formes se chevaucheront, tu obtiendras un effet de mélange de couleurs.

--- task ---

Ajoute maintenant quelques blocs pour définir l'apparence et la position de ton sprite.

![Le sprite "Forme".](images/shape_sprite.png)

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

Pour le moment, tes `Mes Blocs`{:class="block3myblocks"} n'ont pas été utilisés, il n'y aura donc aucun effet sur ton motif. Ajoute du code à `configuration`{:class="block3myblocks"}, pour que le code s'exécute dès que le drapeau est cliqué.

![Le sprite "Forme".](images/shape_sprite.png)

```blocks3
when flag clicked
+ setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
```

--- /task ---

--- task ---

**Teste** ton code en cliquant sur le drapeau et en observant le motif qui a été dessiné. Modifie ensuite les valeurs des paramètres jusqu'à ce que tu obtiennes un motif qui te plaît.

--- /task ---

--- task ---

Le sprite (pas ses clones) est toujours visible ; il peut être caché à la fin, mais devra être montré au début.

![Le sprite "Forme".](images/shape_sprite.png)

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
