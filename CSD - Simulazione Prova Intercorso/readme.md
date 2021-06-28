# Esercizio su Driver

Un sistema è composto da 3 unità A, B e C. B è collegato ad A mediante una periferica seriale, e a C mediante una periferica parallela. Il sistema opera come segue:
A invia fino ad un massimo di M messaggi di N byte a B. Per ogni messaggio ricevuto MSGi, B verifica l’ultimo byte del messaggio MSGi(N-1):
• Se è diverso da 0, B continua con la ricezione;
• Se è uguale a 0, B interrompe la comunicazione con A e C.
Durante la ricezione dei messaggi (in qualsiasi momento), il sistema B può ricevere dei caratteri da C. In particolare, se riceve 2 caratteri (qualsiasi) successivi da C, B termina la ricezione del messaggio eventualmente in sospeso e poi interrompe la comunicazione con A e C.

LINGUAGGIO: assembly Motorola M68000.

NOTA: I due messaggi ricevuti da C non devono essere consecutivi, ma si considerano due messaggi in totale.