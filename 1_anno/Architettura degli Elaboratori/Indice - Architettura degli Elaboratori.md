# Indice - Architettura degli Elaboratori

> [!info] Mappa del corso
> **Legenda:** ✅ scritto · 📄 da scrivere
> Programma ufficiale: [[Programma - Architettura degli Elaboratori]]

| | |
|---|---|
| **Codice** | INF0326 · SSD INF/01 |
| **Crediti** | 6 CFU · 52 ore (32 teoria + 20 laboratorio) |
| **Semestre** | 2° (1° anno) |
| **Prerequisiti** | [[Programma - Programmazione I]] e [[Programma - Fondamenti dell'Informatica]] |
| **Esame** | **Orale obbligatorio**. Ammissione 10 punti + teoria 14 punti + laboratorio 8 punti. Tutte le parti devono essere sufficienti |
| **Testo** | Patterson & Hennessy, *Struttura e progetto dei calcolatori - Progettare con RISC-V* (Zanichelli) |

> ⚠️ **Attenzione:** il corso è costruito interamente su **RISC-V**, non sull'architettura x86 e non sul modello di von Neumann classico. Studia la ISA RISC-V.

> 🔢 **Turno di laboratorio:** ultima cifra della matricola — **pari → T2**, **dispari → T1** (es. `986734` → `4` → T2). Prima lezione: **febbraio 2027**, canali A/B/C.

> 📝 **Prima di iscriverti all'esame** devi aver completato la **valutazione del corso** — è obbligatoria e senza di essa l'iscrizione non è consentita.

---

## Modulo A — Teoria

### A1. Calcolatori: astrazioni e tecnologia

| Argomento | Note |
|---|---|
| Macchina virtuale, astrazione, modelli di prestazione | 📄 [[Astrazione e Prestazioni]] |
| Legge di Moore, legge di Amdahl, sistemi multicore | 📄 [[Legge di Moore e di Amdahl]] |

### A2. Instruction Set Architecture RISC-V

| Argomento | Note |
|---|---|
| Principi di progettazione delle ISA RISC | 📄 [[Progettazione delle ISA RISC]] |
| Registri `x0`–`x31`, convenzioni | 📄 [[Registri RISC-V]] |
| Byte addressing, allineamento, Little-Endian | 📄 [[Allineamento e Little-Endian]] |
| Formati delle istruzioni: R, I, S, SB, U, UJ | 📄 [[Formati delle Istruzioni RISC-V]] |
| Virgola mobile IEEE 754 e istruzioni floating-point | 📄 [[IEEE 754 e RISC-V]] |
| Catena compilatore → assembler → linker → loader | 📄 [[Traduzione e Linking]] |

### A3. Il processore RISC-V

| Argomento | Note |
|---|---|
| Datapath e unità di controllo | 📄 [[Datapath RISC-V]] |
| ALU e gestione dei registri | 📄 [[ALU e Registri]] |
| Temporizzazione e ciclo di clock | 📄 [[Ciclo di Clock]] |
| Implementazione a singolo ciclo | 📄 [[Singolo Ciclo]] |
| Pipelining e hazard (strutturali, dati, controllo) | 📄 [[Pipeline e Hazard]] |

### A4. Bus e sistema di I/O

| Argomento | Note |
|---|---|
| Tipi di bus e arbitraggio | 📄 [[Bus e Arbitraggio]] |
| I/O programmato e busy waiting | 📄 [[IO Programmato]] |
| Interruzioni ed eccezioni RISC-V | 📄 [[Interruzioni]] |
| Direct Memory Access (DMA) | 📄 [[DMA]] |

### A5. Gerarchia delle memorie e cache

| Argomento | Note |
|---|---|
| Località spaziale e temporale | 📄 [[Località]] |
| SRAM vs DRAM | 📄 [[SRAM e DRAM]] |
| Cache: diretta, associativa, set-associativa | 📄 [[Cache]] |
| Politiche di scrittura e rimpiazzo | 📄 [[Politiche di Cache]] |
| Prestazioni: miss rate, hit time, miss penalty | 📄 [[Prestazioni delle Cache]] |

## Modulo B — Laboratorio

| Argomento | Note |
|---|---|
| Sintassi assembly RISC-V, direttive, pseudo-istruzioni | 📄 [[Assembly RISC-V Sintassi]] |
| Istruzioni aritmetico-logiche | 📄 [[Istruzioni Aritmetiche RISC-V]] |
| Salti condizionati e traduzione di if/while/for | 📄 [[Salti Condizionali]] |
| Salti incondizionati e indiretti: j, jal, jalr | 📄 [[Salti e Chiamate]] |
| Convenzioni dei registri e record di attivazione | 📄 [[Convenzioni dei Registri]] |
| Stack pointer, allocazione e deallocazione dei frame | 📄 [[Stack in Assembly]] |
| RARS / MARS e strumenti di simulazione | 📄 [[Simulatori RISC-V]] |

---

## Prerequisiti da ripassare

- Codifica dei dati: [[Programma - Fondamenti dell'Informatica]]
- Puntatori e stack in C: [[Programma - Programmazione I]]

## Collegamenti ad altri corsi

- [[Programma - Programmazione II]] — liste collegate e ADT, che qui realizzi in assembly
- [[Programma - Ricerca Operativa]] — algoritmi su grafi, connessa ai problemi su rete
