

Wie arbeitet das Seuerwerk?:
Es gibt verschiedene Typen von Befehlen, undzwar Transport von Daten, Verarbeitung von Daten und Beeinflussung der Befehlsreihenfolge.
Wie werden diese Befehle notiert?
Naja wie gesagt, 4 Bit befehl und 20 Bit Wert. Davon kann man aber Abstrahieren:
z.B. 001000000000000000101010
Das ist kompliziert aber eigentlich ist das ja nur:
10 Entspricht STV (Store Value at Adress) Befehl
101010 Wert (= 42)
-
Es gibt noch:
LDC const (load constant). Schreibt eine constante const auf den Akkumulator
LDV adr (load value from): Schreibt den Wert von einer Adresse adr auf den Akkumulator
STV adr (Store Value at Adress) schreibt den Wert des Akkumulator auf eine Adresse adr
-
![[Pasted image 20240207103709.png]]
Coolere Befehle:
LDIV ard (load value indirect from address) wir gehen an eine Adresse adr, da schauen wir was steht. Dann gehen wir an die Adresse von dem Wert der an adr steht und gehen dort hin. Es werden von den 24 bit speicher nur die niedrigwertigsten stellen verwendet.
Z.b. bei 46 steht "10", bei 10 steht "42". LDIV 46 schreibt 42 in den Akkumulator.
STIV adr
-
Logische Befehle:
ADD adr wir schreiben auf den Akkumulator $Akku + M(adr)$. (Mit zweierkomplement!)
AND adr (Akkumulatorwert AND adr und dies stellenweise je! Das Ergebnis schreiben wir in den Akkumulator. Analog zu OR und XOR.)
OR adr
XOR adr
NOT (Invertierung de Akku bits)
RAR (Rorate accumulator right) wir machen wie so einen shift. Alle die sozusagen rausfallen von unserem Tisch werden links wieder eingeführt.
EQL adr (equal?) Wenn die Werte gleich sind schreiben wir 111111111111111111111111 auf den Akkumulator, sonst schreiben wir 000000000000000000000000.
-
Krasser Befehl um zu jumpen für schleife mit if:
JMP adr (Jump) setze fort mit Befehl in Adresse adr.
JMN adr (Jump if negative). Springt zu Adresse adr, wenn der Speicher im Akkumulator negativ ist. (Also wenn das 24. Bit eine 1 sind.)
HALT (Okay danke Maschine, das wars wir müssen jetzt nicht mehr weiter machen)

[[Programm in einer Mima]]