# 💻 Windows Command Line (CMD) Fundamentals

In questa sezione ho documentato la padronanza della riga di comando di Windows (Command Prompt). Saper operare senza interfaccia grafica è una competenza critica per la gestione dei sistemi e per le attività di Penetration Testing.

## 🔎 Informazioni di Sistema
Prima di operare su una macchina, è fondamentale capire con cosa si ha a che fare.
* `whoami`: Mostra l'utente corrente e il suo livello di privilegio.
* `hostname`: Visualizza il nome della macchina di rete.
* `ver`: Mostra la versione esatta del sistema operativo (es. Windows 10, Server 2019).
* `systeminfo`: Genera un report dettagliato su hardware, patch di sicurezza (Hotfix) e tempo di attività.

## 📂 Navigazione e Gestione File
I comandi principali per muoversi nel File System e manipolare i dati:
* `dir`: Elenca file e directory nella posizione corrente.
  - `dir /a`: Visualizza anche i file nascosti.
  - `dir /s`: Ricerca ricorsiva in tutte le sottocartelle.
* `cd [percorso]`: Cambia directory (es. `cd C:\Treasure\Hunt`).
  - `cd ..`: Torna alla cartella superiore.
* `type [file]`: Visualizza il contenuto di un file di testo (equivalente a `cat` su Linux).
* `mkdir [nome]`: Crea una nuova cartella.
* `ren [vecchio_nome] [nuovo_nome]`: Rinomina un file o una cartella.



## 🛠️ Esercizio Pratico: Treasure Hunt
Durante il laboratorio, ho messo in pratica queste competenze per localizzare asset nascosti:
1. Navigazione nel percorso: `C:\Treasure\Hunt`.
2. Identificazione del file tramite `dir`: il file è stato identificato come `flag.txt`.
3. Lettura del contenuto: tramite `type flag.txt`, recuperando la flag necessaria per la validazione.

## 🛡️ Cybersecurity Insight: Perché il CMD?
Dal punto di vista della sicurezza, la command line è fondamentale perché:
1. **Low Footprint:** Molti attacchi vengono eseguiti tramite shell per evitare di attivare avvisi legati all'interfaccia grafica.
2. **Automazione:** Permette di creare script (.bat) per eseguire scansioni rapide o raccogliere prove (forensics) in modo sistematico.
3. **Privilege Escalation:** Analizzare l'output di `systeminfo` permette di identificare vulnerabilità legate a patch mancanti.

---
*Note: Questi appunti sono stati presi durante il completamento della stanza "Windows Command Line" su TryHackMe.*
