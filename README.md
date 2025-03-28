# WOS ---Work In Proress: prima bozza---
World Of Warcraft Optimization Settings
## Indice
- [Intro](#intro)
- [Pc Settings](#pc-settings)
  - [Bios Settings](#bios-settings)
  - [Windows Settings](#windows-settings)
  - [Driver Settings](#driver-settings)
  - [Programm Settings](#programm-settings)
  - [Battle.net Settings](#bnet-settings)
- [Wow Settings](#wow-settings)
- [Addons Settings](#addons-settings)
  - [Addons & WA Updater](#wowup-wago)
  - [Addons & WA Settings](#addons-wa-settings)
- [Fix & Workaround](#fix-workaround)
- [Change-log](#change-log)

## Intro
Salve sono Scarna86, su WoW sono Itanku, Monk Brewmaster. Ho voluto finalmente raccogliere tutte le informazione e le esperienze che conosco per migliorare ed ottimizzare World of Warcraft al meglio, in particolare per l'ambiente raid, m+ e competitivo in generale.

I miei sono CONSIGLI, come tali potete scegliere di seguirli o meno, come tali verrà segnalato quando una modifica puo risultare pericolosa ed il grado di difficoltà nel metterla in pratica.
Sentitive liberi di consigliarmi suggerimenti o modiciche, e segnalare possibili errori. Vorrei che questa guida resti fruibile a chiunque ne abbia bisogno per giocare al meglio al nostro "amato/odiato" gioco.
Grazie e buon game!

## PC Settings
### Bios Settings
Saltabile: SI 

Difficoltà: Alta 

Pericolo: Alto

Per entrare nel bios del vostro pc avete 2 modi:
- Riavviare il pc, e nella prima schermata con il logo della scheda madre premere ripetutamente il tasto "F2" o il tasto "DEL"/"Canc"
- Da windows cercare "avvio avanzato" e premere "riavvia ora"
Una volta nel bios le opzioni modificabili per migliorare WOW sono:

1 - Abilitare il profilo XMP (x intel) o DOCP (x AMD), nelle schermate principali dei bios l'opzione è quasi sempre in prima vista, abilitarla e premete il tasto "F10" (salva ed esci) e confermare con "INVIO". Questa modifica abilità l'auto overclock delle ram portandole alle specifiche alle quali vengono vendute 

![xmp](https://github.com/user-attachments/assets/e6d953ac-938c-457d-8b0f-9189cecff378)

![Docp](https://github.com/user-attachments/assets/35b31e42-ac94-410d-b4f3-1509d09eb0b0)


  ATTENZIONE! se notate crash, riavvii freeze o schermate BSOD dell'intero PC significa che il vostro pc non supporta appieno il profilo overclock delle ram, in questo case avete 2 opzioni, provare ad aggiornare il bios, per sperare in compatibilità migliorata all'overclock ram, oppure non utilizzare questa funzione. Se il pc inizia un ciclio di riavvii non spaventatevi dopo 3 o 5 riavvii non a buon fine il pc disattiva in automatico il profilo XMP o DOCP, controllate quindi che sia disattivato e salvate, in caso negativo dovrete effetturare un BIOS RESET o CLEAR-MOS

2 - Abilitare SAM / ReBAR / Resaizable Bar per le schede video, in alcuni modelli lo trovate in piccolo in alto o in basso nella schermata principale del bios, in altri lo trovate sotto la sezione PCIE, in coppia si abilita sia ReBAR sia ABOVE 4G DECODING, questa modifica serve a migliorare la gestione della vram della scheda video ed ha beneficio anche per molti altri giochi moderni.

  ATTENZIONE! Non dovrebbero esserci effetti collaterali con questa modifica su sistemi moderni, su sistemi un po piu vecchiotti potrebbe non visualizarsi piu a video nulla, in questo caso dopo 3 o 5 riavvii il sistema dovrebbe disabilitare la funzione e riavviarsi normalmente, in caso negativo dovrete effetturare un BIOS RESET o CLEAR-MOS

### Windows Settings
Saltabile: NO

Difficoltà: Medio-Bassa

Pericolo: Nessuno

Le modifiche alle impostazioni di windows consigliate che possono essere utili non solo per WoW ma per tutti sono le seguenti:

1 - Disabilitare Avvio Rapido.

Questa funzione non ha senso di esistere su PC che montano dischi SSD o NVME, per disabilitarla ci sono mille guide, ve ne lascio 2 random

https://www.asus.com/it/support/faq/1045548/

https://support.lenovo.com/it/it/solutions/ht513773-how-to-enable-or-disable-fast-startup-on-windows-11

2 - Disabilitare Proxy

Queta funzione risulta attiva anche se non configurata, basta cercare "Proxy" dalla ricerca windows e disattivare la funzione. Ora le pagine web dovrebbero caricarsi piu velocemente quando avviate il browser ed eviterete anche reindirizzamente non rischiesti causati magari da programmi indesiderati o malware

3 - App di Avvio

Cercate "app di Avvio" e controllate che non ci siano programmi che partano in automatico all'avvio, esclusi driver e antivirus il resto delle app non dovrebbero partire in automatico.

4 - Impostazioni Schermo

Controllate in impostazioni schermo di avere le seguenti impostazioni:

  - La Risoluzione impostata correttamente del vostro schermo, esempio 1920x1080 se HD, 2440x1440 se 2K, ecc
  - La frequenza di aggiornamento (hz) impostata al massimo del vostro schermo, lo trovate nella sezione "Impostazioni Schermo Avanzate", se avete monitor che vanno a 120 144 165 240 ecc settate di conseguenza
  - Di NON usare la funzione HDR. WoW non supporta HDR e anche forzando l'HDR automatico di windows si potrebbero riscontrare oltre che colori e luminosità non adeguata, crash e freeze del gioco.

5 - Impostazioni Grafica Avanzate

Usate le seguenti impostazioni in impostazioni grafica avanzata

AutoHDR off (wow non lo supporta e potrebbe creare problemi)

Ottimizzazione giochi modalità finestra ON 

Pianificazione GPU con Accellerazione Hardware OFF (detto HAGS, se cercate online praticamente nessun gioco ne trae benefici)

Frequenza aggiornamento variabile OFF (WoW non supporta di base freesync o gsync, forzarlo potrebbe provocare stuttering o tearing, se vi funziona potete tenerlo attivo, altrimenti disattivate

![image](https://github.com/user-attachments/assets/ef3ae958-c104-41ca-801a-d5f68efd679a)

### Driver Settings
Saltabile: NO 

Difficoltà: Media 

Pericolo: Medio

Di base il consiglio per i driver è il seguente:

- Se giocate solo a wow, aggiornateli solo quando escono delle patch major (inizio season, prepatch, ecc) non è necessario aggiornare i driver ad ogni release
- Se giocate ad altro, aggiornate i driver quando il gioco che vi interessa riceve aggiornamenti driver, altrimenti skippate tranquillamente

Detto questo, sia per NVIDIA che per AMD usate installazioni semplici, per Nvidia solo driver e Nvidia App, per Amd solo driver e adrenaline software.

In entrambe le App, non modificare nulla di aggiuntivo, se non disattivare l'overlay e combinazioni tasti.

Per i driver di altre periferiche usate solo versioni di base windows quando possibile, unici esclusi sono driver e software per mouse e tastiere che usano macro o comandi aggiuntivi

GHUB, corsair, razer ecc usate le versioni con meno optional possibili e anche qua disattivate overlay o preload in windows delle parti no necessarie.

### Programm Settings

Saltabile: NO 

Difficoltà: Bassa 

Pericolo: Nessuno

1 - Discord

Disattivare Overlay dal menu impostazioni "rotella in basso" sezione "overlay"
Disattivare Accellerazione Hardware dalla sezione "avanzate"
Scegliete voi se tenere Discord in esecuzione automatica

2 - Browser

Chrome/Edge/firefox disattivare accelerazione hardware. ATTENZIONE! questa modifica serve per allegerire il browser ma impedisce a netflix youtube e altri servizi di video streaming di poter usare la risoluzione 4k e l'hdr, se vi serve mantenere queste opzioni non usate questa modifica

Solo Chrome/Edge disattivare avvio rapido e caricaemnte pagine in background, quando chiudiamo il browser deve essere chiuso no che faccia roba sotto

3 - Altri programmi

Qualunque programma è in uso mentre giocate consuma memoria e memoria video, se potete chiudete app e programmi che non vi servono o settatili senza accelerazione hardware

### Battle.net Settings

Potete avere battle.net installato nelle cartelle di default, controllate che anche lui non abbia accellerazione hardware e che non venga avviato in automatico all'avvio del pc

Per l'installazione di wow invece il consiglio è di installarlo in un percorso semplice fuori dalla cartella di default

Esempio: "C:\Giochi\World of Warcraft" oppure "D:\World of Warcraft"

ATTENZIONE!

Battle.net e WoW supportano solo file system NTFS, se usate hard disk esterni e volete che wow sia installato su di essi, assicuratevi che il file system sia NTFS o il gioco non si aggiorna o da problemi di aggiornamenti infiniti


























