# Alcuni esperimenti con Raspberry Pi, una TV e un account Netflix.

Almeno il 95% deriva da istruzioni di qualcun altro, che ha risolto i problemi prima di me.
Io ho provato. 

Per due motivi:

- divertirmi a fare questi esperimenti,
- verificare se posso realizzare un dispositivo utilizzabile quotidianamente.

Quello che segue sono appunti sui passi che ho seguito.

## Procurarsi il materiale

- Raspberry Pi 3 B+
- **FONDAMENTALE** un alimentatore fidato; io ho scelto l'Alimentatore ufficiale per RPI 3 (5.1 V, 2.5 A) 
- **FONDAMENTALE** scheda di memoria microSD Sandisk Ultra, Categoria Performance A1. Per maggiori informazioni per scegliere la scheda SD rimando a un [capitolo di armbian user guide](https://docs.armbian.com/User-Guide_Getting-Started/#how-to-prepare-a-sd-card).
- TV dotata di entrata HDMI (e telecomando)
- un cavo HDMI/HDMI
- Un laptop (così posso usarlo vicino alla TV).
- Una tastiera e un mouse USB (nel mio caso wireless)
- una chiavetta USB di memoria

## scegliere e procurarsi il software

Ho deciso che il dispositivo doveva servire solo come media center, che non mi interessava usarlo come desktop.

Quindi ho scelto KODI come software per media center, che fornisce una interfaccia a tutti i vari sottosistemi necessari.

Ho scelto di far girare KODI su una distribuzione Linux minimale, che fornisce le necessarie risorse a KODI per funzionare.

Tra varie possibilità, ho scelto la distribuzione [LibreELEC](https://libreelec.tv/downloads_new/raspberry-pi-3-3/) e ho scaricato l'immagine del sistema operativo.

## Creare la SD avviabile

Per trasferire l'immagine della distro sulla scheda SD ho usato [Etcher](https://www.balena.io/etcher/).

## Primo setup

- inserisco la scheda SD nel RPI
- collego RPI alla TV (HDMI #1) con un cavo DHMI
- accendo la TV e imposto HDMI #1 come input video
- collego mouse e tastiera a RPI
- inserisco l'alimentatore nella presa 230V
- collego l'alimentatore al RPI
- Dopo un po' ho un sistema linux con interfaccia Kodi funzionante.
- mi collego al Wi-fi di casa (o alla ethernet)

## usare Netflix

- Sul laptop scarico l'add-on, ossia il componente aggiuntivo, per vedere Netflix su Kodi; la versione che ho utilizzato è [quella di Stefano Gottardo](https://github.com/CastagnaIT/repository.castagnait).
- Copio lo zip in questione sulla chiavetta USB.
- metto la chiavetta nel RPI
- Ordino a Kodi di permettere l'installazione di add-ons di terze parti `Settings > System > Add-ons > Unknown sources`.
- Installo l'add-on `Add-ons > Install from zip file > nome-del-file.zip`; verrà richiesto di installare altri add-ons, accetto.
- Adesso tra i miei Addons trovo Netflix
- inserisco le credenziali dell'account Netflix (grazie Sam!)
- al primo accesso, verrà richiesto di installare dell'altro software, accetto.
- Netflix (per adesso) funzionante!


