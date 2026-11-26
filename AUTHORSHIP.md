# Come è stato realizzato SKOrganizer 2

**Pastoris Marco Vincenzo** ha ideato il progetto, stabilito gli obiettivi, scelto le funzioni da mantenere e quelle da eliminare, diretto le revisioni e svolto prove d'uso su Windows. Ha coordinato strumenti di intelligenza artificiale durante l'analisi del programma, la scrittura e revisione di codice, la preparazione dei test, dell'installer e della documentazione. Parti del lavoro tecnico e dei testi sono state quindi prodotte con assistenza AI; non sarebbero correttamente descritte come scritte interamente a mano.

Le decisioni di prodotto sono state umane. In particolare, dopo aver valutato l'effetto pratico delle funzioni AI, il titolare ha deciso di **non includerle nell'applicazione 2.0** e di concentrare il programma su regole, anteprima, organizzazione e recupero dei file. L'assistenza AI usata nello sviluppo non è una funzione eseguita dall'app distribuita.

Il lavoro è passato da analisi del codice esistente a modifiche in piccoli passaggi, prove automatiche, compilazioni indipendenti e collaudo dell'installer. Per il candidato 2.0 preparato sono stati controllati i 125 file installati; l'app è stata avviata e la sua disinstallazione è stata verificata sul PC di prova Windows 11 x64. Le prove hanno limiti documentati: non è stata eseguita una prova su Windows appena installato e l'installer non è firmato digitalmente.

I diritti del codice originale dell'applicazione appartengono a Pastoris Marco Vincenzo. I componenti di terzi, inclusi Qt, PySide6, shiboken6 e Python, restano attribuiti ai rispettivi autori secondo le loro licenze. [Termini, licenze e sorgenti delle librerie](LICENSE_AND_SOURCES.md).
