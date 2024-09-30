# Risoluzione dei problemi

Questa pagina offre consigli per la risoluzione di problemi comuni. Se non riesci a risolvere il tuo problema con i consigli su questa pagina, entra nel [canale Discord di Nintendo Homebrew](https://discord. g/MWxPgEp) e descrivi il tuo problema, indicando quello che hai già provato.

:::details Indice

Utilizzato su più pagine:

- [SafeB9SInstaller](#issues-with-safeb9sinstaller)

Pagine guida:

- [Installazione di boot9strap (Soundhax)](#installing-boot9strap-soundhax)
- [Installazione di boot9strap (MSET9)](#installing-boot9strap-mset9)
- [Installazione di boot9strap (SSLoth-Browser)](#installing-boot9strap-ssloth-browser)
- [Installazione di boot9strap (super-skaterhax)](#installing-boot9strap-super-skaterhax)
- [Completamento dell'installazione](#finalizing-setup)

Problemi dopo l’installazione:

- [Problemi di avvio](#boot-issues-on-consoles-with-custom-firmware)
- [Problemi software](#software-issues-on-consoles-with-custom-firmware)

:::

## Problemi con SafeB9SInstaller

### Prima di avviare SafeB9SInstaller

:::details Impossibile aprire SafeB9SInstaller.bin

Il file `SafeB9SInstaller.bin` è mancante o mal posizionato. Scarica l'ultima versione di [SafeB9SInstaller](https://github.com/d0k3/SafeB9SInstaller/releases/download/v0.0.7/SafeB9SInstaller-20170605-122940.zip), estraila e posiziona il file 'SafeB9SInstaller.bin' della directory principale della tua scheda SD. Non aggiungere l'estensione `.bin` se non la vedi presente.

:::

### SigHaxed FIRM was not installed! Check lower screen for more info.

:::details MicroSD Card - init failed

La tua scheda SD ha probabilmente qualcosa che non va. Prova a riformattarla ([Windows](formatting-sd-\(windows\)), [macOS](formatting-sd-\(mac\)), [Linux](formatting-sd-\(linux\))). Se questo non risolve il problema, prova una scheda SD diversa.

:::

:::details SigHaxed FIRM - File not found

Ti mancano i file `boot9strap.firm` e `boot9strap.firm.sha` dalla cartella `boot9strap`, o la cartella `boot9strap` non è stata correttamente nominata. Scarica l'ultima versione di [boot9strap](https://github.com/SciresM/boot9strap/releases/download/1.4/boot9strap-1.4.zip), e posiziona i file `boot9strap.firm` e `boot9strap.firm.sha` nella cartella `boot9strap`.

:::

:::details SigHaxed FIRM - invalid FIRM

C'è un problema con i tuoi file `boot9strap.firm` e `boot9strap.firm.sha`. Ri-scarica l'ultima versione di [boot9strap](https://github.com/SciresM/boot9strap/releases/download/1.4/boot9strap-1.4.zip), e posiziona i file `boot9strap.firm` e `boot9strap.firm.sha` nella cartella `boot9strap`.

:::

:::details Secret Sector - File not found

Ti manca il file `secret_sector.bin` dalla cartella `boot9strap`, o la cartella `boot9strap` non è stata correttamente nominata. Scarica [secret_sector.bin](magnet:?xt=urn:btih:15a3c97acf17d67af98ae8657cc66820cc58f655\&dn=secret_sector.bin\&tr=udp%3a%2f%2ftracker.torrent.eu.org%3a451%2fannounce\&tr=udp%3a%2f%2ftracker.lelux.fi%3a6969%2fannounce\&tr=udp%3a%2f%2ftracker.loadbt.com%3a6969%2fannounce\&tr=udp%3a%2f%2ftracker.moeking.me%3a6969%2fannounce\&tr=udp%3a%2f%2ftracker.monitorit4.me%3a6969%2fannounce\&tr=udp%3a%2f%2ftracker.ololosh.space%3a6969%2fannounce\&tr=udp%3a%2f%2ftracker.pomf.se%3a80%2fannounce\&tr=udp%3a%2f%2ftracker.srv00.com%3a6969%2fannounce\&tr=udp%3a%2f%2ftracker.theoks.net%3a6969%2fannounce\&tr=udp%3a%2f%2ftracker.tiny-vps.com%3a6969%2fannounce\&tr=udp%3a%2f%2fopen.tracker.cl%3a1337%2fannounce\&tr=udp%3a%2f%2ftracker.zerobytes.xyz%3a1337%2fannounce\&tr=udp%3a%2f%2ftracker1.bt.moack.co.kr%3a80%2fannounce\&tr=udp%3a%2f%2fvibe.sleepyinternetfun.xyz%3a1738%2fannounce\&tr=udp%3a%2f%2fwww.torrent.eu.org%3a451%2fannounce\&tr=udp%3a%2f%2ftracker.openbittorrent.com%3a6969%2fannounce\&tr=udp%3a%2f%2f9.rarbg.com%3a2810%2fannounce\&tr=udp%3a%2f%2ftracker.opentrackr.org%3a1337%2fannounce\&tr=udp%3a%2f%2fexodus.desync.com%3a6969%2fannounce\&tr=http%3a%2f%2fopenbittorrent.com%3a80%2fannounce) con un client torrent, e posizionalo nella cartella `boot9strap`.

:::

:::details Qualcos'altro

Entra nel [canale Discord di Nintendo Homebrew](https://discord.gg/MWxPgEp) per ricevere assistenza, e indica il messaggio che ricevi.

:::

## Installazione di boot9strap (Soundhax)

:::details Schermata rossa/viola/rosa e bianca dopo aver eseguito Soundhax

Se la tua console è alla versione di sistema 9.4.0, 9.5.0 o 9.6.0, potresti riscontrare problemi usando una vecchia versione di universal-otherapp. Scarica l'ultima versione da [qui. Scarica l'ultima versione da [qui](https://github.com/TuxSH/universal-otherapp/releases/latest).

Se la tua console non ha queste versioni di sistema, probabilmente hai già un custom firmware. Dovresti [verificare la presenza di un CFW](checking-for-cfw).

:::

:::details "Si è verificato un errore che ha provocato la chiusura del software..." (messaggio d'errore su schermata bianca)

C'è un problema con il tuo file `otherapp.bin` (è mancante, mal posizionato o corrotto). Scarica l'ultima versione di [universal-otherapp](https://github.com/TuxSH/universal-otherapp/releases/latest) e inseriscila nella directory principale della tua scheda SD.

:::

:::details "Impossibile riprodurre"

Hai il file Soundhax sbagliato per la tua console e regione, o la tua console è incompatibile con Soundhax. In quest'ultimo caso, dovrai scoprire la versione presente sul tuo 3DS. Entra nel [canale Discord di Nintendo Homebrew](https://discord.gg/MWxPgEp) per chiedere assistenza.

:::

:::details Impossibile leggere la scheda SD!

Se il problema non si risolve, prova ad usare un'altra scheda SD.

:::

## Installazione di boot9strap (MSET9)

:::details Python 3 is not installed

Python non è installato sul computer che stai utilizzando. Scaricalo dal [sito di Python](https://www.python.org/downloads/), fai doppio clic sull'installer e segui le istruzioni a schermo per installare Python. Una volta installato Python, riprova.

:::

:::details HOME Menu extdata: Missing!

Accendi la console con la scheda SD inserita, quindi controlla nuovamente lo stato di MSET9.

Se non funziona, la scheda SD deve essere formattata:

1. Copia tutto dalla scheda SD sul tuo PC
2. Formatta la scheda SD ([Windows](formatting-sd-\(windows\)), [Linux](formatting-sd-\(linux\)), [macOS](formatting-sd-\(mac\)))
3. Ricopia tutto nella scheda SD
4. Ricomincia dalla [Sezione I Passo 7](installing-boot9strap-\(mset9-cli\)#section-i---prep-work)

:::

:::details Mii Maker extdata: Missing!

I dati del Centro di creazione Mii non sono stati trovati sulla scheda SD. Accendi la console con la scheda SD inserita, avvia il Centro di creazione Mii, quindi controlla nuovamente lo stato di MSET9.

Se non funziona, la scheda SD deve essere formattata:

1. Copia tutto dalla scheda SD sul tuo PC
2. Formatta la scheda SD ([Windows](formatting-sd-\(windows\)), [Linux](formatting-sd-\(linux\)), [macOS](formatting-sd-\(mac\)))
3. Ricopia tutto nella scheda SD
4. Ricomincia dalla [Sezione I Passo 8](installing-boot9strap-\(mset9-cli\)#section-i---prep-work).

:::

:::details Title database: Not initialized!

Assicurati di aver resettato il database dei titoli.

- Accendi la console con la scheda SD inserita
- Avvia le Impostazioni della console e vai su `Gestione dati` -> `Nintendo 3DS` -> `Software` -> Reset ([immagine](/images/screenshots/database-reset.jpg))
  - Non verranno cancellati i tuoi dati
- Se ricevi una conferma di ripristino, al termine spegni e riaccendi la console e ricomincia dalla [Sezione I Passo 14](installing-boot9strap-\(mset9-cli\)#section-i---prep-work)

Se _non_ ricevi una conferma di ripristino, la tua scheda SD deve essere formattata:

1. Copia tutto dalla scheda SD sul tuo PC
2. Formatta la scheda SD ([Windows](formatting-sd-\(windows\)), [Linux](formatting-sd-\(linux\)), [macOS](formatting-sd-\(mac\)))
3. Ricopia tutto nella scheda SD

<!--@include: ./_include/mset9-chorus.md -->

1. Digita il numero corrispondente al modello di console e alla versione, quindi premi Invio
2. Digita `2` quindi premi Invio per controllare lo stato di MSET9
   - Verranno ricreati nuovamente i database fittizi
3. Chiudi la finestra dello script MSET9
4. Ricomincia dalla [Sezione I Passo 12](installing-boot9strap-\(mset9-cli\)#section-i---prep-work).

:::

:::: details Error 01: Couldn't find Nintendo 3DS folder

Non stai eseguendo MSET9 dalla directory principale della scheda SD, oppure manca la cartella Nintendo 3DS.

Ricorda, la tua scheda SD dovrebbe assomigliare a questo:

::: info

![](/images/screenshots/mset9/mset9-root-layout.png)

:::

Se il contenuto della scheda SD è corretto, la scheda SD molto probabilmente non sta venendo letta dalla console e deve essere formattata:

1. Copia tutto dalla scheda SD sul tuo PC
2. Formatta la scheda SD ([Windows](formatting-sd-\(windows\)), [Linux](formatting-sd-\(linux\)), [macOS](formatting-sd-\(mac\)))
3. Ricopia tutto nella scheda SD
4. Ricomincia dall'inizio della [Sezione I](installing-boot9strap-\(mset9-cli\)#section-i---prep-work)

::::

:::details Error 02: Your SD is write protected

La protezione da scrittura è abilitata su questa scheda SD. Se stai utilizzando una scheda SD standard, assicurati che il blocco sia impostato [verso l'alto](/images/sdlock.png). Altrimenti, prova a espellere e reinserire la scheda SD.

:::

:::details Error 04: You don't have 1 ID0, you have (#)!

Hai più cartelle ID0. Per determinare la cartella corretta, segui queste istruzioni:

1. Rinomina la cartella `Nintendo 3DS` in `BACKUP_Nintendo 3DS`
2. Reinserisci la scheda SD nella tua console
3. Accendi la tua console
4. Attendi che la console generi i dati nella scheda SD
   - Le tue applicazioni saranno scomparse. È normale e verrà risolto a breve
5. Spegni la tua console
6. Inserisci la scheda SD nel tuo computer
7. Entra nella cartella `Nintendo 3DS` della tua scheda SD
8. Trascrivi i primi caratteri della cartella che vedi
   - Questo è il tuo vero ID0, che manterremo nella cartella Nintendo 3DS reale
9. Elimina la cartella ID0 dalla cartella `Nintendo 3DS` corrente
10. Sposta la vera cartella ID0 dalla cartella `BACKUP_Nintendo 3DS` nella cartella `Nintendo 3DS`
11. Se esiste, sposta la cartella `Private` dalla cartella `BACKUP_Nintendo 3DS` nella cartella `Nintendo 3DS`

Al termine, continua dalla [Sezione I Passo 3](installing-boot9strap-\(mset9-cli\)#section-i---prep-work).

:::

:::: details Error 05: You don't have 1 ID1, you have (#)!

<!--@include: ./_include/id1-check.md -->

::::

:::details Error 06: You need at least 16MB free

La tua scheda SD non ha abbastanza spazio per eseguire MSET9. Libera un po' di spazio e riprova.

Al termine di questa guida avrai bisogno di almeno 1.3GB di spazio per fare un backup della NAND, quindi è meglio liberarne almeno altrettanto.

:::

:::details Error 07: One or more files are missing or malformed!

Uno o più file necessari all'esecuzione di MSET9 mancano o sono corrotti. Ri-scarica il file [Release `.zip` di MSET9](https://github.com/hacks-guide/MSET9/releases/latest) ed estrailo nella directory principale della tua scheda SD, sostituendo tutti i file esistenti, quindi riprova.

:::

:::details Error 18: Windows Locale Settings are broken!

<!--@include: ./_include/winerror234.md -->

:::

:::details Schermata rossa dopo il reinserimento della scheda SD (Sezione II Passo 11)

Potrebbe mancarti il file `SafeB9S.bin` dalla directory principale della tua scheda SD, o il file potrebbe essere danneggiato. Copialo dal'archivio `.zip` di MSET9, sostituendo qualsiasi file esistente, quindi segui queste istruzioni per rimuovere il file scatenante:

1. Forza lo spegnimento della console tenendo premuto il pulsante d'accensione per 20 secondi
2. Inserisci la scheda SD nel tuo computer

<!--@include: ./_include/mset9-chorus.md -->

1. Digita il numero corrispondente al modello di console e alla versione, quindi premi Invio
   - Lo stato attuale dovrebbe visualizzare [Injected](/images/screenshots/mset9/mset9-injected.png)
   - Se hai già rimosso il file scatenante (o non l'hai mai iniettato), lo stato attuale mostrerà [Ready](/images/screenshots/mset9/mset9-ready.png), e puoi [riprovare la Sezione II](installing-boot9strap-\(mset9-cli\)#section-ii---mset9)
2. Digita `4`, quindi premi Invio
3. Una volta che la finestra dice "Removed trigger file", digita `0` quindi premi Invio
4. Reinserisci la scheda SD nella console
5. Accendi la tua console
6. Ritorna alla [Sezione II Passo 1](installing-boot9strap-\(mset9-cli\)#section-ii---mset9)

Altrimenti, la scheda SD potrebbe essere formattata o partizionata in modo errato. Dopo aver rimosso il file scatenante, formattala:

1. Copia tutto dalla scheda SD sul tuo PC
2. Formatta la scheda SD ([Windows](formatting-sd-\(windows\)), [Linux](formatting-sd-\(linux\)), [macOS](formatting-sd-\(mac\)))
3. Ricopia tutto nella scheda SD
4. Ricomincia dalla [Sezione II Passo 1](installing-boot9strap-\(mset9-cli\)#section-ii---mset9)

:::

:::details Caricamento infinito delle Impostazioni della console dopo il reinserimento della scheda SD

Molto probabilmente hai fatto qualcosa di diverso dalle istruzioni di MSET9, selezionato il modello/versione sbagliata, o la scheda SD deve essere formattata. Assicurati di aver scelto il [modello](/images/3dsmodels.png) e versione del sistema corretti all'apertura dello script.

Segui queste istruzioni per rimuovere il file scatenante e riprova la Sezione II:

1. Forza lo spegnimento della console tenendo premuto il pulsante d'accensione per 20 secondi
2. Inserisci la scheda SD nel tuo computer

<!--@include: ./_include/mset9-chorus.md -->

1. Digita il numero corrispondente al modello di console e alla versione, quindi premi Invio
   - Lo stato attuale dovrebbe visualizzare [Injected](/images/screenshots/mset9/mset9-injected.png)
   - Se hai già rimosso il file scatenante (o non l'hai mai iniettato), lo stato attuale mostrerà [Ready](/images/screenshots/mset9/mset9-ready.png), e puoi riprovare la Sezione II
2. Digita `4`, quindi premi Invio
3. Una volta che la finestra dice "Removed trigger file", digita `0` quindi premi Invio
4. Reinserisci la scheda SD nella console
5. Accendi la tua console
6. Ritorna alla [Sezione II Passo 1](installing-boot9strap-\(mset9-cli\)#section-ii---mset9)

Se continui ad avere questo problema e sei sicuro di avere fatto tutto correttamente, assicurati che il file scatenante sia stato rimosso e formatta la tua scheda SD:

1. Copia tutto dalla scheda SD sul tuo PC
2. Formatta la scheda SD ([Windows](formatting-sd-\(windows\)), [Linux](formatting-sd-\(linux\)), [macOS](formatting-sd-\(mac\)))
3. Ricopia tutto nella scheda SD
4. Ricomincia dalla [Sezione II Passo 1](installing-boot9strap-\(mset9-cli\)#section-ii---mset9)

:::

:::details An exception occurred after triggering MSET9

Probabilmente significa che hai già un custom firmware. Dovresti [verificare la presenza di un CFW](checking-for-cfw).

:::

## Installazione di boot9strap (super-skaterhax)

:::details "Si è verificato un errore. Salva i dati di qualunque applicazione attualmente in uso, quindi riavvia la console."

Se nessun colore lampeggia dopo aver premuto "GO GO!":

- Assicurati di aver impostato correttamente la data di sistema e [regione](/images/screenshots/skater/skater-lang.png)
- Assicurarsi che non siano aperte altre schede del browser, quindi riavvia il browser e ritenta l'exploit

Se lo schermo lampeggia con i colori, poi si blocca o crasha:

- Assicurati di avere la versione corretta di `arm11code.bin` e `browserhax_hblauncher_ropbin_payload.bin` per la versione e la regione della tua console
- Prova a reimpostare i dati del browser:
  1. Avvia il browser internet, quindi apri le sue impostazioni
  2. Scorri verso il basso e seleziona "Reimposta tutti i dati salvati" (può avere nomi simili come "Inizializza i dati di salvataggio" o "Elimina tutti i dati salvati")
  3. Riprova ad eseguire l'exploit
- Prova a cambiare la lingua di sistema in una lingua diversa da quella corrente

:::

:::: details "Si è verificato un errore. Tieni premuto il pulsante POWER per spegnere la console..." (schermata nera con testo)

Il file `arm11code.bin` è mancante o mal posizionato. Assicurati di copiare i file [dell'ultima versione di super-skaterhax](https://github.com/zoogie/super-skaterhax/releases/latest) per la tua regione e versione della console nella directory principale della tua scheda SD (non all'interno di una cartella).

::: info

![](/images/screenshots/skaterhax/skater-root-layout.png)

:::

::::

:::details Si verifica un'eccezione oppure "DLL_HEAP_INFORMATION" premendo GO! GO!

Probabilmente significa che hai già un custom firmware. Dovresti [verificare la presenza di un CFW](checking-for-cfw).

:::

## Installazione di boot9strap (SSLoth-Browser)

:::details Schermata rossa/viola/rosa e bianca dopo aver eseguito Browserhax

Probabilmente significa che hai già un custom firmware. Dovresti [verificare la presenza di un CFW](checking-for-cfw).

:::

:::details "Si è verificato un errore. Tieni premuto il pulsante POWER per spegnere la console..." (schermata nera con testo)

Il file `arm11code.bin` è mancante o mal posizionato. Scarica l'ultima versione di [universal-otherapp](https://github.com/TuxSH/universal-otherapp/releases/latest), posiziona il file `otherapp.bin` nella directory principale della tua scheda SD`e rinominalo in`arm11code.bin`. Non aggiungere l'estensione `.bin\` se non la vedi presente.

:::

:::details "Si è verificato un errore che ha provocato la chiusura del software..." (messaggio d'errore su schermata bianca)

Potrebbe esserci un problema con il tuo file `arm11code.bin`. Scarica l'ultima versione di [universal-otherapp](https://github.com/TuxSH/universal-otherapp/releases/latest), posiziona il file `otherapp.bin` nella directory principale della tua scheda SD`e rinominalo in`arm11code.bin`. Non aggiungere l'estensione `.bin\` se non la vedi presente.

Puoi anche provare a resettare i dati del tuo browser:

1. Avvia il browser internet, quindi apri le sue impostazioni
2. Scorri verso il basso e seleziona "Reimposta tutti i dati salvati" (può avere nomi simili come "Inizializza i dati di salvataggio" o "Elimina tutti i dati salvati")
3. Riprova ad eseguire l'exploit

:::

:::details Crash aprendo il codice QR di browserhax o l'URL

Gli exploit basati sul browser (come questo) sono instabili e crashano spesso, ma seguendo i seguenti passaggi, i problemi potrebbero venire risolti.

1. Avvia il browser internet, quindi apri le sue impostazioni
2. Scorri verso il basso e seleziona "Reimposta tutti i dati salvati" (può avere nomi simili come "Inizializza i dati di salvataggio" o "Elimina tutti i dati salvati")
3. Riprova ad eseguire l'exploit

:::

:::details Richiesta di aggiornamento di sistema all'apertura del browser

Il proxy SSLoth è stato configurato in modo errato. Ripeti la sezione SSLoth della pagina.

:::

:::details Errore 032-0420 all'apertura del browser

Segui in ordine questi passaggi:

1. Avvia le Impostazioni di sistema sulla tua console
2. Entra in `Impostazioni Internet` -> `Impostazioni di collegamento`
3. Clicca sulla tua connessione wifi e naviga su `Modifica` -> `Pagina Successiva (la freccia a destra)` -> `Impostazioni proxy`
4. Imposta "Impostazioni proxy" su "No"
5. Fai clic su OK, quindi su Salva
6. Quando richiesto, clicca su "Test" per eseguire il test di connessione
   - Il test dovrebbe andare a buon fine
7. Clicca "OK" per continuare
8. Premi "Indietro" due volte, poi "Chiudi" per tornare al menu HOME
9. Apri il Browser Internet una volta sola
10. Se ti viene richiesto di fare un aggiornamento di sistema, premi OK
    - Non verrà effettivamente aggiornato il sistema
11. Ricomincia dalla [Sezione II](installing-boot9strap-\(ssloth-browser\).html#section-ii---ssloth)

:::

:::details Bloccato su "Doing agbhax..."

Potrebbe esserci un problema con il tuo file `arm11code.bin`. Riscarica l'ultima versione di [universal-otherapp](https://github.com/TuxSH/universal-otherapp/releases/latest), posizionala nella directory principale della tua scheda SD`e rinominalo in`arm11code.bin`. Non aggiungere l'estensione `.bin\` se non la vedi presente.

:::

:::details "PrepareArm9ForTwl returned error c8804631!"

Entra nel [canale Discord di Nintendo Homebrew](https://discord.gg/MWxPgEp) per chiedere assistenza.

:::

:::details Impossibile leggere la scheda SD!

Effettua il backup dei tuoi dati e riformatta la tua scheda SD come FAT32 con lo strumento consigliato a seconda del sistema operativo ([Windows](formatting-sd-\(windows\)), [macOS](formatting-sd-\(mac\)), [Linux](formatting-sd-\(linux\))). MiniTool Partition Wizard e lo strumento di formattazione HP (HPUSBDisk) sono noti per causare problemi con schede SD 3DS.

Se il problema non si risolve, prova ad usare un'altra scheda SD.

:::

## Completamento dell'installazione

:::details Impossibile aggiornare la console

I passaggi qui sotto possono essere seguiti in qualsiasi ordine, ma sono elencati dal più facile al più difficile da eseguire.

1. Se stai usando Pretendo, ritorna a Nintendo con Nimbus e riprova
2. Imposta le impostazioni DNS su "Auto"
3. Avvicinati al tuo router WiFi
4. Aggiorna tramite la Safe Mode spegnendo la console, tenendo premuti (L) + (R) + (D-Pad Su) + (A) all'avvio, e seguendo le istruzioni a schermo
5. Elimina il profilo di connessione WiFi, quindi connettiti di nuovo alla rete WiFi
6. Riavvia il tuo router WiFi
7. Connettiti ad una rete WiFi alternativa, ad esempio un hotspot mobile
8. I server Nintendo potrebbero essere irraggiungibili. Riprova più tardi
9. Se continui a ricevere un errore, [segui la guida per il CTRTransfer](ctrtransfer), poi ritenta l'aggiornamento
10. Se hai bisogno di aiuto (in inglese), entra nel [canale Discord di Nintendo Homebrew](https://discord.gg/MWxPgEp)

:::

:::details Error #22: finalize.romfs is invalid

Il file `finalize.romfs` è danneggiato o illeggibile. [Ri-scaricalo](https://github.com/hacks-guide/finalize/releases/latest/download/finalize.romfs) e copialo nella della directory principale della scheda SD, sostituendo qualsiasi file esistente, quindi riprova.

:::

:::details Information #23: finalize.romfs in wrong location

Il file `finalize.romfs` è stato posizionato in maniera errata e non nella directory principale della scheda SD. Lo script tenterà di risolvere questo problema, ma occorre il tuo permesso per farlo. Premi (A) alle prossime richieste per continuare.

:::

:::details Error #24: SD is write-protected

Assicurati che la tua scheda SD non sia [protetta dalla scrittura](/images/sdlock.png). Se la scheda SD non è protetta e continui ad ottenere questo errore, entra nel [canale Nintendo Homebrew su Discord](https://discord.gg/MWxPgEp) per ricevere assistenza.

:::

:::details Error #02: Missing essential.exefs

Hai risposto 'No' alla richiesta "Make essential files backup?" in GodMode9. Spegni la console, riaccendila tenendo premuto (Start) per avviare GodMode9, rispondi 'Yes' alla domanda, quindi riprova.

:::

:::details Error #04: No space

Hai bisogno di almeno 1,3GB di spazio libero per eseguire il backup della NAND, che è una parte dello script. Se non hai abbastanza spazio, segui questi passaggi:

1. Spegni la tua console
2. Inserisci la scheda SD nel tuo computer
3. Copia la cartella `Nintendo 3DS` dalla directory principale della tua scheda SD al tuo computer
4. Elimina la cartella `Nintendo 3DS` dalla scheda SD
5. Reinserisci la scheda SD nella tua console
6. Premi (Start) e accendi la console continuando a tenerlo premuto. Verrà avviato GodMode9
7. Premi il pulsante (Home)
8. Seleziona "Scripts..."
9. Seleziona "finalize"
10. Premi (A) per creare un backup della NAND
    - Potrebbero volerci circa quindici minuti
11. Premi di nuovo (A)
    - La console dovrebbe spegnersi automaticamente
12. Inserisci la scheda SD nel tuo computer
13. Copia i file in `/gm9/backups/` sulla tua SD in una posizione sicura sul tuo computer
14. Elimina i file `<data>_<seriale>_sysnand_##.bin` e `<data>_<seriale>_sysnand_##.bin.sha` dalla scheda SD
15. Copia la cartella `Nintendo 3DS` dal tuo computer nella directory principale della tua scheda SD
16. Elimina la cartella `Nintendo 3DS` dal tuo computer

Ora che hai il backup della NAND in un luogo sicuro:

1. Reinserisci la scheda SD nella tua console
2. Premi (Start) e accendi la console continuando a tenerlo premuto. Verrà avviato GodMode9
3. Premi il pulsante (Home)
4. Seleziona "Scripts..."
5. Seleziona "finalize"
6. Continua lo script normalmente
   - Il backup della NAND verrà automaticamente saltato

:::

:::details Information #05: No title database

Premi (A) per importare un database dei titoli, inserisci i pulsanti mostrati a schermo per sbloccare la scrittura su SysNAND, quindi prosegui normalmente con lo script.

:::

:::details Error #06 o "Error: Could not open directory" durante il backup della NAND

Assicurati di avere almeno 1.3GB disponibili nella tua scheda SD. Se non hai abbastanza spazio, segui questi passaggi:

1. Spegni la tua console
2. Inserisci la scheda SD nel tuo computer
3. Copia la cartella `Nintendo 3DS` dalla directory principale della tua scheda SD al tuo computer
4. Elimina la cartella `Nintendo 3DS` dalla scheda SD
5. Reinserisci la scheda SD nella tua console
6. Premi (Start) e accendi la console continuando a tenerlo premuto. Verrà avviato GodMode9
7. Esegui un [Backup NAND](godmode9-usage#creating-a-nand-backup)
8. Copia i file in `gm9/out` sulla tua SD in una posizione sicura sul tuo computer
9. Elimina i file `<data>_<seriale>_sysnand_##.bin` e `<data>_<seriale>_sysnand_##.bin.sha` dalla scheda SD, mantenendo il file `essential.exefs` in `/gm9/out/`
10. Copia la cartella `Nintendo 3DS` dal tuo computer nella directory principale della tua scheda SD
11. Elimina la cartella `Nintendo 3DS` dal tuo computer

Se riieni di avere abbastanza spazio sulla tua scheda SD, questa potrebbe essere danneggiata o difettosa. Verifica la presenza di eventuali errori nella tua scheda SD seguendo la guida corretta per il sistema operativo del tuo computer: [Windows](h2testw-\(windows\)), [Linux](f3-\(linux\)), [macOS](f3xswift-\(mac\)).

:::

:::details Error #12: Copy (file).db fail

Assicurati che la tua scheda SD non sia [protetta dalla scrittura](/images/sdlock.png). Se la scheda SD non è protetta e continui ad ottenere questo errore, entra nel [canale Nintendo Homebrew su Discord](https://discord.gg/MWxPgEp) per ricevere assistenza.

:::

:::details Information #17: Duplicate NAND backup

Lo script ha rilevato che manca la cartella Nintendo 3DS E che hai precedentemente fatto un backup della NAND. Se intendi installare applicazioni homebrew, dovresti fare quanto segue:

1. Premi (B) per annullare la creazione di un altro backup della NAND
2. Tenendo premuto (R), premi (Start) per spegnere la console
3. Copia il contenuto della cartella `/gm9/backups/` in una posizione sicura sul tuo computer
4. Elimina la cartella `/gm9/backups/` dalla tua scheda SD
5. Se hai spostato la cartella Nintendo 3DS al di fuori dalla scheda SD, copiala nuovamente sulla scheda SD
   - Se non hai la cartella Nintendo 3DS, avvia il menu HOME con la scheda SD inserita per generarla automaticamente
6. Premi (Start) e accendi la console continuando a tenerlo premuto. Verrà avviato GodMode9
7. Premi il pulsante HOME per far apparire il menu delle azioni
8. Seleziona "Scripts..."
9. Seleziona "finalize"
10. Segui le istruzioni dello script, rispondendo alle domande che ti vengono poste

:::

:::details Error #18a/18b: MSET9 detected

Non hai rimosso MSET9 nella pagina precedente. Lo script tenterà di rimuovere MSET9; segui le istruzioni fornite dallo script.

:::

---

## Problemi di avvio su console con custom firmware

::: info

I passaggi qui dettagliati generalmente presuppongono che la tua console abbia un'installazione moderna del custom firmware (boot9strap + Luma3DS 8.0 o superiore). Se la tua console sta eseguendo una vecchia configurazione (ad esempio, qualcosa basato su arm9loaderhax o menuhax), dovresti aggiornare la tua installazione prima di seguire queste istruzioni.

:::

### Indicatori luminosi di accensione/notifica

:::details La mia console si spegne quando provo ad accenderla, e/o il LED di notifica mostra un colore all'accensione

C'è un problema con il tuo file `boot.firm`. Se stai usando [boot9strap 1.4](https://github.com/SciresM/boot9strap/releases/tag/1.4), il tuo LED di notifica 3DS potrebbe lampeggiare di un certo colore. Questo colore è usato per diagnosticare problemi riguardanti il tuo file `boot.firm` nella scheda SD o nella memoria interna. Su versioni molto vecchie di boot9strap, la luce blu si spegne quasi subito quando si tenta di accendere la console.

Se il LED di notifica lampeggia:

- **Bianco**: Il tuo 3DS non è stato in grado di trovare il file `boot.firm` nella tua scheda SD o nella memoria interna.
- **Magenta**: Il tuo 3DS non è stato in grado di trovare il file `boot.firm` nella tua scheda SD. È stato in grado di trovare il file `boot.firm` nella memoria interna, tuttavia il file è corrotto.
- **Rosso**: Il tuo 3DS è stato in grado di trovare il file `boot.firm` sia nella tua scheda SD sia nella memoria interna, tuttavia entrambi i file sono corrotti.

Puoi ottenere un nuovo file `boot.firm` scaricando l'[ultima versione di Luma3DS](https://github.com/LumaTeam/Luma3DS/releases/latest), estraendola e posizionando il file `boot.firm` nella directory principale della tua scheda SD. Se il tuo file `boot.firm` continua a risultare corrotto, potresti dover verificare la presenza di errori nella tua scheda SD ([Windows](h2testw-\(windows\)), [Linux](f3-\(linux\)), o [macOS](f3xswift-\(mac\))). Inoltre, tieni presente che il 3DS tende ad avere problemi con file estratti usando WinRAR.

Se si sente un "suono scoppiettante", potenzialmente seguito dalla retroilluminazione accendersi per un istante, c'è un problema hardware con la tua console (come un cavo della retroilluminazione disconnesso). Potresti riuscire ad accendere la console tenendola in determinate posizioni.

:::

:::details La mia console si blocca con una schermata nera e la luce di accensione rimane blu

I passaggi qui sotto possono essere seguiti in qualsiasi ordine, ma sono elencati dal più rapido al più lungo da eseguire.

1. Spegni la tua console, rimuovi la scheda SD, reinseriscila, quindi accendi la tua console.
2. Spegni la tua console, estrai la cartuccia di gioco se inserita, accendi la tua console, quindi attendi fino a dieci minuti. Se la tua console si avvia entro dieci minuti, il problema è stato risolto e probabilmente non avverrà più
3. Rinomina la cartella `Nintendo 3DS` sulla tua scheda SD in `Nintendo 3DS_BACKUP`, poi tenta l'avvio. Se la tua console si avvia correttamente, c'è qualche problema con la tua cartella `Nintendo 3DS`. Prova a cancellare gli extdata del menu HOME:
   - Entra nella cartella `/Nintendo 3DS/<ID0>/<ID1>/extdata/00000000/`
   - Elimina la cartella corrispondente per la tua regione 3DS:
     - **Regione EUR**: Elimina `00000098`
     - **Regione JPN**: Elimina `00000082`
     - **Regione USA**: Elimina `0000008f`
     - **Regione CHN**: Elimina `000000A1`
     - **Regione KOR**: Elimina `000000A9`
     - **Regione TWN**: `000000B1`
4. Prova ad avviare la modalità di ripristino e ad aggiornare la console:
   - Spegni la tua console
   - Tieni premuti i pulsanti (L) + (R) + (Su) + (A)
   - Accendi la tua console
   - Se hai avuto successo, la console si avvierà mostrando la schermata "Aggiornamento"
5. Segui la guida [CTRTransfer](ctrtransfer)
6. Se hai bisogno di aiuto, chiedi pure nel [canale Discord di Nintendo Homebrew](https://discord.gg/MWxPgEp)

:::

### Messaggio di errore all'avvio

:::details "An error has occurred: Failed to apply 1 FIRM patch(es)" o "An exception has occurred -- Current process: pm"

La tua versione di Luma3DS è obsoleta. Scarica l'ultima versione di [Luma3DS](https://github.com/LumaTeam/Luma3DS/releases/latest) e posiziona il file `boot.firm` nella directory principale della tua scheda SD, sostituendo qualunque file preesistente. Assicurati di non stare estraendo il file ZIP con WinRAR, in quanto è noto per causare problemi con file relativi al 3DS.

:::

:::details "Unable to mount CTRNAND or load the CTRNAND FIRM. Please use an external one."

Ci sono diverse ragioni per cui questo potrebbe accadere. In ogni caso, questo errore di solito si può risolvere seguendo la guida [CTRTransfer](ctrtransfer).

:::

:::details "Si è verificato un errore. Tieni premuto il pulsante POWER per spegnere la console..."

I gestori di eccezione ARM11 sono disabilitati, o un custom firware non è installato. Prova ad abilitare i gestori di eccezione ARM11:

- Spegni la tua console
- Tieni premuto (Select)
- Accendi la tua console, continuando a tenere premuto il pulsante (Select)
- Se la casella "Disable ARM11 exception handlers" è selezionata, deselezionala

:::

:::details Al menu HOME mancano delle applicazioni installate

Questo potrebbe essere causato da vari motivi, ma principalmente perché la scheda SD non viene letta dal sistema.
Puoi controllare se la tua SD non viene letta tenendo premuto SELECT all'avvio e controllando il testo giallo nella schermata inferiore; se dice "Booted from CTRNAND via B9S", la console si sta avviando dalla memoria interna e non dalla scheda SD.
Se è questo il caso, prova a seguire i seguenti passaggi, indicati dal più semplice al più complesso:

1. Spegni la tua console, rimuovi la scheda SD, reinseriscila, quindi accendi la tua console
2. Spegni la console, rimuovi la scheda SD, inseriscila sul tuo computer, scarica l'ultima versione di [Luma3DS](https://github. om/LumaTeam/Luma3DS/releases/latest), estrai il file `boot.firm` dall'archivio `Luma3DS.zip` e posizionalo nella directory principale della tua scheda SD (sostituendo qualunque file preesistente)
3. Spegni la console, rimuovi la scheda SD, inseriscila sul tuo computer e formatta la scheda SD secondo il sistema operativo del computer: [Windows](formatting-sd-\(windows\)), [macOS](formatting-sd-\(mac\)), [Linux](formatting-sd-\(linux\)) _(questo cancellerà i dati della tua scheda SD)_
4. Verifica la presenza di eventuali errori nella tua scheda SD seguendo la guida corretta per il sistema operativo del tuo computer: [Windows](h2testw-\(windows\)), [Linux](f3-\(linux\)), [macOS](f3xswift-\(mac\)). Se la tua scheda SD è contrassegnata come difettosa, allora dovrai sostituirla
5. Lo slot della tua scheda SD potrebbe essere rotto. Entra nel [canale Discord di Nintendo Homebrew](https://discord.gg/MWxPgEp) per chiedere assistenza

:::

:::details Schermata blu con la scritta "BOOTROM ERROR"

La tua console è probabilmente brickata. Dovrai acquistare una flashcart ntrboot per reinstallare boot9strap e tentare riparare la tua console. Potrebbe anche indicare un problema hardware non risolvibile. In ogni caso, entra nel [canale Discord di Nintendo Homebrew](https://discord.gg/MWxPgEp) per chiedere assistenza.
\+ È anche possibile che qualcuno abbia impostato una schermata di avvio a tempo che assomigli al messaggio di errore. Prova a lasciare la tua console accesa sulla schermata blu per cinque minuti.

:::

:::details Qualche altro errore

Per favore scatta una foto dell'errore ed entra nel [canale Discord di Nintendo Homebrew](https://discord.gg/MWxPgEp) per ricevere assistenza.

:::

## Problemi software su console con custom firmware

:::details La funzionalità DSi / DS è corrotta o è stata sostituita con Flipnote Studio

1. Scarica l'ultima versione di [TWLFix-CFW](https://github.com/MechanicalDragon0687/TWLFix-CFW/releases/latest) (il file `.3dsx`)
2. Spegni la tua console
3. Se assente, crea una cartella chiamata `3ds` nella directory principale della tua scheda SD
4. Copia il file `TWLFix-CFW.3dsx` nella cartella `/3ds/` nella tua scheda SD
5. Reinserisci la scheda SD nella tua console
6. Avvia l'Homebrew Launcher
7. Avvia TWLFix-CFW dalla lista degli homebrew disponibili
8. Premi il pulsante (A) per disinstallare i titoli TWL corrotti
9. Premi (Start) per riavviare la console
10. Aggiorna la console andando su Impostazioni della console, poi "Impostazioni generali", infine scorri a destra e seleziona "Aggiornamento"
    - L'aggiornamento si occuperà di disinstallare i principali titoli TWL, per riscaricarli e reinstallarli
11. Al termine dell'aggiornamento, premi "OK" per riavviare la console

:::

:::details La funzionalità GBA Virtual Console e/o Modalità Provvisoria è corrotta

La tua console sta eseguendo Luma3DS 6.6 o precedente, probabilmente tramite arm9loaderhax. Dovresti seguire [Da A9LH a B9S](a9lh-to-b9s) per aggiornare la tua console con un custom firmware moderno.

:::

:::details I giochi in modalità memoria estesa (Pokemon Sole/Luna, Smash, ecc.) non funzionano

Questo può verificarsi dopo un CTRTransfer o dopo un cambio di regione su Old 3DS / 2DS. Segui le istruzioni indicate [qui](region-changing#section-vi---fixing-locale-related-issues) per risolvere il problema (saltando i passaggi 3, 4, 5 e 6).

:::

:::details Schermata di errore all'avvio/caricamento di un'applicazione

Cerca la tua schermata di errore in [questa pagina](https://wiki.hacks.guide/wiki/3DS:Error_screens/Luma3DS_exception_screen).
Se non sei stato in grado di trovare il tuo errore o le istruzioni non funzionano, unisciti a [Nintendo Homebrew su Discord](https://discord.gg/MWxPgEp) per ulteriore assistenza.

:::

:::details Avviare le impostazioni del menu HOME crasha la console o carica l'Homebrew Launcher

Probabilmente la tua console ha ancora menuhax67 installato. Per disinstallare menuhax67, scarica l'ultima versione di [menuhax67](https://github.com/zoogie/menuhax67/releases/latest) (il file `.zip` di menuhax), quindi segui la [sezione "Uninstall menuhax67"](https://wiki.hacks.guide/wiki/3DS:Alternate_Exploits/menuhax67#Uninstall_menuhax67).

:::

---

## Risoluzione di ulteriori problemi

:::details Cancellare gli extdata del menu Home

1. Spegni la tua console
2. Inserisci la scheda SD nel tuo computer
3. Entra nella cartella `/Nintendo 3DS/<ID0>/<ID1>/extdata/00000000/` presente all'interno della tua scheda SD
4. Elimina la cartella corrispondente per la tua regione 3DS:
   - **Regione EUR**: Elimina `00000098`
   - **Regione JPN**: Elimina `00000082`
   - **Regione USA**: Elimina `0000008f`
   - **Regione CHN**: Elimina `000000A1`
   - **Regione KOR**: Elimina `000000A9`
   - **Regione TWN**: `000000B1`
5. Reinserisci la scheda SD nella tua console

:::

:::details Pulizia dei dati dei temi del menu HOME

1. Spegni la tua console
2. Inserisci la scheda SD nel tuo computer
3. Entra nella cartella `/Nintendo 3DS/<ID0>/<ID1>/extdata/00000000/` presente all'interno della tua scheda SD
4. Elimina la cartella corrispondente per la tua regione 3DS:
   - **Regione EUR**: `000002ce`
   - **Regione JPN**: `000002cc`
   - **Regione USA**: `000002cd`
   - **Regione KOR**: `000002cf`
5. Reinserisci la scheda SD nella tua console

:::

:::details Avvio manuale dell'Homebrew Launcher

Se ti manca l'applicazione Homebrew Launcher dal menu HOME, puoi seguire queste istruzioni per avviarlo manualmente. (Avrai bisogno dei file [boot.3dsx e boot.firm](https://github.com/LumaTeam/Luma3DS/releases/latest) nella directory principale della tua scheda SD.)

<!--@include: ./_include/launch-hbl-dlp.md -->

:::

:::details Disattivare il Filtro famiglia

È possibile disattivare la funzione Filtro famiglia entrando in Impostazioni della console -> Filtro famiglia e inserendo il PIN, quindi premendo "Cancella impostazioni", e infine "Cancella" per rimuoverlo.
Tuttavia, se non conosci il PIN e quindi non puoi accedere alle impostazioni della console, dovrai disabilitarlo. A tal scopo, dovrai ottenere la master key della tua console (mkey):

1. Vai su [questo sito](https://mkey.eiphax.tech/)
2. Riempi le caselle con le seguenti informazioni:
   - Device Type: Seleziona "3DS" (vale anche se stai usando un 2DS, New 3DS (XL/LL) o New 2DS (XL/LL))
   - System Date: Il giorno e il mese impostati nella tua console
   - Inquiry Number: Si può ottenere premendo "Ho dimenticato il PIN" e poi "L'ho dimenticato" nella schermata Filtro famiglia
3. Dopo aver ottenuto il tuo mkey, premi OK sulla schermata in cui hai ottenuto il tuo Inquiry Number, quindi inserisci la master key
4. Premi "Cancella le impostazioni", quindi "Cancella" per rimuovere tutti i dati del Filtro famiglia

:::
