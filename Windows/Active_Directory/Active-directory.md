# 🏛️ Active Directory (AD) Fundamentals

In questa sezione ho documentato l'apprendimento dei concetti base di Active Directory attraverso i laboratori di TryHackMe. Active Directory è il servizio di directory di Microsoft utilizzato per la gestione centralizzata di utenti, computer e risorse all'interno di una rete aziendale.

## 🔑 Concetti Chiave Appresi

### 1. La Gerarchia di AD
Ho esplorato la struttura logica che permette di scalare la rete da pochi utenti a migliaia di dispositivi:
* **Forest (Foresta):** Il confine di sicurezza più esterno. Contiene tutti gli alberi e i domini.
* **Tree (Albero):** Un insieme di domini che condividono una radice DNS comune.
* **Domain (Dominio):** L'unità amministrativa principale dove risiedono oggetti come utenti e computer.
* **OU (Organizational Unit):** Contenitori logici usati per organizzare gli oggetti e delegare i permessi.


 
### 2. Gestione degli Utenti e Privilegi
Durante l'analisi dell'utente `Sophie`, ho compreso l'importanza della gestione degli account privilegiati:
* **Domain Admins:** Account con controllo totale sul Domain Controller. La loro protezione è la priorità numero uno per la cybersecurity.
* **Enumerazione:** Identificare i membri di gruppi privilegiati è un passaggio critico nella fase di ricognizione di un attacco.

### 3. Amministrazione e Sicurezza
* **Delegation (Delegazione):** Il processo di assegnazione di permessi specifici su una OU a utenti non amministratori. Segue il **Principio del Minimo Privilegio (PoLP)**.
* **GPO (Group Policy Objects):** Strumenti utilizzati per applicare impostazioni di sicurezza e configurazioni in modo centralizzato a gruppi di utenti o computer.
* **SYSVOL:** Una condivisione di rete speciale presente su tutti i Domain Controller, utilizzata per distribuire i file delle GPO e gli script di logon a tutta la rete.



### 4. Protocolli di Autenticazione: Kerberos
Ho approfondito il funzionamento di Kerberos, il protocollo di default in AD, che si basa su un sistema di "Ticket":
1.  **TGT (Ticket Granting Ticket):** Ottenuto dopo il login iniziale.
2.  **TGS (Ticket Granting Service):** Richiesto per accedere a una risorsa specifica senza reinserire la password.
*Questo sistema evita il passaggio di password in chiaro sulla rete, migliorando drasticamente la sicurezza rispetto al vecchio NTLM.*



---
*Note: Note: Questi appunti sono stati presi durante il completamento della stanza "Active Directory Basics" su TryHackMe.*
