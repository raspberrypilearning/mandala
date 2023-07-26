## Ρύθμισε το αντικείμενό σου

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Ρύθμισε το αντικείμενό σου για να επαναφέρεις το μάνταλά σου.
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

Προς το παρόν, τα μάνταλα μοτίβα σου μπορεί να φαίνεται να αλλάζουν κάθε φορά, ανάλογα με τις τιμές των παραμέτρων που χρησιμοποιείς. Στη συνέχεια, θα δημιουργήσεις τη νέα `"εντολή μου"`{:class="block3myblocks"}, έτσι ώστε το αντικείμενο **μάνταλά** σου να ξεκινά πάντα στην ίδια κατάσταση.

--- task ---

Χρησιμοποίησε το μενού `Οι εντολές μου`{:class="block3myblocks"} για να δημιουργήσεις ένα νέο μπλοκ που ονομάζεται `ρύθμιση`{:class="block3myblocks"}. Η εντολή πρέπει να έχει τέσσερις παραμέτρους: `μέγεθος`{:class="block3myblocks"}, `φάντασμα`{:class="block3myblocks"}, `y`{:class="block3myblocks"}, και `κίνηση`{:class="block3myblocks"}. Μην ανησυχείς, μπορείς να τις αλλάξεις ή να προσθέσεις περισσότερες αργότερα.

![Το αντικείμενο σχήματος.](images/shape_sprite.png)

```blocks3
define setup: size (size) ghost (ghost) y (y) move (move)
```

--- /task ---

Όταν χρωματίσεις το μάνταλα στο επόμενο βήμα, το μπλοκ `φάντασμα`{:class="block3myblocks"} θα κάνει τα χρώματα διαφανή έτσι όταν τα σχήματα επικαλύπτονται, θα αποκτήσεις ένα εφέ ανάμιξης χρωμάτων.

--- task ---

Τώρα πρόσθεσε μερικά μπλοκ για να ορίσεις την εμφάνιση και τη θέση του αντικειμένου σου.

![Το αντικείμενο σχήματος.](images/shape_sprite.png)

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

Προς το παρόν, η `"εντολή μου"`{:class="block3myblocks"} δεν έχει χρησιμοποιηθεί, οπότε δεν θα υπάρξει καμία επίδραση στο μοτίβο σου. Πρόσθεσε κώδικα στην `ρύθμιση`{:class="block3myblocks"}, ώστε ο κώδικας να εκτελεστεί μόλις πατηθεί η σημαία.

![Το αντικείμενο σχήματος.](images/shape_sprite.png)

```blocks3
when flag clicked
+ setup: size (60) ghost (50) y (10) move (10) ::custom
pattern: repeat (3) size (10) move (5) turn (60) ::custom
pattern: repeat (5) size (10) move (45) turn (30) ::custom
pattern: repeat (6) size (10) move (90) turn (30) ::custom
```

--- /task ---

--- task ---

**Δοκίμασε** τον κώδικά σου κάνοντας κλικ στη σημαία και παρατηρώντας το μοτίβο που σχεδιάστηκε. Στη συνέχεια, άλλαξε τις τιμές των παραμέτρων μέχρι να έχεις ένα μοτίβο που σου αρέσει.

--- /task ---

--- task ---

Το αντικείμενο (όχι οι κλώνοι του) είναι ακόμα ορατό, μπορεί να κρυφτεί στο τέλος, αλλά θα πρέπει να εμφανιστεί στην αρχή.

![Το αντικείμενο σχήματος.](images/shape_sprite.png)

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
