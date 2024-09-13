TARGET DECK
Grundbegriffe der Informatik

8 Zweierkomplement von Binärzahlen
---
Ist so definiert: Für positive Zahlen schrieben wir die Zahl auf und setzten vorne eine 0 dran. Für negative Zahlen setzten wir vorne eine 1 dran und berechnen die Binärdarstellung mit führenden nullen von der negativen Zahl x + 2^(l-1). Dies hat einen Vorteil und einen Nachteil in meiner Sicht:
Der Vorteil ist, dass negative Zahlen im Zweierkomplement gut binär addierbar sind, wenn man den Überhang entfernt.
Der Nachteil ist, dass man negative Zahlen nicht so ganz einfach lesen kann.
Definition vom Zweierkomplement:
$Zkpl_{\ell}(x) = \begin{cases} 0\text{bin}_{\ell-1}(x) & \text{if } x \geq 0 \\ 1\text{bin}_{\ell-1}\left(2^{\ell-1} + x\right) & \text{if } x < 0 \end{cases}$
<!--ID: 1706970496006-->

[[Problematik - Führende Nullen]]