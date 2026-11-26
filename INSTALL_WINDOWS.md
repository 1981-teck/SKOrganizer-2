# Installazione su Windows

Queste istruzioni si riferiscono a **SKOrganizer 2.0 per Windows x64**. Il pacchetto è stato collaudato su Windows 11 x64 con processore Intel/AMD. Windows a 32 bit e ARM non sono supportati; altre versioni Windows non sono state qualificate.

## Prima di iniziare

1. Installa la versione x64 più recente supportata di [Microsoft Visual C++ v14 Redistributable](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist/). È un prerequisito esterno: l'installer SKOrganizer non lo include e segnala le librerie mancanti.
2. Scarica `SKOrganizer2-2.0-win-x64.exe` dagli **asset della Release 2.0** di questo repository, quando disponibili. Installa il programma e gestisci i file su un disco locale fisso; unità rimovibili e condivisioni di rete non sono supportate.
3. Controlla l'impronta del file scaricato. In PowerShell, nella cartella che lo contiene, esegui:

   ```powershell
   (Get-FileHash -LiteralPath .\SKOrganizer2-2.0-win-x64.exe -Algorithm SHA256).Hash
   ```

   Per il candidato 2.0 collaudato deve risultare `af3a6633cb6be18babf5d59a8cf512dcc9fa51bffe0467d1a7c713f2c3e9607e`. Se la Release pubblica indica un'impronta diversa, usa quella riportata accanto al suo asset e verifica che i due valori coincidano. Non avviare un file con impronta inattesa.

## Installazione e primo utilizzo

1. Avvia l'installer, leggi i termini e scegli una cartella nel tuo profilo su disco locale fisso. Il collegamento sul Desktop è facoltativo.
2. Apri **SKOrganizer 2** dal menu Start.
3. Aggiungi una piccola cartella di prova e controlla categorie e regole. Usa **Preview** per vedere le destinazioni; **Apply** richiede una conferma separata. Per i tipi sconosciuti puoi scegliere una categoria in Preview e, se vuoi, salvare una regola per l'estensione.
4. Se necessario usa **Undo** finché è disponibile. La cartella `.skorganizer-transactions`, con file come `journal.json` e `origin.json`, serve alla tracciabilità e al recupero: non eliminarla manualmente.
5. Usa **Organize All** e **Monitoring** dopo avere controllato regole e cartelle: queste modalità non chiedono la conferma di Preview per ogni spostamento.

Python 3.13.13 e Qt/PySide6 6.11.3 sono compresi nel pacchetto e non vanno installati a parte.

## Problemi e rimozione

Se l'installer segnala DLL Visual C++ x64 mancanti, installa o ripara il [pacchetto ufficiale Microsoft](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist/) e riprova. Evita DLL scaricate singolarmente da siti non ufficiali. Se Windows indica un editore non verificato, controlla provenienza e SHA-256: questo installer non ha una firma digitale.

Per disinstallare, chiudi l'app e usa **Impostazioni → App → App installate → SKOrganizer 2 → Disinstalla**. Il programma rimuove i propri file, collegamenti e voce di installazione; i file che hai organizzato restano nelle tue cartelle.

Il ciclo di installazione, avvio e disinstallazione del candidato 2.0 è stato completato su Windows 11 x64. Non è stata effettuata una prova su Windows appena installato.
