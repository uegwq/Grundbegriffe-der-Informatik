
Durchführung de Befehle in drei Phasen:
+ Holphase (holen eines Befehls und gleichzeitige Berechnung des nächsten Befehls)
1. Holens der Wertes vom Speicher (SAR verarbetiet den Werd, SDR outputter ihn.)
2. IAR Addiert im ALU 1 zum Aktuellen Adressenwert. 
3. Der output wird dann im IAR gespeichert. Das ist dann die Adresse des nächstens Befehls.
-> In der Realität passieren Schritte 1,2,3 aber simultan und getaktet. Bisschen wie bei einem 4 Takter Motot (Belüftungsphase, keine Ahnung Phase aber getaktet.)
+ Decodierphase
1. Das Steuerwerk liest die obersten 4 bits des aktuellen Befehls um zu wissen welcher befehl ausgeführt werden soll, und für den Jump if Negative Befehl soll dann der höchste Bit des Akkumulators gelesen werden.
+ Ausführungsphase
-> Abhängig vom zu Ausführenden Befehl
Es gibt dann da eine Tabelle, die je nach Befehlsbit die Befehle in die Leitungen führt und koodiniert wo was wie hinfließt. Das ist dann letzendlich auch ein endlicher Automat.

[[Wie läuft das ab mit den Befehlen]]