TARGET DECK
Grundbegriffe der Informatik

18 Zustandsuswertungsfunktionen eines endlichen Automaten
---
Als info: ein Stern soll bedeuten, dass ein zweites Argument nicht nur ein einzelnes Symbol ist, sondern ein ganzes Wort.
Zwei Sterne soll bedeuten, dass wir uns nicht für einen Funktionswert interessieren, sondern für ein ganzes Wort von Funktionswerten.
$f_*(z, \varepsilon) = z$ 
$\forall w \in X^* : \forall x \in X : f_*(z, wx) = f(f_*(z, w), x)$
zudem:
$f_{**}(z, \varepsilon) = z$
$\forall w \in X^* : \forall x \in X : f_{**}(z, wx) = f_{**}(z,w) \cdot f_*(z,wx)$
<!--ID: 1707321587557-->

[[Mealy-Automat]]
[[Moore-Automaten]]