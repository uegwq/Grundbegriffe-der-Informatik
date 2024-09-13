TARGET DECK
Grundbegriffe der Informatik

18 Ausgabeauswertungsfunktion eines Endlichen Automatens
---
Als info: ein Stern soll bedeuten, dass ein zweites Argument nicht nur ein einzelnes Symbol ist, sondern ein ganzes Wort.
Zwei Sterne soll bedeuten, dass wir uns nicht für einen Funktionswert interessieren, sondern für ein ganzes Wort von Funktionswerten.
$g_*(z, \varepsilon) = \varepsilon$
$\forall w \in X^* : \forall x \in X : g_*(z, wx) = g(f_*(z,w),x)$
-
$g_{**}(z, \varepsilon) = \varepsilon$
$\forall w \in X^* : \forall x \in X : g_{**}(z, wx) = g_{**}(z,w) \cdot g^*(z,wx)$
<!--ID: 1707321823792-->

[[Abbildung]]
