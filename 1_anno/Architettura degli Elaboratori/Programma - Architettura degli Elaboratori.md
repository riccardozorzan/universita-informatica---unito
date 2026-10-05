> [!info] Programma ufficiale del corso
> Le note di studio sono in [[Indice - Architettura degli Elaboratori]] · la mappa di tutti i corsi è in [[Indice generale]]

# Guida allo Studio: Architettura degli Elaboratori (6 CFU)

**Corso di Laurea in Informatica — Università degli Studi di Torino**

---

## 1. Informazioni Generali sull'Insegnamento

* **Codice Attività Didattica:** INF0326
* **Settore Scientifico-Disciplinare (SSD):** INF/01 (Informatica)
* **Crediti Formativi Universitari (CFU):** 6 CFU
  * **Teoria:** 4 CFU (32 ore di lezione frontale in aula)
  * **Laboratorio:** 2 CFU (20 ore di esercitazioni guidate al computer)
* **Anno di Corso e Semestre:** 1° Anno, 2° Semestre
* **Tipologia Insegnamento:** Caratterizzante
* **Lingua di Erogazione:** Italiano (English-Friendly Course)
* **Frequenza:** Facoltativa (ma fortemente consigliata, specialmente per il laboratorio)
* **Insegnamenti Propedeutici (Prerequisiti):**
  * *Programmazione I e Laboratorio* (1° semestre)
  * *Fondamenti dell'Informatica* (1° semestre)
  * Si richiede la conoscenza dei concetti fondamentali della programmazione imperativa e la capacità di progettare semplici algoritmi.

### Informazioni operative (a.a. 2026/2027)

* **Prima lezione:** la lezione introduttiva è in programma per **febbraio 2027** (2° semestre).
* **Canali e turni:** il corso è articolato su **tre canali (A, B, C)** con orari pubblicati sull'agenda UniTO. L'appartenenza al **turno T1 o T2** dipende dall'**ultima cifra del numero di matricola**:

  | Ultima cifra della matricola | Turno |
  |---|---|
  | **pari** | **T2** |
  | **dispari** | **T1** |

  Esempio: matricola `986734` → ultima cifra `4` (pari) → **T2**.

* **Corsi A, B e C:** il programma svolto è **lo stesso** per i tre corsi e anche le **modalità d'esame sono le stesse**, illustrate durante il corso. In ogni caso i compiti degli studenti del corso X vengono esaminati dai docenti del corso X.
* **Valutazione del corso obbligatoria:** alla fine del corso sei tenuto a dare una tua valutazione del corso — **senza di essa non è consentita l'iscrizione all'esame**.

---

## 2. Obiettivi Formativi e Risultati di Apprendimento

L'insegnamento ha lo scopo di fornire agli studenti la comprensione dell'organizzazione hardware dei calcolatori digitali, strutturata attraverso la nozione di gerarchia di macchine virtuali, e delle interfacce tra hardware e software di sistema.

### Competenze Acquisite:
1. **Conoscenza e Comprensione:**
   * Comprendere le relazioni tra linguaggi ad alto livello (es. C, Java) e il linguaggio macchina sottostante.
   * Riconoscere le fasi di traduzione, assemblaggio, collegamento (*linking*) e caricamento (*loading*) dei programmi.
   * Analizzare la struttura interna dei componenti digitali di un processore moderno e della gerarchia delle memorie.
2. **Capacità di Applicare Conoscenza e Comprensione:**
   * Progettare e sviluppare programmi in linguaggio assemblativo utilizzando lo standard **RISC-V**.
3. **Autonomia di Giudizio e Abilità Comunicative:**
   * Valutare l'impatto delle caratteristiche hardware sulle prestazioni del software.
   * Esprimere con linguaggio tecnico appropriato le dinamiche del funzionamento interno di un elaboratore.

---

## 3. Programma Dettagliato dell'Insegnamento

### A. Modulo di Teoria (4 CFU - 32 Ore)

1. **Calcolatori: Astrazioni e Tecnologia:**
   * Concetto di macchina virtuale, astrazione e modelli di prestazione.
   * Legge di Moore, legge di Amdahl, consumo energetico e transizione ai sistemi multicore.
2. **Instruction Set Architecture (ISA) RISC-V:**
   * Principi di progettazione delle ISA RISC (regolarità, semplicità, compromessi di progetto).
   * Operandi dell'hardware: registri di uso generale (`x0-x31`), memoria principale, indirizzamento al byte, allineamento e convenzione *Little-Endian*.
   * Rappresentazione delle istruzioni e formati macchina RISC-V (Tipo R, Tipo I, Tipo S, Tipo SB, Tipo U, Tipo UJ).
   * Aritmetica in virgola mobile nello standard IEEE 754 e relative istruzioni RISC-V.
   * Catena di traduzione ed esecuzione: Compilatore, Assembler, Linker e Loader.
3. **Il Processore RISC-V:**
   * Architettura della CPU: Unità di Elaborazione (*Datapath*) e Unità di Controllo.
   * Realizzazione dell'Unità Aritmetico-Logica (ALU) e gestione dei registri.
   * Metodologia di temporizzazione e ciclo di clock.
   * Schema di implementazione a singolo ciclo e introduzione ai concetti di *pipelining* e *hazard* (strutturali, sui dati, sul controllo).
4. **Bus e Sistema di Input/Output (I/O):**
   * Tipi di bus, struttura delle connessioni e meccanismi di arbitraggio.
   * I/O programmato mediante attesa attiva (*busy waiting / polling*).
   * I/O guidato dalle interruzioni (*interrupt*) e meccanismo di eccezione nel RISC-V.
   * Accesso Diretto alla Memoria (*Direct Memory Access - DMA*).
5. **Gerarchia delle Memorie e Cache:**
   * Principi di località spaziale e temporale.
   * Tecnologie di memoria: SRAM vs DRAM.
   * Organizzazione e funzionamento delle memorie Cache (mappatura diretta, associativa a blocchi, set-associativa).
   * Politiche di rimpiazzo e di scrittura (*write-through*, *write-back*) e calcolo delle prestazioni (Miss Rate, Hit Time, Miss Penalty).

---

### B. Modulo di Laboratorio (2 CFU - 20 Ore)

1. **Linguaggio Assemblativo RISC-V:**
   * Sintassi dell'assembly RISC-V, direttive dell'assembler e pseudo-istruzioni (`li`, `mv`, `la`, ecc.).
   * Operazioni aritmetico-logiche (`add`, `sub`, `addi`, `and`, `or`, `xor`, `sll`, `srl`, `sra`).
2. **Controllo del Flusso ed Esecuzione Condizionale:**
   * Salti condizionati (`beq`, `bne`, `blt`, `bge`, `bltu`, `bgeu`) per la traduzione di costrutti `if-then-else`, cicli `while` e `for`.
   * Salti incondizionati e indiretti (`j`, `jal`, `jalr`).
3. **Supporto Hardware alle Procedure e Gestione della Memoria:**
   * Convenzioni dei registri RISC-V: registri temporanei (`x5-x7`, `x28-x31`), registri da preservare (`x8-x9`, `x18-x27`), registri argomento (`x10-x17`), registro di ritorno `ra` (`x1`).
   * Gestione dello **Stack**: *Stack Pointer* (`sp` / `x2`), allocazione e deallocazione dei frame di attivazione (*record di attivazione*).
   * Chiamate a procedura foglia e non-foglia (ricorsione).
4. **Strumenti Pratici:**
   * Uso di compilatori, simulatori e debugger dell'architettura RISC-V (es. RARS / MARS o ambienti simulati di laboratorio).

---

## 4. Modalità d'Esame e Valutazione

> ⚠️ **Prerequisito per l'iscrizione:** non puoi iscriverti all'esame se non hai prima completato la **valutazione del corso** (vedi §1 — Informazioni operative). È l'unico prerequisito "amministrativo", oltre ai requisiti di crediti.

Le modalità sono **le stesse per i corsi A, B e C** e vengono illustrate durante il corso.

L'esame consiste in una prova scritta e in una prova orale obbligatoria, valutate in trentesimi (con eventuale lode).

### Struttura della Prova d'Esame:
1. **Prova di Ammissione (Sbarramento - 10 punti):**
   * Test a risposta chiusa o aperta svolto al computer per verificare le competenze elementari di base. Il superamento è necessario per accedere alle parti successive.
2. **Prova di Teoria (14 punti):**
   * Domande a risposta aperta o a scelta multipla sugli argomenti del corso di teoria (architettura della CPU, memorie cache, bus, I/O, traduzione di codice).
3. **Prova di Laboratorio (8 punti):**
   * Esercizio pratico di programmazione in linguaggio assemblativo RISC-V svolto in laboratorio con l'ausilio di simulatori/compilatori. Viene valutata la correttezza sintattica ed algoritmica del codice sottomesso.

Tutte le parti contribuiscono al voto finale e devono risultare sufficienti.

---

## 5. Testi Consigliati e Materiale Didattico

* **Testo di Riferimento Ufficiale:**
  * David A. Patterson, John L. Hennessy, *Struttura e progetto dei calcolatori - Progettare con RISC-V*, 2ª edizione italiana (a cura di A. Borghese), Zanichelli, 2023.
* **Materiale Integrativo:**
  * Slide ufficiali delle lezioni e dispense di laboratorio pubblicate sulla piattaforma **Moodle / Campusnet** di UniTO.
