# WOS ---Work In Proress---
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
Salve mi chiamo Matteo, online sono Itanku, Monk Brewmaster. Ho voluto finalmente raccogliere tutte le informazione e le esperienze che conosco per migliorare ed ottimizzare World of Warcraft al meglio, in particolare per l'ambiente raid, m+ e competitivo in generale.

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

