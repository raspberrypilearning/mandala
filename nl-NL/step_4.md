## Stel je sprite in

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Stel je sprite in om je mandala te resetten.
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

Op dit moment lijken je mandala-patronen elke keer te veranderen, afhankelijk van de parameterwaarden die je gebruikt. Vervolgens maak je nieuwe `mijn blokken`{:class="block3myblocks"}, zodat je **mandala** sprite altijd op dezelfde manier begint.

--- task ---

Gebruik het menu `Mijn blokken`{:class="block3myblocks"} om een nieuw blok te maken met de naam `instellen`{:class="block3myblocks"}. Het blok zou vier parameters moeten hebben: `afmeting`{:class="block3myblocks"}, `transparant`{:class="block3myblocks"}, `y`{:class="block3myblocks"} en `beweeg`{:class="block3myblocks"}. Maak je geen zorgen, je kunt deze wijzigen of later meer toevoegen.

![De vorm sprite.](images/shape_sprite.png)

```blocks3
define instellen: grootte (grootte) transparant (transparant) y (y) beweeg (beweeg)
```

--- /task ---

Wanneer je de mandala in de volgende stap kleurrijk maakt, zal het `transparant`{:class="block3myblocks"} blok de kleuren transparant maken, dus wanneer de vormen elkaar overlappen, krijg je een kleurmengeffect.

--- task ---

Voeg nu een paar blokken toe om het uiterlijk en de positie van je sprite in te stellen.

![De vorm sprite.](images/shape_sprite.png)

```blocks3
define instellen: grootte (grootte) transparant (transparant) y (y) beweeg (beweeg)
+ set size to (grootte) %
+ set [ghost v] effect to (transparant)
+ go to x: (0) y: (0)
+ point in direction (90)
+ change y by (y)
+ move (beweeg) steps
```

--- /task ---

--- task ---

Op dit moment wordt je `mijn blokken`{:class="block3myblocks"} niet gebruikt, dus zal er geen effect op je patroon zijn. Voeg code toe aan `instellen`{:class="block3myblocks"}, zodat de code wordt uitgevoerd zodra op de vlag wordt geklikt.

![De vorm sprite.](images/shape_sprite.png)

```blocks3
when flag clicked
+ instellen: grootte (60) transparant (50) y (10) beweeg (10) ::custom
patroon: herhaal (3) grootte (10) beweeg (5) draai (60) ::custom
patroon: herhaal (5) grootte (10) beweeg (45) draai (30) ::custom
patroon: herhaal (6) grootte (10) beweeg (90) draai (30) ::custom
```

--- /task ---

--- task ---

**Test** je code door op de vlag te klikken en het patroon te bekijken dat is getekend. Wijzig vervolgens de waarden van de parameters totdat je een patroon hebt dat je leuk vindt.

--- /task ---

--- task ---

De sprite (niet de klonen) is nog steeds zichtbaar; hij kan aan het einde verborgen worden, maar moet aan het begin getoond worden.

![De vorm sprite.](images/shape_sprite.png)

```blocks3
when flag clicked
+ show
instellen: grootte (60) transparant (50) y (10) beweeg (10) ::custom
patroon: herhaal (3) grootte (10) beweeg (5) draai (60) ::custom
patroon: herhaal (5) grootte (10) beweeg (45) draai (30) ::custom
patroon: herhaal (6) grootte (10) beweeg (90) draai (30) ::custom
+ hide
```

--- /task ---

--- save ---
