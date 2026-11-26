# Termini, licenze e sorgenti delle librerie

SKOrganizer 2 è un'applicazione **proprietaria utilizzabile gratuitamente**. I [termini completi dell'applicazione](LEGAL/SKORGANIZER_TERMS.txt), inclusi anche nell'installer, consentono l'uso personale, didattico e aziendale senza costo e la condivisione gratuita del pacchetto ufficiale completo e non modificato. Non concedono una licenza open source per il codice originale dell'applicazione.

L'app usa componenti separati con licenze proprie. Qt 6.11.3, PySide6-Essentials 6.11.3 e shiboken6 6.11.3 sono distribuiti sotto **LGPLv3**; Python e gli altri componenti seguono i rispettivi termini. I diritti sulle librerie LGPL, compresa la possibilità di studiarle, modificarle e sostituirle con versioni compatibili, non sono limitati dai termini dell'app.

La cartella `LEGAL` contenuta nell'installer comprende:

- i testi di licenza e gli avvisi dei componenti;
- le istruzioni per sostituire le librerie LGPL accanto all'eseguibile;
- gli archivi ufficiali dei sorgenti `qtbase`, `qtsvg`, `qtimageformats` e `pyside-setup` della versione 6.11.3, con dimensioni, impronte SHA-256 e indirizzi ufficiali nell'[elenco degli archivi](LEGAL/SOURCE_ARCHIVES.txt).

I file delle librerie Qt/PySide/shiboken6 presenti nel pacchetto sono stati confrontati con i wheel Windows ufficiali 6.11.3. Il confronto dei tree dei sorgenti pubblici con gli elementi CI esaminati sostiene la corrispondenza del codice esaminato; le informazioni pubbliche non identificano esplicitamente ogni wheel distribuito come prodotto di quel preciso lavoro CI né attestano ogni opzione di build. Il 23 novembre 2026 il titolare ha chiesto chiarimenti al team Qt; alla preparazione di questa documentazione non risultava una risposta. L'eventuale risposta sarà valutata per aggiornare il materiale fornito. La richiesta non è un'approvazione di Qt.

Microsoft Visual C++ v14 Redistributable **x64** è un prerequisito da installare separatamente dalla [pagina ufficiale Microsoft](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist/); non è incluso nell'installer.

Questo repository ospita documentazione e il collegamento all'installer come asset di Release. Gli archivi automatici **Source code** generati da GitHub contengono soltanto i file del repository: non sono il codice sorgente dell'applicazione e non sostituiscono gli archivi Qt/PySide presenti nell'installer. Per i dettagli completi e giuridicamente rilevanti valgono i testi distribuiti nella cartella `LEGAL` dell'esatto installer scaricato.
