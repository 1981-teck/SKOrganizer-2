# SKOrganizer 2 — v2.0.0

> Bozza privata delle note di Release. Verificare repository, pagina web e asset prima della pubblicazione.

SKOrganizer 2 organizza file e cartelle locali secondo categorie e regole configurate dall'utente. Offre **Preview** delle destinazioni, **Organize All**, **Monitoring** e **Undo** quando l'operazione lo consente. La versione visualizzata nell'app è **2.0**; `v2.0.0` è il tag previsto per questa Release.

## Dalla versione 1.0 alla 2.0

La [versione 1.0 è presente sul Microsoft Store](https://apps.microsoft.com/detail/9njsg8vsvcf8?hl=it-IT&gl=IT). Secondo l'autore, la prima implementazione era concentrata in un unico file. Per la 2.0 il programma è stato riorganizzato in moduli, sono stati ampliati i controlli sulle operazioni e sono stati preparati test, installer e documentazione delle dipendenze. Le funzioni elencate sopra descrivono la 2.0: non implicano che fossero tutte assenti nella 1.0. Questa Release GitHub è separata dalla versione distribuita tramite Microsoft Store.

SKOrganizer 2 è stato sviluppato con assistenza AI **sotto la direzione di Pastoris Marco Vincenzo**. Marco ha definito obiettivi e vincoli, orchestrato gli assistenti, valutato le scelte, guidato correzioni e verifiche e deciso il rilascio. Il programma distribuito **non usa funzioni AI**.

## Download e requisiti

L'asset Windows previsto per questa Release è `SKOrganizer2-2.0-win-x64.exe` (**105.205.944 byte**). Va allegato alla Release; non è un file del repository. La sua impronta SHA-256 verificata è:

```text
af3a6633cb6be18babf5d59a8cf512dcc9fa51bffe0467d1a7c713f2c3e9607e  SKOrganizer2-2.0-win-x64.exe
```

- **Sistema:** Windows x64 su processore Intel o AMD. È stato collaudato su Windows 11 x64; questo pacchetto non supporta Windows a 32 bit o ARM.
- **Prerequisito:** [Microsoft Visual C++ v14 Redistributable x64](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist/), da installare separatamente nella versione x64 supportata più recente. L'installer segnala se mancano le librerie richieste.
- **Percorsi:** installazione e cartelle gestite su disco locale fisso; unità rimovibili e condivisioni di rete sono fuori ambito.

Python 3.13.13 e Qt/PySide6 6.11.3 sono inclusi nell'installer. Per disinstallare, usare **Impostazioni → App → App installate → SKOrganizer 2 → Disinstalla**. I file organizzati dall'utente non vengono rimossi dalla disinstallazione.

## Verifiche e limiti

Il candidato identificato dall'impronta sopra ha superato un ciclo reale su Windows 11 x64: installazione e verifica dei **125 file**, avvio e chiusura dell'app, controllo della schermata Informazioni e disinstallazione. Il rapporto finale registra la rimozione dei **125 file**, dei collegamenti, della ricevuta, del disinstallatore e della voce di disinstallazione. Una prova separata ha verificato che il controllo di rimozione tollera un errore temporaneo di Windows ma segnala quello persistente.

Una prova su Windows appena installato **non è stata eseguita**. L'installer **non è firmato digitalmente**: Windows non dispone di un editore verificato per questo file. L'esito dei test descrive gli ambienti e i percorsi provati, senza costituire una certificazione generale.

## Licenze e sorgenti delle librerie

L'applicazione originale è distribuita senza costo secondo i propri [termini](https://github.com/1981-teck/SKOrganizer-2/blob/main/LEGAL/SKORGANIZER_TERMS.txt). Qt, PySide6, shiboken6 e gli altri componenti mantengono le rispettive licenze. L'installer include la cartella `LEGAL` con testi delle licenze, avvisi, archivi dei sorgenti pubblici Qt/PySide6/shiboken6 e istruzioni per sostituire le librerie LGPL compatibili. Il codice sorgente proprietario dell'app non è pubblicato in questo repository.

Il 23 novembre 2026 è stata inviata al team Qt una richiesta di chiarimenti sulla corrispondenza dei sorgenti pubblici con i wheel Windows usati. Alla data di questa bozza non è pervenuta una risposta; la richiesta non equivale a un'approvazione di Qt.
