# Guida all'aggiornamento firmware del modulo

Per semplicità di spiegazione le immagini sono riferite a Windows, 
ma per Linux o Mac OSX il procedimento è analogo.

E' più semplice programmare il modulo utilizzando un normale convertitore "FTDI" a 6 pin 5V, ma
è possibile usare anche un semplice convertitore USB/Seriale collegando solo RX, TX e massa, ma 
bisognerà accendere il modulo appena dopo aver premuto il pulsante di programmazione, dato che 
il convertitore non sarà in grado di generare il segnale di reset.


Scaricare e installare l’ultima versione del software IDE Arduino dal sito:
https://www.arduino.cc/en/Main/Software


Scaricare ed estrarre dal .zip l’ultima release del firmware del modulo dal sito:
https://github.com/MikyM0use/JAFaR/releases

<p align="center">
<img src="/docs/directory_struct.png" width="50%" height="50%" />
</p>

aprire il file "arduino\_sketch.ino" dentro alla cartella arduino\_sketch.

<p align="center">
<img src="/docs/arduino_files.jpg" width="50%" height="50%" />
</p>

Se è la prima volta che si aggiorna il modulo, bisognerà installare le librerie:

<p align="center">
<img src="/docs/installa_zip.jpg" width="50%" height="50%" />
</p>

selezionare poi le tre cartelle (ripetendo il procedimento tre volte) contenute nella directory /libs
del file scaricato ed estratto da Github.

<p align="center">
<img src="/docs/installa_libs.jpg" width="50%" height="50%" />
</p>

a questo punto selezionare il corretto tipo di board (Arduino pro o pro mini) e la porta (che dipende 
dal sistema operativo, *controllare che la porta sia corretta*)

<p align="center">
<img src="/docs/board_e_porta.jpg" width="50%" height="50%" />
</p>

effettuare le eventuali modifiche al software, poi collegare il modulo al convertitore FTDI (i
nomi dei pin sono scritti direttamente sul modulo, basta allineare i pin con il convertitore FTDI).

a questo punto premere il pulsante "carica" sull'IDE arduino e attendere il messaggio di "caricamento completato"

<p align="center">
<img src="/docs/scarica.jpg" width="50%" height="50%" />
</p>
