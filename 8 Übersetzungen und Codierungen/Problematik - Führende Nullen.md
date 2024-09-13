TARGET DECK
Grundbegriffe der Informatik

8 Führende Nullen Problematik
---
In der Funktion Num_k(w) besteht das Problem, dass führende Nullen gelöscht werden. Um das zu umgehen kann man diese wieder hinzufügen :). Es ist wichtig sich die Problematik der löschung der Führenden Nullen im Kopf zu haben weil man sonst bisschen blundern kann in der Klausur :(
Bsp:
$\text{bin}_\ell : \mathbb{Z}_{2^\ell} \rightarrow \{0,1\}^\ell$
$\text{bin}_\ell(n) = 0^{\ell - |\text{Repr}_2(n)|} \text{Repr}_2(n)$
Da fügen wir l minus Länge von der Reprä. nullen hinzu. Unser output wort ist also immer so lang wie es stellen gibt: hier sind es l stellen
<!--ID: 1706969472116-->

[[K-äre Darstellung bzw K-Äre Repräsentation]]
[[num(x) Dezimaldarstellung von Zahlen]]