# 🪟 Windows Fundamentals Series (I, II, III)

In questa sezione ho raccolto le competenze acquisite durante il percorso di studio sui sistemi operativi Windows, partendo dalle basi fino alla gestione avanzata della sicurezza.

---

## 📂 Windows Fundamentals 1: Le Basi del Sistema
*Focus sull'interfaccia utente e le impostazioni principali.*

- **Desktop & File System:** Gestione delle cartelle, permessi di base e navigazione.
- **Task Manager:** Monitoraggio dei processi e gestione delle applicazioni bloccate.
- **Control Panel vs Settings:** Differenze tra la gestione classica e la nuova interfaccia di Windows.

---

## 📂 Windows Fundamentals 2: Amministrazione del Sistema
*Focus sugli strumenti di gestione e configurazione.*

- **System Information:** Visualizzazione dettagliata dell'hardware e del software installato.
- **Computer Management:** Gestione dei dischi, degli utenti e dei gruppi locali.
- **Command Prompt (CMD):** Utilizzo dei comandi base (`dir`, `cd`, `ipconfig`, `systeminfo`).
- **Registry Editor:** Basi del Registro di Sistema e come vengono salvate le configurazioni.

---

## 📂 Windows Fundamentals 3: Sicurezza e Analisi
*Focus sulla protezione del sistema e il monitoraggio.*

- **Windows Firewall:**
  - **Public Profile:** Utilizzato per reti non sicure (es. aeroporti). Disabilita il Network Discovery.
  - **Private/Domain Profile:** Profili per ambienti fidati.
- **BitLocker & TPM:**
  - Utilizzo del chip **TPM** per la crittografia.
  - In assenza di TPM (1.2+), necessità di una **Startup Key** (file `.bek`) su drive USB rimovibile.
- **Event Viewer:** Analisi dei log di sistema (Security, System, Application) per il monitoraggio degli accessi.
- **MSConfig:** Gestione avanzata dell'avvio e della modalità provvisoria.

---

## 🛠️ Strumenti Rapidi (Cheatsheet)
| Strumento | Comando (Win+R) | Scopo |
| :--- | :--- | :--- |
| **Event Viewer** | `eventvwr.msc` | Analisi Log e Errori |
| **System Config** | `msconfig` | Gestione Boot e Servizi |
| **Regedit** | `regedit` | Modifica Registro |
| **Services** | `services.msc` | Gestione Servizi in background |
| **Resource Monitor**| `resmon` | Analisi performance in tempo reale |

---
*Note e Laboratori completati nel percorso SOC Level 1 di TryHackMe.*
