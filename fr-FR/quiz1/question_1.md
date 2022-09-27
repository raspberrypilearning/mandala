## Questionnaire rapide

Répond aux deux questions. Il y a des indices pour te guider vers la bonne réponse.

Lorsque tu as répondu à chaque question, clique sur **Vérifier ma réponse**.

Amuse-toi bien !

--- question ---

---
legend: Question 1 sur 2
---

Dans ton projet, tu as utilisé des clones pour créer des motifs. Regarde la définition suivante de `Mes Blocs`{:class='block3myblocks'} :

```blocks3
define pattern (repeat) (size) (move) (turn)
repeat (repeat)
change size by (size)
move (move) steps
turn cw (turn) degrees
create clone of (myself v)
```

Voici un motif qui a été créé. ![quatre pétales sont également espacés, tous à partir du même centre. Chaque pétale augmente sa taille.](images/quiz_1.png)

Lequel des appels suivants créerait le motif ci-dessus ?

--- choices ---

- ( )
```blocks3
when flag clicked
pattern (3) (10) (0) (90)::custom
```
  --- feedback ---

Cela ne créerait que trois clones, et il y en a quatre dans l'image.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
pattern (4) (10) (100) (90)::custom
```

  --- feedback ---

Cela ferait bouger le clone de `100` pas, mais tous les clones dans l'image ont les mêmes coordonnées `x` et `y`.

  --- /feedback ---

- (x)

```blocks3
when flag clicked
pattern (4) (10) (0) (90)::custom
```

  --- feedback ---

Oui, ce code crée 4 pétales dont la taille augmente de 10. Chaque pétale a tourné de 90 degrés.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
pattern (4) (10) (0) (360)::custom
```

  --- feedback ---

Les clones feraient ainsi un cercle complet, et tu ne pourrais voir qu'un seul grand clone.

  --- /feedback ---

--- /choices ---

--- /question ---
