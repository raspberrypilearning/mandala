
--- question ---

---
legend: Question 2 sur 2
---

Dans ton projet, tu as utilisé l'opérateur d'addition « + » pour modifier les costumes en fonction d'une entrée « Mes Blocs ».

Si nous avons ces costumes :

![Images de tous les costumes : costume 1 est un pétale transparent ; costume 2 est un pétale violet ; costume 3 est un globe transparent et le costume 4 est un globe violet.](images/costumes_quiz.png)

Lequel des blocs de code suivants permettrait à ton motif de passer du pétale violet au globe violet ?

--- choices ---

- (x)

 ```blocks3
 when flag clicked
 switch costume to ((costume [number v]) + (2))
 ```

  --- feedback ---

Oui, le numéro du costume sur lequel tu es est le costume 2 et le costume sur lequel tu veux passer est le costume 4. Tu devras donc passer au costume 2 + 2 = 4.

  --- /feedback ---

- ( )


 ```blocks3
 when flag clicked
 switch costume to ((costume [number v]) + (1))
 ```

  --- feedback ---

Cela passera du costume 2 au costume 2 + 1 = 3. Le costume 3 est le globe transparent et non le globe violet.

  --- /feedback ---

- ( )


 ```blocks3
 when flag clicked
 switch costume to ((costume [number v]) - (1))
 ```

  --- feedback ---

Cela passera du costume 2 au costume 2 - 1 = 1. Le costume 1 est le pétale transparent, pas le globe violet.

  --- /feedback ---

- ( )

 ```blocks3
 when flag clicked
 switch costume to ((1)+(1))
 ```

  --- feedback ---

Cela fera passer le costume à `costume 2`{:class='block3looks'} quel que soit le costume actuellement affiché.

  --- /feedback ---

--- /choices ---

--- /question ---
