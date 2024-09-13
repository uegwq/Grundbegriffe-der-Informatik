TARGET DECK
Grundbegriffe der Informatik

8 Übersetzten
---
Was heißt es etwas zu übersetzten?
* Die Zuordnung von einem Wort aus einer Sprache zu einem Wort aus einer anderen Sprache
* Die Bedeutung der beiden Wörter bleibt jedoch gleich!
Man kann eine Übersetzung also auch als Funktion auffassen:
$\text{semA}: L_A \rightarrow \text{Sem}$ und $\text{semB}: L_B \rightarrow \text{Sem}$, wobei $L_A$ und $L_B$ jeweils zwei formale Sprachen sind.
Eine Abbildung $f : L_A \rightarrow L_B$ heißt Übersetzung bezüglich $sem_A$ und $sem_B$, wenn f die Bedeutung erhält. D.h. $\forall w \in L_A : \text{semA}(w) = \text{semB}(f(w))$
<!--ID: 1706965318850-->

[[Abbildung]]