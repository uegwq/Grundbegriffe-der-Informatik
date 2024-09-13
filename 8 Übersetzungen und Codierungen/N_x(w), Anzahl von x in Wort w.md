TARGET DECK
Grundbegriffe der Informatik

8 N_x(w), Anzahl von x in Wort w
---
$N_x : A^* \rightarrow \mathbb{N}_0$
$N_x(\varepsilon) = 0,$
$\forall y \in A, \forall w \in A^* : N_x(yw) = \begin{cases} 1 + N_x(w) & \text{if } y = x \\ N_x(w) & \text{otherwise} \end{cases}$
Aka Zählt rekursiv eins hoch für jedes mal wenn es x sieht.
<!--ID: 1706979826099-->


[[Wort aus einem Alphabet A]]
[[Abbildung]]