# Come è stato prodotto SKOrganizer 2

SKOrganizer 2 è un progetto ideato e diretto da **Pastoris Marco Vincenzo**. L'autore ha definito l'obiettivo del prodotto, scelto i comportamenti da mantenere o eliminare, orchestrato il lavoro con strumenti di intelligenza artificiale, valutato le proposte, richiesto correzioni e deciso quali risultati sottoporre a prova e distribuire.

Gli strumenti AI hanno contribuito alla scrittura e revisione di codice, test e documentazione durante uno sviluppo iterativo. La supervisione e le decisioni di prodotto e di rilascio sono rimaste all'autore. Questa descrizione riguarda **il processo di sviluppo**: la versione 2.0 distribuita non include funzioni AI né richiede un servizio AI per organizzare i file.

## Dal prototipo al pacchetto Windows

Secondo l'autore, SKOrganizer 1.0 era costituito da un unico file ed è disponibile su [Microsoft Store](https://apps.microsoft.com/detail/9njsg8vsvcf8?hl=it-IT&gl=IT). Per la 2.0 il codice è stato suddiviso in moduli e sono stati sviluppati e verificati flussi più controllabili per anteprima, applicazione delle operazioni, tracciamento e recupero. Le funzioni di organizzazione e monitoraggio esistevano già nel percorso precedente: la [cronologia delle modifiche](CHANGELOG.md) distingue i miglioramenti dalle funzioni preesistenti.

Il pacchetto Windows x64 è stato costruito con **Python 3.13.13**, **Qt/PySide6 6.11.3**, **PyInstaller 6.22.3** e **NSIS 3.13**. Python e Qt sono inclusi nell'installer; Microsoft Visual C++ v14 Redistributable x64 è un prerequisito separato. L'installer contiene le licenze, gli avvisi e gli archivi pubblici dei sorgenti Qt/PySide6/shiboken6 nella cartella `LEGAL`.

## Verifica del candidato 2.0

Il candidato Windows identificato da SHA-256 `af3a6633cb6be18babf5d59a8cf512dcc9fa51bffe0467d1a7c713f2c3e9607e` è stato ricompilato due volte: le due copie del programma risultano identiche sui 125 file del pacchetto. Nel ciclo reale su Windows 11 x64 sono stati verificati installazione dei 125 file, avvio dell'app, schermata Informazioni con il nome dell'autore, chiusura e disinstallazione. La rimozione ha eliminato i 125 file e i quattro elementi di installazione controllati, senza lasciare la voce di disinstallazione nel registro.

La suite completa precedente aveva superato 1.681 test; nella build attuale l'unica modifica al codice dell'applicazione rispetto a quel pacchetto è il testo della schermata Informazioni, verificato separatamente. La prova su un Windows appena installato non è stata eseguita. Il pacchetto non è firmato digitalmente: Windows non dispone di un editore verificato per l'installer.

## Cosa contiene questo repository

Questo repository raccoglie la presentazione, le istruzioni e i testi documentali della versione 2.0. **Non è il repository dei sorgenti dell'applicazione** e non contiene la ricetta completa per ricostruire l'eseguibile. L'applicazione originale ha i propri [termini d'uso](LEGAL/SKORGANIZER_TERMS.txt); le librerie di terze parti mantengono le proprie licenze. Gli archivi automatici «Source code» generati da GitHub contengono i file di questo repository, non i sorgenti dell'app o i sorgenti corrispondenti alle librerie incluse nell'installer. Per i materiali delle librerie consultare la cartella `LEGAL` installata e [licenze e sorgenti](LICENSE_AND_SOURCES.md).
