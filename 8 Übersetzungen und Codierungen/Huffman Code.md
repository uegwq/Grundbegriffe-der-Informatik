TARGET DECK
Grundbegriffe der Informatik

8 Huffman Code
---
Motivation: Einen präfixfreien Homomorphismus  konstruieren, sodass ein Wort w aus dem Alphabet $A$ möglichst komprimiert in Binärdarstellung dargestellt wird.
Wie geht das?
Wir bauen uns einen Baum. An den Blättern sind die Zeichen die im Wort w Vorkommen zusammen mit ihrer vorkommenszahl notiert. Initial nenne ich diese Zeichen elementare Wörter.
Man verbindet nun iterativ sozusagen die zwei elemenate Wörter, die die geringste Vorkommenszahl haben über einen neuen Knoten. Der Knoten trägt den Namen der konkatenation der Wörter und hat als Wert die Summe der Vorkommenszahlen.
Man wiederholt das mit dem neunen Knoten als neues Elementares Wort.
Dann baut man es auf und wenn man wissen will was die Repräsentation eines Zeichens in der Huffman Codierung von dem Wort w ist, dann geht man den Baum runter und merkt sich was man liest.
<!--ID: 1706987688305-->

[[Gerichteter Graph]]
[[Präfixfreier Homomorphismus]]
[[Codierung]]