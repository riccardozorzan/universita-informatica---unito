# Codifica dei Caratteri

Ogni carattere che leggi sullo schermo è, per il computer, un **numero**. La codifica è la convenzione che associa carattere ↔ numero.

---

## Perché serve una codifica?

La tastiera produce solo numeri (i tasti sono numerati). Serve un accordo condiviso: il numero 65 significa `A` per tutti i produttori. Senza un accordo comune, un file scritto su un computer sarebbe illeggibile su un altro.

---

## ASCII

**American Standard Code for Information Interchange** (1963). Ogni carattere occupa **1 byte**, valori da 0 a 127.

- 0-31 → caratteri di **controllo** (invio a capo, tabulazione, backspace)
- 32-126 → caratteri **stampabili** (spazio, cifre, lettere, punteggiatura)
- 127 → carattere di cancellazione (DEL)

### I valori da ricordare a memoria

| Codice | Carattere | Codice | Carattere |
|---|---|---|---|
| 32 | spazio | 65-90 | A-Z |
| 48-57 | 0-9 | 97-122 | a-z |
| 10 | Invio (a capo) | 9 | Tab |
| 13 | Ritorno carrello | 0 | Null |

> 💡 **Le cifre sono consecutive!** `'0'` = 48, `'1'` = 49 … `'9'` = 57. Perciò `'7' - '0'` in C vale esattamente 7: la differenza tra due caratteri consecutivi è 1.

---

## Limiti di ASCII

- Solo **128 caratteri** → niente accented Italian (`è`, `à`, `ò`), niente `€`, `→`, emoji.
- I primi 128 codici erano **standardizzati**, i successivi no: ogni costruttore li usava a modo proprio (codifiche proprietarie: **Codepage** su Windows, ISO-8859-1 su Unix).
- Risultato: lo stesso byte poteva significare `é` su un sistema e `Æ` su un altro. Problema serio per lo scambio di file e i siti web.

---

## EBCDIC

Usata dai **mainframe IBM** (storicamente). Anche 256 caratteri, ma con una peculiarità: le cifre `0-9` **non sono consecutive** (0xF0-0xF9) e le lettere minuscole stanno **prima** delle maiuscole. È il motivo per cui il C ha il "problema dei caratteri" sulle vecchie macchine IBM.

---

## Unicode: la soluzione moderna

**Unicode** assigns un unico codice a ogni carattere di tutte le lingue del mondo: latino, greco, arabo, cinese, giapponese, coreano, emoji, simboli matematici.

- Oltre **1,1 milioni** di punti di codice definiti (alfabeto con codice fino a 0x10FFFF)
- Assegnati dal consorzio **Unicode Consortium**
- Non è una codifica: è uno **standard di caratteri**. La codifica è il modo di tradurlo in byte.

---

## UTF-8: la codifica più diffusa

UTF-8 usa da 1 a 4 byte per carattere, in base al punto di codice. È lo standard di default di internet e di Linux.

| Byte | Intervallo | Cosa contiene |
|---|---|---|
| **1** | 0x00 - 0x7F | ASCII (identico, retrocompatibile) |
| **2** | 0x80 - 0x7FF | Latino esteso, greco, ebraico, arabo |
| **3** | 0x800 - 0xFFFF | Alfabeti non latini, CJK, punteggiatura |
| **4** | 0x10000 - 0x10FFFF | Emoji e simboli supplementari |

> ⚠️ **Attenzione — UTF-8 non è a lunghezza fissa:** la lettera `a` occupa 1 byte, `è` ne occupa 2, un'emoji 4. Quindi **non puoi assumere che un carattere = un byte**: funzioni come `strlen` o l'indicizzazione di stringhe in C restituiscono un numero che **non** è il numero di caratteri visibili. Per questo esiste `wchar_t` e in C++ le stringhe UTF-8.

---

## Esempio: perché un file "rotto"?

Il testo `caffè` scritto correttamente in UTF-8 è:

| Carattere | Punto di codice | Byte UTF-8 |
|---|---|---|
| c | U+0063 | 1 byte: `63` |
| a | U+0061 | 1 byte: `61` |
| f | U+0066 | 1 byte: `66` |
| f | U+0066 | 1 byte: `66` |
| è | U+00E8 | 2 byte: `C3 A8` |

Sono **6 byte** per 5 caratteri.

Se quel file viene aperto con una codifica diversa (es. Latin-1), i due byte `C3 A8` vengono letti come due caratteri diversi (`Ã¨`) e si vede **caffÃ¨**. Non è un bug: è una decodifica con la codifica sbagliata.

---

## BOM (Byte Order Mark)

Alcuni editor (in particolare quelli Windows per UTF-16) inseriscono a inizio file dei byte invisibili che segnalano la codifica. Sono spesso la causa di strani caratteri all'inizio di un file o di fallimenti in compilazione.

---

## Esempi contesto informatico

- **Sorgenti C/C++**: salvati in UTF-8, altrimenti `printf("caffè")` stampa roba illeggibile.
- **Database**: MySQL ha `utf8mb4` come charset raccomandato (`utf8` storicamente copriva solo 3 byte, quindi le emoji erano tagliate).
- **HTTP**: l'header `Content-Type: text/html; charset=UTF-8` dice al browser come interpretare i byte ricevuti.
- **File di testo**: un `.txt` salvato in UTF-8 e aperto in un editor impostato su Latin-1 mostra caratteri accentati sbagliati.

---

## Riepilogo

| Codifica | Byte per carattere | Caratteri | Note |
|---|---|---|---|
| ASCII | 1 | 128 | Solo americano, senza accenti |
| EBCDIC | 1 | 256 | Mainframe IBM, ordinamento strano |
| Latin-1 | 1 | 256 | Estensione europea di ASCII, incompatibile |
| UTF-8 | 1-4 | Tutti | Standard attuale di internet e Linux |
| UTF-16 | 2 | Circa 65.000 | Usata da Windows, con BOM |

- ASCII: i caratteri `'0'`-`'9'` differiscono di 1 nel codice
- Unicode è lo standard dei caratteri, UTF-8 è la sua codifica più comune
- **Codifica diverse producono testo diverso dagli stessi byte** → disallineamento

---

## Link

- [[Programma - Fondamenti dell'Informatica]] — il programma di questo corso
- [[Sistemi di Numerazione]] — i byte sono numeri in base 2
- [[Programma - Architettura degli Elaboratori]] — perché servono codifiche standard
- [[Programma - Programmazione I]] — `char`, stringhe in C e problemi di encoding
