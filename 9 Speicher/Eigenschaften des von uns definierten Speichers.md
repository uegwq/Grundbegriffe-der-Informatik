TARGET DECK
Grundbegriffe der Informatik

9 Eigenschaften des von uns definierten Speichers
---
Er ist konsistent: Das heißt wenn wir einen Wert an eine Adresse schreiben und danach den Speicher an dieser Adresse auslesen kriegen wir den Wert den wir geschrieben haben.
Er ist unabhängig: Das schreiben von einem Wert an einer Adresse ändert nichts an den Werten bei anderen Adressen. Formaler:
($m$ ist die Speicherfunktion/Tabelle, $a$ ist die Adresse, $v$ ist ein Wert)
$memread(memwrite(m,a,v),a) = v$
$memread(memwrite(m,a′,v′),a) = memread(m,a)$
<!--ID: 1707066807974-->

[[Schreibfunktion eines Speichers]]
[[Auslesefunktion eines Speichers]]