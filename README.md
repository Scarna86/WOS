# WOS ---Work In Proress: prima bozza---
World Of Warcraft Optimization Settings
## Indice
- [Intro](#intro)
- [Pc Settings](#pc-settings)
  - [Bios Settings](#bios-settings)
  - [Windows Settings](#windows-settings)
  - [Driver Settings](#driver-settings)
  - [Programm Settings](#programm-settings)
  - [Battlenet Settings](#battlenet-settings)
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

![image](https://github.com/user-attachments/assets/1d0100cc-fd08-4090-abd8-944d2bc50188)

3 - App di Avvio

Cercate "app di Avvio" e controllate che non ci siano programmi che partano in automatico all'avvio, esclusi driver e antivirus il resto delle app non dovrebbero partire in automatico.

![image](https://github.com/user-attachments/assets/3b45470a-1da3-471f-99fe-a0e0506ada91)

4 - Impostazioni Schermo

Controllate in impostazioni schermo di avere le seguenti impostazioni:

  - La Risoluzione impostata correttamente del vostro schermo, esempio 1920x1080 se HD, 2440x1440 se 2K, ecc
  - La frequenza di aggiornamento (hz) impostata al massimo del vostro schermo, lo trovate nella sezione "Impostazioni Schermo Avanzate", se avete monitor che vanno a 120 144 165 240 ecc settate di conseguenza
  - Di NON usare la funzione HDR. WoW non supporta HDR e anche forzando l'HDR automatico di windows si potrebbero riscontrare oltre che colori e luminosità non adeguata, crash e freeze del gioco.

![image](https://github.com/user-attachments/assets/f2bc1515-e350-435f-a52c-76f3295be5c3)

5 - Impostazioni Grafica Avanzate

Usate le seguenti impostazioni in impostazioni grafica avanzata

AutoHDR off (wow non lo supporta e potrebbe creare problemi)

Ottimizzazione giochi modalità finestra ON 

Pianificazione GPU con Accellerazione Hardware OFF (detto HAGS, se cercate online praticamente nessun gioco ne trae benefici)

Frequenza aggiornamento variabile OFF (WoW non supporta di base freesync o gsync, forzarlo potrebbe provocare crash, stuttering o tearing, se vi funziona potete tenerlo attivo, altrimenti disattivatelo)

![image](https://github.com/user-attachments/assets/ef3ae958-c104-41ca-801a-d5f68efd679a)

### Driver Settings
Saltabile: NO 

Difficoltà: Media 

Pericolo: Medio

Di base il consiglio per i driver è il seguente:

- Se giocate solo a wow, aggiornateli solo quando escono delle patch major (inizio season, prepatch, ecc) non è necessario aggiornare i driver ad ogni release
- Se giocate ad altro, aggiornate i driver quando il gioco che vi interessa riceve aggiornamenti driver, altrimenti skippate tranquillamente

Detto questo, sia per NVIDIA che per AMD usate installazioni semplici, per Nvidia solo driver e Nvidia App, per Amd solo driver e adrenaline software.

In entrambe le App, non modificare nulla di aggiuntivo, se non disattivare l'overlay, photo mode e combinazioni tasti.

![nvidia](https://github.com/user-attachments/assets/2901dac8-50dc-410f-8e78-b73757aa68c9)

![amd](https://github.com/user-attachments/assets/d874dcb4-da36-4435-975a-004d5d1383ea)

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

![image](https://github.com/user-attachments/assets/2a258c2b-f008-4be1-b2d9-e522d80798be)
![image](https://github.com/user-attachments/assets/74165d16-4c95-4525-9570-ffea2fd0c778)
![image](https://github.com/user-attachments/assets/83cd46e9-e8fd-49b6-84d9-2ac10fb07e64)

2 - Browser

Chrome/Edge/firefox disattivare accelerazione hardware. ATTENZIONE! questa modifica serve per allegerire il browser ma impedisce a netflix youtube e altri servizi di video streaming di poter usare la risoluzione 4k e l'hdr, se vi serve mantenere queste opzioni non usate questa modifica

Solo Chrome/Edge disattivare avvio rapido e caricaemnte pagine in background, quando chiudiamo il browser deve essere chiuso no che faccia roba sotto

![image](https://github.com/user-attachments/assets/6b8c2aaa-993f-4203-8a05-c22f44ad3286)

3 - Altri programmi

Qualunque programma è in uso mentre giocate consuma memoria e memoria video, se potete chiudete app e programmi che non vi servono o settatili senza accelerazione hardware

### Battlenet Settings

Potete avere battle.net installato nelle cartelle di default, controllate che anche lui non abbia accellerazione hardware e che non venga avviato in automatico all'avvio del pc

![bnet](https://github.com/user-attachments/assets/f9be95de-6fde-49b6-adf8-ece6c9f08d89)

Per l'installazione di wow invece il consiglio è di installarlo in un percorso semplice fuori dalla cartella di default

Esempio: "C:\Giochi\World of Warcraft" oppure "D:\World of Warcraft"

ATTENZIONE!

Battle.net e WoW supportano solo file system NTFS, se usate hard disk esterni e volete che wow sia installato su di essi, assicuratevi che il file system sia NTFS o il gioco non si aggiorna o da problemi di aggiornamenti infiniti

## WoW-Settings

Le impostazioni di wow spiegate e consigliate punto per punto sia per open world sia per raid

Monitor: Scegliete il monitor su cui giocare

Visualizzazione: Lasciate schermo intero (in finestra)

Risoluzione: Mettete quella massima pari al vostro monitor

Scala Rendering: Lasciate 100%

ATTENZIONE! attualmente è buggata quindi qualsiasi valore diverso da 100% provoca cali enormi di fps, un altra feature intelligente rotta da piu di 1 espansione...

Attiva dimensione intefaccia: è lo scaling ui, se usate elvui o altri addons non toccatelo se usate l'interfaccia blizzard scegliete a vostro piacimento

Sincronia Verticale (Vsync): Di Base Disattivato, utilizzatelo solo ed esclusivamente se avete problemi di tearing, ossia vi sembra che l'immagine si spacchi orizzontalmente, quando è attivo aumenta leggermente la latenza e blocca gli fps alla risoluzione dello schermo e ai suoi sottomultipli (migliorabili con triplo buffering vedi sotto)

Modalita a Bassa Latenza: se avete una gpu AMD lasciatelo disattivato, non porta benefici. Se avete una gpu Nvidia usate l'opzione nvidia reflex (NON reflex+boost che provoca tearing e fps minori) 

Anti-Aliasing: se avete schermi superiori al 2k usate solo tecniche basate su immagini con cmaa2, se usate obs usate il cmaa base. Se avete monitor fullHD usate una combinazione di cmaa2 e msaa 2x.
Se dovete raidare al massimo disattivatelo

Multisample alpha test: usatelo SOLO se usate tecnice multisample 

Campo Visivo Visuale: Lasciare al Massimo

![g1](https://github.com/user-attachments/assets/49bf2d7f-fe40-4db5-8060-ca37b8b3d72a)

ATTENZIONE! La sezione Incursioni e campi di battaglia attualmente è non funzionante (o meglio va e non va quando preferisce), quindi cambiate le impostazioni solo nella schermate base ogni volta... GG blizzard davvero...

Ignorate lo Slide da 1 a 10 Non serve a nulla

Qualità ombre: se  raidate usate bassa/low, di base non andate oltre Alto/High, non porta nessun vantaggio visivo visibile

Dettagli dei liquidi: se raidate usate bassa/low, di base non oltre Buona/Good in quanto ad alto spacca gli fps senza un notevole miglioramento

Densità delle Particelle: in qualunque situazione usate Alta/High, serve per vedere con maggiore dettaglio spell personali e delle fight

SSAO: in raid disattivato, normalmente Buona/Good, al limite alto/high

Effetti di profondità: in raid disattivato, normalmente Buona/Good, al limite High

Effetti di calcolo: in raid disattivato, normalmeno Buona/Good, pesa molto sugli fps oltre questa soglia (sono le nebbie e le aree nebbiose sfocate, di grande impatto ma pesante)

Modalità Contorno: sempre Alto/High

Risoluzione Texture: sempre Alto/High salvo pc vecchiotti

Densità magica: sempre Essenziali/Essenzial filtra le spell facendo vedere solo le nostre, quelle delle fight e le principali dei compagni

Proiezione Texture: IMPORTANTE sempre ON o non vedrete le spell dei boss

Distanza Visuale: in raid 1, altrimenti 7

Dettaglio Ambientale: in raid 1, altrimenti 7

Effetti del suolo: in raid 1, altrimenti 7

![g2](https://github.com/user-attachments/assets/4877cb92-ed80-407f-aa00-8c3516265127)

Buffering Triplo: Usarlo solo se si usa la Sincronia Verticale Sopra, altrimenti disattivare

Filtro Texture: Usare 16X, su pc vecchiotti 8X

Ray Tracing delle ombre: LOL togliete sta inutilità

Ricampionamento: lasciare fidelityFX (anche su Nvidia)

Modalità VRS: Disattivato

API grafiche: Usate DX12, se avete schede video super vecchie e avete problemi provate le DX11

Interazioni fisiche: Scegliete voi

Scheda Video: se usate un notebook o un processore con gpu integrata controllate di avere la scheda discreta dedicata giusta

FPS massimi primo piano: Settatelo alla pari del monitor, se usate Vsync potete disattivarlo

FPS massimi background: Usate un normale 30 ATTENZIONE! per alcuni utenti che hanno freeze quando eseguono ALT+TAB disattivate questa opzione o provate i fix nella sezione fix in fondo

Soglia FPS: Disattivato

Ricampionamento Nitidezza: ATTENZIONE! per poterne sfruttare i vantaggi dato che è buggata l'attivazione, usate questo comando

``` /console set ResampleAlwaysSharpen 1 ```

Poi Scegliete voi a piacere i livelli restanti

![g3](https://github.com/user-attachments/assets/aefabb67-5ede-482d-8b01-8b3476798452)

Nella sezione audio Disattivate Riverbero, attualmente buggato carica esageratamente la cpu, e impostate i canali audio a 128 e dimensione grande 128, questo permette ai suoni di addon e wa di sovrapporsi e non cancellarsi

![a1](https://github.com/user-attachments/assets/2ed0e714-7b95-4354-9e71-7d70aef52cea)

Nella sezione rete se non siete voi a prendere i log disattivate cronologia di combattimento avanzata, o vi crea i file log e aumenta il carico in raid sulla cpu

![r1](https://github.com/user-attachments/assets/e7515cda-64e5-4aa2-9243-af8218453884)



















