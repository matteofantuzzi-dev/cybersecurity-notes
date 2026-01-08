# 🔐 Cryptography Basics

In questa sezione ho documentato i principi fondamentali della crittografia, dalle tecniche classiche ai moderni algoritmi di cifratura asimmetrica e hashing. La crittografia è il cuore della protezione dei dati (Confidenzialità e Integrità).

---

## 🏛️ 1. Crittografia Classica
Ho analizzato i primi metodi di cifratura basati sulla sostituzione.
* **Cifrario di Cesare:** Un algoritmo che sposta le lettere dell'alfabeto di un numero fisso di posizioni (Key Shift).
* **Vulnerabilità:** Facile da rompere tramite **analisi delle frequenze** o attacchi di **brute force** sulle 25 rotazioni possibili.

---

## 🔢 2. Matematica per la Crittografia
La crittografia moderna si basa su operazioni matematiche binarie e modulari.

### Operazione XOR (Exclusive OR) ⊕
Lo XOR è fondamentale perché è un'operazione reversibile utilizzata per "mescolare" i dati con una chiave.
* **Esercizio:** `1001 ⊕ 1010 = 0011`
* **Logica:** Restituisce `1` solo se i bit sono diversi.

### Aritmetica Modulare (%)
Chiamata "matematica dell'orologio", restituisce il resto di una divisione. È il motore di algoritmi come RSA.
* **Esempio 1:** `118613842 % 9091 = 3565`
* **Esempio 2:** `60 % 12 = 0` (Indica che il numero è perfettamente divisibile).

---

## 🛡️ 3. Cifratura Moderna: Simmetrica vs Asimmetrica

### Cifratura Simmetrica
Utilizza una **singola chiave** per cifrare e decifrare.
* **Pro:** Estremamente veloce.
* **Contro:** Difficoltà nel distribuire la chiave in modo sicuro.
* **Esempi:** AES (Advanced Encryption Standard).

### Cifratura Asimmetrica
Utilizza una coppia di chiavi: una **Chiave Pubblica** (per cifrare) e una **Chiave Privata** (per decifrare).
* **Pro:** Risolve il problema dello scambio delle chiavi.
* **Esempi:** RSA, Diffie-Hellman.

---

## 🧩 4. Hashing vs Encoding
È fondamentale distinguere tra queste due tecniche spesso confuse:

1. **Encoding (es. Base64):** NON è crittografia. Serve a cambiare il formato dei dati per la trasmissione. È facilmente reversibile.
2. **Hashing (es. SHA-256, MD5):** Una funzione a senso unico che crea un'impronta digitale fissa di un dato. Usata per verificare l'integrità (assicurarsi che un file non sia stato alterato).

---

## 🛠️ Strumenti Utilizzati
* **CyberChef:** Il "coltellino svizzero" della crittografia per manipolare dati, encoding e cifrari.
* **Calcolatrici Modulari:** Per la risoluzione di algoritmi basati sul resto.

---
*Note: Note prese durante il completamento della room Cryptography Basics su TryHackMe.*
