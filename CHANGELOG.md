# Modifiche fra SKOrganizer 1.0 e 2.0

## Versione 2.0 — 2026

La 2.0 prosegue il progetto [SKOrganizer 1.0 pubblicato sul Microsoft Store](https://apps.microsoft.com/detail/9NJSG8VSVCF8). Secondo l'autore, l'applicazione 1.0 era concentrata in un unico file. La 2.0 usa moduli distinti per interfaccia, regole, organizzazione e gestione delle operazioni.

- **Controllo prima dello spostamento:** Preview mostra la proposta e Apply richiede una conferma distinta. Organize All e Monitoring restano disponibili per le regole già impostate.
- **Undo e recupero:** le operazioni usano un journal e informazioni sull'origine per verificare e ripristinare gli spostamenti quando possibile. Il trattamento dei conflitti è stato corretto e rafforzato: Skip lascia i file al loro posto; un ripristino dopo sostituzione considera anche il file che occupava la destinazione.
- **Semplificazione del prodotto:** le funzioni AI sperimentate durante lo sviluppo sono state abbandonate nel programma distribuito. La classificazione della 2.0 usa categorie e regole deterministiche; un tipo sconosciuto può essere assegnato manualmente in Preview.
- **Distribuzione Windows:** installer per Windows x64 con Python 3.13.13, Qt/PySide6 6.11.3, icona SK2, testi di licenza, avvisi e archivi dei sorgenti pubblici delle librerie Qt pertinenti. Microsoft Visual C++ v14 x64 va installato separatamente.
- **Verifica:** il candidato 2.0 è stato installato, avviato e disinstallato su Windows 11 x64; tutti i 125 file installati sono stati confrontati con il manifest. La disinstallazione ha rimosso i 125 file e i collegamenti previsti. Non è stata eseguita una prova su Windows appena installato.

Le modalità per estensione, ordine alfabetico, data, regole personalizzate, il monitoraggio e una forma precedente di Undo compaiono già nel materiale storico. Questa nota non le presenta come funzioni nate con la 2.0: il lavoro ha mirato a renderne il comportamento più coerente e verificabile.

## Versione 1.0

La versione precedente è identificata sul Microsoft Store dal Product ID `9NJSG8VSVCF8`, registrato nella documentazione del progetto dal titolare. Questa pagina descrive il passaggio alla 2.0; per la disponibilità e le caratteristiche commerciali della 1.0 fa fede la sua pagina Store.
