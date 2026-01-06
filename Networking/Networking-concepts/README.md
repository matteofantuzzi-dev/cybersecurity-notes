# 🌐 Guida Approfondita ai Networking Concepts

Questo repository documenta l'analisi tecnica dei protocolli di rete e dei modelli di comunicazione studiati tramite TryHackMe. La comprensione del networking è il prerequisito fondamentale per il Penetration Testing e la Network Forensics.

---

## 🏗️ 1. Il Modello OSI (Open Systems Interconnection)
Il modello OSI è un framework concettuale in 7 livelli che standardizza le funzioni di un sistema di comunicazione.

| Livello | Nome | Funzione Principale | Protocolli/Hardware |
| :--- | :--- | :--- | :--- |
| **7** | **Application** | Interfaccia utente e servizi di rete. | HTTP, FTP, Telnet, SSH, DNS |
| **6** | **Presentation** | Traduzione, cifratura e compressione dati. | SSL/TLS, JPEG, GIF |
| **5** | **Session** | Gestione delle sessioni di comunicazione. | NetBIOS, RPC |
| **4** | **Transport** | Trasferimento dati end-to-end e controllo errori. | TCP, UDP |
| **3** | **Network** | Instradamento dei pacchetti e indirizzamento logico. | IP, ICMP, Router |
| **2** | **Data Link** | Trasferimento dati tra nodi adiacenti (fisico). | Ethernet, MAC, Switch |
| **1** | **Physical** | Trasmissione di bit grezzi su mezzi fisici. | Cavi, Hub, Ripetitori |



---

## 📍 2. Indirizzamento IP (IPv4)
L'indirizzo IP identifica univocamente un host su una rete.

### Anatomia di un indirizzo:
* **Struttura:** 32 bit divisi in 4 ottetti (es: `192.168.1.1`).
* **Range:** Ogni ottetto varia da `0` a `255`. Valori come `305` sono matematicamente impossibili poiché superano gli 8 bit ($2^8 = 256$ combinazioni).
* **Indirizzi Privati vs Pubblici:**
  - **Privati:** Usati all'interno di una LAN (es. `10.x.x.x`, `192.168.x.x`). Non sono instradabili su Internet.
  - **Pubblici:** Univoci a livello mondiale, assegnati dall'ISP.

---

## 🚪 3. Porte e Socket
Le porte permettono a un singolo indirizzo IP di gestire più servizi simultaneamente.

* **Totale Porte:** 65.535.
* **Well-known Ports (0-1023):**
  - **21 (FTP):** Trasferimento file.
  - **22 (SSH):** Accesso remoto sicuro (Criptato).
  - **23 (Telnet):** Accesso remoto insicuro (In chiaro).
  - **80 (HTTP):** Traffico web non criptato.
  - **443 (HTTPS):** Traffico web criptato tramite TLS/SSL.
* **Socket:** È la combinazione di `Indirizzo IP + Porta` (es: `192.168.1.10:80`).

---

## 🛠️ 4. Protocolli di Trasporto: TCP vs UDP
La scelta del protocollo di trasporto cambia radicalmente la natura della comunicazione.

### TCP (Transmission Control Protocol)
* **Connection-oriented:** Richiede il "Three-way Handshake" (SYN, SYN-ACK, ACK).
* **Affidabile:** Garantisce che i pacchetti arrivino e siano nell'ordine corretto.
* **Uso:** Web browsing, Email, Trasferimento file.

### UDP (User Datagram Protocol)
* **Connectionless:** Invia i dati senza verificare se il destinatario è pronto.
* **Veloce:** Nessun controllo di errore o riordinamento.
* **Uso:** Streaming video, Gaming online, VoIP, DNS.



---

## 📟 5. Analisi Pratica: Il Problema di Telnet
Durante il laboratorio, ho utilizzato **Telnet** per interagire con un server remoto.

**Security Takeaway:** Telnet è un protocollo "Clear-text". Durante i test ho osservato che:
1. Qualsiasi dato inviato (comandi, password) viaggia in chiaro.
2. Un utente malintenzionato può eseguire uno "Sniffing" del traffico tramite tool come **Wireshark** per rubare credenziali.
3. **Best Practice:** Disabilitare Telnet e migrare a **SSH** per ogni attività amministrativa.

---
*Note: Note: Documentazione creata durante lo studio del modulo Networking Concepts su TryHackMe.* cioè questo file dovrei fare?con tutto questo contenuto chiamandolo readme.md nella cartella networking concepts?
