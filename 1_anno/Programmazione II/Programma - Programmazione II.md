> [!info] Programma ufficiale del corso
> Le note di studio sono in [[Indice - Programmazione II]] · la mappa di tutti i corsi è in [[Indice generale]]

# Programmazione II - Guida Completa all'Insegnamento (UniTO)

* **Corso di Laurea:** Laurea Triennale in Informatica (L31) - Università degli Studi di Torino
* **Codice Attività Didattica:** INF0330 | **SSD:** INF/01 (Informatica)
* **Crediti:** 6 CFU (32 ore di lezione in aula + 20 ore di laboratorio)
* **Anno e Semestre:** 1° Anno, 2° Semestre
* **Tipologia:** Caratterizzante | **Frequenza:** Facoltativa

---

## 1. Descrizione e Obiettivi Formativi
L'insegnamento di **Programmazione II** prosegue e approfondisce il percorso di programmazione imperativa iniziato con *Programmazione I*. L'obiettivo principale è sviluppare la capacità di progettare e realizzare applicazioni di piccola e media complessità nel linguaggio **C**, gestendo in modo rigoroso la memoria dinamica e le strutture dati ricorsive.

Vengono introdotte le metodologie fondamentali dell'ingegneria del software (modularità su più file, sviluppo guidato dai test - TDD, invarianti di ciclo e gestione di casi eccezionali) unitamente a cenni di complessità computazionale in tempo e spazio.

---

## 2. Prerequisiti
Per affrontare con successo l'insegnamento è richiesta la padronanza dei concetti base della programmazione imperativa in C forniti da *Programmazione I*:
* Tipi di dato elementari, variabili e operatori.
* Strutture di controllo: condizionali (`if-else`, `switch`) ed iterative (`while`, `for`, `do-while`).
* Vettori (array monodimensionali e bidimensionali/matrici), stringhe e strutture (`struct`).
* Concetto di puntatore, algebra dei puntatori e passaggio dei parametri a funzione (per valore e per indirizzo).
* Astrazione procedurale e ricorsione elementare.
* Operazioni base di Input/Output (lettura da `stdin`, scrittura su `stdout`).

---

## 3. Programma e Argomenti Dettagliati

### Modulo 1: Ripasso e Lettura delle Specifiche
1. **Ripasso della programmazione imperativa in C:** Variabili, funzioni, passaggio parametri, array e puntatori.
2. **Lettura e analisi della consegna:** Identificazione degli input/output necessari, filtraggio dei dati non rilevanti, progettazione della soluzione algoritmica e strutturazione dell'output.

### Modulo 2: Gestione Esplicita e Dinamica della Memoria
1. **Allocazione dinamica nella memoria Heap:**
   * Utilizzo delle funzioni di libreria `<stdlib.h>`: `malloc()`, `calloc()`, `realloc()`, `free()`.
   * Gestione dei puntatori `NULL` e controllo dei fallimenti di allocazione.
   * Concetti di Memory Leak (perdita di memoria) e Dangling Pointers (puntatori pendenti).

### Modulo 3: Strutture Dati Dinamiche Lineari
1. **Liste collegate semplici (Singly Linked Lists):**
   * Strutture autoreferenziali (`struct` contenenti un puntatore al tipo stesso).
   * Operazioni fondamentali: inserimento (in testa, in coda, ordinato), cancellazione di nodi, ricerca, attraversamento.
   * Algoritmi iterativi e ricorsivi su liste.
2. **Liste doppiamente collegate (Doubly Linked Lists) e Liste Circolari:** Cenni e strutture con doppio puntatore (`prev`, `next`).

### Modulo 4: Tipi di Dato Astratti (ADT - Abstract Data Types)
1. **Pila (Stack - LIFO):**
   * Operazioni `push()`, `pop()`, `isEmpty()`, `top()`.
   * Implementazione tramite array statico/dinamico e tramite liste collegate.
2. **Coda (Queue - FIFO):**
   * Operazioni `enqueue()`, `dequeue()`, `isEmpty()`.
   * Implementazione tramite array (gestione circolare) e tramite liste collegate (gestione con puntatori `head` e `tail`).

### Modulo 5: Strutture Dati Non Lineari
1. **Alberi Binari (Binary Trees):**
   * Definizione di nodo di un albero binario (`data`, `leftPtr`, `rightPtr`).
   * Visite di un albero binario: in-ordine (In-order), pre-ordine (Pre-order), post-ordine (Post-order).
   * Inserimento e ricerca in Alberi Binari di Ricerca (BST - Binary Search Trees).
   * Algoritmi ricorsivi su alberi (calcolo dell'altezza, conteggio nodi/foglie).

### Modulo 6: Modularità, Compilazione Separata e Tipi Avanzati
1. **Programmazione Modulare su più file:**
   * Divisione del codice tra file sorgente (`.c`) e file di intestazione/header (`.h`).
   * Uso delle direttive al preprocessore: `#include`, `#define`, `#ifndef`, `#define`, `#endif` (include guards).
2. **Tipi Unione (`union`):**
   * Definizione e differenza di allocazione di memoria rispetto alle `struct`.
   * Utilizzo delle unioni per la gestione di tipi di dati variabili.

### Modulo 7: Gestione dell'I/O su File
1. **File formattati di testo:**
   * Apertura e chiusura file: `fopen()`, `fclose()` con controllo delle modalità (`"r"`, `"w"`, `"a"`).
   * Lettura e scrittura formattata: `fscanf()`, `fprintf()`, `fgets()`, `fgetc()`, `feof()`.

---

## 4. Modalità d'Esame e Valutazione

* **Tipologia:** Prova Scritta al Calcolatore in Laboratorio.
* **Struttura della Prova:**
  * Domande a risposta chiusa/aperta sulla teoria e sintassi C.
  * Esercizi di programmazione in ambiente controllato con compilazione e sottomissione del codice.
  * I progetti e gli esercizi pratici vengono sottoposti a **test automatici** (condizione necessaria per il superamento è l'esito positivo di tutti i test).
* **Esonero:**
  * È prevista la possibilità di sostenere una prova di **Esonero** (punteggio da 1 a 3 punti).
* **Composizione del Voto Finale:**
  $$\text{Voto Finale} = \text{Punteggio Esonero (1-3)} + \text{Punteggio Scritto (17-30)}$$
  * Se il totale è $\ge 31$, il voto verbalizzato è **30 e Lode**.

---

## 5. Testi Consigliati e Risorse
* **Libri di Riferimento:**
  * *Il linguaggio C. Fondamenti e tecniche di programmazione* (IX ed.) - Paul J. Deitel, Harvey M. Deitel, Pearson.
  * *Struttura e progetto dei calcolatori - Progettare con RISC-V* - D. A. Patterson, J. L. Hennessy, Zanichelli (per approfondimenti su allocazione in memoria e stack).
* **Piattaforme Online:**
  * Pagina Moodle del corso (*informatica.i-learn.unito.it*): slide, registrazioni lezioni, esercizi ed esempi di test.
