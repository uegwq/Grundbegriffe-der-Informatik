TARGET

22 Allgemeiner Aufbau des Prozessors
---
Register
Rechenwerk: **ALU** / arithmetic logic unit. Dieser hat verschiedene Funktionen aber kann auf die Register zugreifen, sie lesen, sie verarbeiten und darauf wieder speichern.
Steuerwerk: 
- **IR** Instruction Register (Dort wird der aktuelle Befehl gespeichert, damit der Prozessor weiß was getan werden soll)
- **IAR** Instruction Address Register (Dort wird geschrieben wo wir in unserer Befehlsausführungskette gerade sind, dort steht die Adresse vom Speicher von der nächsten zu lesenden Funktion)
Speicherwerk: (Naja noch nicht so ganz verstasnden, ist das Speicherwert wie die Funktion die einer Adresse einen Wert zuweist?)
* **SAR** Storage address register (Über welche Adresse rede ich gerade)
* **SDR** Storage data register (Was steht am Wert von der Adresse)
Datenbus:
* Erlaubt Kommunikation zwischen den einzelnen Einheiten die Oben genannt wurden. Sonst bräuchte man O(n^2) viele Datenlinien zwischen den Einheiten also machen wir eine Busverbindung mit einer Linie und jeder hängt da dran.
<!--ID: 1707306987540-->

[[Turingmaschine]]