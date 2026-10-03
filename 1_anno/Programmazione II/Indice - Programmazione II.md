# Indice - Programmazione II

> [!info] Mappa del corso
> **Legenda:** ✅ scritto · 📄 da scrivere
> Programma ufficiale: [[Programma - Programmazione II]]

| | |
|---|---|
| **Codice** | INF0330 · SSD INF/01 |
| **Crediti** | 6 CFU · 52 ore (32 aula + 20 laboratorio) |
| **Semestre** | 2° (1° anno) |
| **Esame** | Scritto al calcolatore in laboratorio. Teoria + esercizi di programmazione **sottoposti a test automatici**: tutti i test devono passare. Esone da 1-3 punti. Voto = esone (1-3) + scritto (17-30); ≥31 diventa 30L |
| **Prerequisiti** | [[Programma - Programmazione I]] — padronanza del C |
| **Testi** | Deitel & Deitel, *Il linguaggio C* · Patterson & Hennessy, *Progettare con RISC-V* (per stack e memoria) |

> ⚠️ **Questo NON è un corso di OOP.** È **C avanzato**: memoria dinamica, strutture dati ricorsive, ADT, compilazione multi-file. Non ci sono classi, ereditarietà o Java.

---

## Modulo 1. Ripasso e lettura delle specifiche

| Argomento | Note |
|---|---|
| Ripasso della programmazione imperativa in C | 📄 [[Ripasso C Imperativo]] |
| Analisi della consegna: input/output, filtraggio, output | 📄 [[Analisi delle Specifiche]] |
| Ingegneria del software, TDD e invarianti | 📄 [[Testing e Invarianti]] |

## Modulo 2. Gestione esplicita e dinamica della memoria

| Argomento | Note |
|---|---|
| `malloc()`, `calloc()`, `realloc()`, `free()` | 📄 [[Allocazione Dinamica]] |
| Puntatori NULL e controllo dei fallimenti | 📄 [[Gestione dei Fallimenti]] |
| Memory leak e dangling pointers | 📄 [[Memory Leak e Dangling Pointers]] |

## Modulo 3. Strutture dati dinamiche lineari

| Argomento | Note |
|---|---|
| Strutture autoreferenziali | 📄 [[Strutture Autoreferenziali]] |
| Liste semplicmente collegate: operazioni | 📄 [[Liste Collegate]] |
| Algoritmi iterativi e ricorsivi su liste | 📄 [[Algoritmi su Liste]] |
| Liste doppiamente collegate e circolari | 📄 [[Liste Doppie e Circolari]] |

## Modulo 4. Tipi di dato astratti (ADT)

| Argomento | Note |
|---|---|
| Pila (stack, LIFO) | 📄 [[Pila]] |
| Coda (queue, FIFO) | 📄 [[Coda]] |
| Realizzazione con array e con liste collegate | 📄 [[ADT con Array e Liste]] |

## Modulo 5. Strutture dati non lineari

| Argomento | Note |
|---|---|
| Alberi binari: definizione e nodi | 📄 [[Alberi Binari]] |
| Visite in-ordine, pre-ordine, post-ordine | 📄 [[Visite di Alberi]] |
| Alberi binari di ricerca (BST) | 📄 [[Alberi Binari di Ricerca]] |
| Algoritmi ricorsivi: altezza, conteggio nodi e foglie | 📄 [[Algoritmi su Alberi]] |

## Modulo 6. Modularità e compilazione separata

| Argomento | Note |
|---|---|
| File sorgente `.c` e header `.h` | 📄 [[Compilazione Multi-File]] |
| Direttive del preprocessore e include guard `#ifndef` | 📄 [[Preprocessore e Include Guard]] |
| `union` e suo rapporto con `struct` | 📄 [[Unioni]] |

## Modulo 7. I/O su file

| Argomento | Note |
|---|---|
| `fopen()`, `fclose()`, modalità r/w/a | 📄 [[File e Stream]] |
| `fscanf()`, `fprintf()`, `fgets()`, `fgetc()`, `feof()` | 📄 [[File Formattati]] |

---

## Sicurezza in C: cosa verrà chiesto

- Controllare **sempre** il valore restituito da `malloc()` (NULL = fallimento)
- Liberare **tutto** ciò che è stato allocato: il memory leak è l'errore più comune
- Non lasciare dangling pointer dopo `free()`
- Nel laboratorio gli esercizi passano solo se **tutti** i test automatici danno esito positivo

## Collegamenti ad altri corsi

- [[Programma - Programmazione I]] — il C di base, prerequisito diretto
- [[Programma - Architettura degli Elaboratori]] — lo stack in C visto come record di attivazione
- [[Programma - Fondamenti dell'Informatica]] — le strutture dati nella loro forma teorica
