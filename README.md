# SKOrganizer 2

**Versione 2.0 per Windows x64.** SKOrganizer organizza file in cartelle locali secondo categorie e regole configurate dall'utente. Consente di esaminare una proposta in **Preview** prima di applicarla, usare **Organize All** e **Monitoring** e, quando disponibile, ripristinare un'operazione con **Undo**. Questa versione non usa funzioni di intelligenza artificiale durante l'esecuzione.

Il progetto è ideato e diretto da **Pastoris Marco Vincenzo**. Lo sviluppo della 2.0 è stato svolto da lui orchestrando strumenti di AI per analisi, implementazione, verifiche e documentazione. Le decisioni sul prodotto e il collaudo finale sono rimasti sotto il suo controllo. Leggi [il ruolo dell'autore](AUTHORSHIP.md) e [come è stato prodotto il programma](COME_E_STATO_PRODOTTO.md).

La [pagina di presentazione](docs/index.html) è disponibile nei file del repository.

## Scaricare e installare

L'installer `SKOrganizer2-2.0-win-x64.exe` si trova negli **asset della [sezione Releases](https://github.com/1981-teck/SKOrganizer-2/releases)** di questo repository, non tra i file del codice Git. Prima dell'installazione servono Windows x64 su processore Intel/AMD, [Microsoft Visual C++ v14 Redistributable x64](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist/) installato separatamente e un disco locale fisso. Python 3.13.13 e Qt/PySide6 6.11.3 sono già inclusi nell'installer.

Leggi [installazione, controllo SHA-256 e primo utilizzo](INSTALL_WINDOWS.md). Il candidato 2.0 verificato ha SHA-256:

```text
af3a6633cb6be18babf5d59a8cf512dcc9fa51bffe0467d1a7c713f2c3e9607e
```

Il ciclo di installazione, avvio e disinstallazione di questi byte è riuscito su Windows 11 x64. Non è stata eseguita una prova su Windows appena installato; Windows ARM e a 32 bit non sono supportati da questo pacchetto. L'installer non è firmato digitalmente, perciò Windows non mostra un editore verificato.

## Dalla versione 1.0 alla 2.0

La [versione 1.0 sul Microsoft Store](https://apps.microsoft.com/detail/9NJSG8VSVCF8) è il prodotto precedente. Secondo l'autore, la sua applicazione era concentrata in un unico file. La 2.0 è stata riorganizzata in moduli e ha ricevuto un lavoro di correzione e verifica della gestione dei file: Preview con conferma distinta, registrazione delle operazioni per Undo e recupero, e controlli più rigorosi sui conflitti. Le categorie, le regole e il monitoraggio avevano già precedenti nella storia del programma: non vengono presentati come invenzioni della 2.0. [Dettagli delle modifiche](CHANGELOG.md).

L'identificativo Microsoft Store `9NJSG8VSVCF8` è quello registrato nella documentazione del progetto dal titolare; la disponibilità della pagina può dipendere dal paese e dallo Store.

## Termini e sorgenti delle librerie

Il codice originale dell'applicazione è proprietario e il suo utilizzo è gratuito secondo i termini inclusi nell'installer. Qt, PySide6, shiboken6, Python e gli altri componenti conservano le rispettive licenze. La cartella `LEGAL` distribuita con l'app contiene testi, avvisi, istruzioni per sostituire le librerie LGPL e quattro archivi dei sorgenti pubblici Qt/PySide6 pertinenti al pacchetto. [Licenze e provenienza dei sorgenti](LICENSE_AND_SOURCES.md).

I pacchetti automatici **Source code** creati da GitHub contengono solo i file di questo repository; non sono i sorgenti dell'applicazione né quelli delle librerie incluse nell'installer.
