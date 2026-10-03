# Algoritmi e Programmi

> [!warning] Nota trasversale
> Questo argomento **non è nel programma di Fondamenti dell'Informatica** come argomento di esame: è un'introduzione generale che fa da ponte fra i corsi. Il contenuto che esce all'esame di Fondamenti è in [[Algebra di Boole e Porte Logiche]], [[Logica Proposizionale]] e nel blocco linguaggi formali. La programmazione imperativa è invece oggetto di [[Programma - Programmazione I]].

Fondamenta di tutta l'informatica. Distinguere i due concetti è essenziale.

---

## Le tre definizioni

| Concetto | Definizione | Chi lo esegue |
|---|---|---|
| **Dato** | un fatto grezzo, senza significato | nessuno |
| **Informazione** | un dato interpretato, che ha significato | la persona |
| **Algoritmo** | sequenza **finita** e **deterministica** di passi che risolve un problema | la macchina |
| **Programma** | un algoritmo scritto in un linguaggio formale | il computer |

### Algoritmo vs Programma

Sono la **stessa cosa a due livelli diversi**:

- L'**algoritmo** è l'idea, il metodo per risolvere il problema. È indipendente dal linguaggio e dall'hardware. Si può descrivere a parole, con un diagramma di flusso o in pseudocodice.
- Il **programma** è l'algoritmo codificato in un linguaggio che il computer capisce, quindi in byte eseguibili.

> 💡 Ricorda: *ogni programma è un algoritmo, ma non ogni algoritmo è un programma.* Un algoritmo di cucina è un algoritmo ma non è un programma.

---

## Le quattro proprietà di un algoritmo

Un buon algoritmo deve essere:

1. **Finito** — deve terminare dopo un numero **finito** di passi
2. **Deterministico** — a ogni passo, il passo successivo è **univocamente** determinato
3. **Corretto** — produce l'output atteso
4. **Efficiente** — usa risorse ragionevoli (tempo e memoria)

La proprietà **1** e la **2** non sono negoziabili: un algoritmo che non le rispetta non è un algoritmo.

> ⚠️ **Il caso dei programmi che non terminano:** il problema di stabilire se un dato programma **termina** è il **problema dell'arresto** (Halting Problem), dimostrato **non risolvibile da algoritmi** da Alan Turing nel 1936. È il limite che separa la computabilità dagli algoritmi effettivamente implementabili: esistono problemi che possiamo descrivere ma non risolvere sistematicamente.

---

## Come si scrive un algoritmo: lo pseudocodice

Prima di programmare si ragiona in **pseudocodice**: un misto di linguaggio naturale e sintassi di programmazione.

```
INIZIO
    LEGGI n
    SOMMA ← 0
    PER i DA 1 A n
        SOMMA ← SOMMA + i
    FINECHO
    SCRIVI SOMMA
FINE
```

Vantaggi:
- funziona in **qualsiasi** linguaggio
- si concentra sulla **logica**, non sulla sintassi
- è più facile da correggere prima di scrivere codice

---

## Metodi per progettare un algoritmo

| Metodo | Quando usarlo |
|---|---|
| **Divide et impera** | il problema si spezza in sottoproblemi indipendenti (es. merge sort) |
| **Programmazione dinamica** | sottoproblemi che si sovrappongono, con risultati memorizzati |
| **Greedy** | una scelta locale ottima a ogni passo, senza guardare il futuro |
| **Backtracking** | si prova, si torna indietro se sbagliato (es. labirinto, N regine) |

Questi metodi sono il cuore della programmazione lineare (in [[Programma - Ricerca Operativa]]) e di quasi tutti gli esercizi d'esame di algoritmica.

---

## Diagrammi di flusso

Notazione grafica classica. Utile per capire un algoritmo, meno per scrivere programmi complessi.

| Simbolo | Significato |
|---|---|
| Ellisse | inizio / fine |
| Rettangolo | operazione (istruzione) |
| Rombo | decisione (sì/no) |
| Parallelogramma | input / output |

> 💡 **Limite:** la teoria dei diagrammi di flusso mostra che sono equivalenti alla **macchina di Turing** (quindi Turing-completi), ma il teorema di Böhm-Jacopini dimostra che i tre costrutti **sequenza**, **selezione** e **iterazione** bastano per tutto: ogni algoritmo si può riscrivere usando solo questi. È la base del C.

---

## Dalle proprietà: tipi di algoritmo

| Tipo | Esempio |
|---|---|
| Sequenziale | somma di una lista |
| Condizionale | somma solo dei numeri pari |
| Iterativo | somma i numeri da 1 a n |
| Ricorsivo | fattoriale, algoritmi divide et impera |

---

## Esempi contesto informatico

- **Ordinamento di una lista di file** per nome: il `sort` di Linux è un algoritmo, il comando è il programma.
- **Ricerca in una directory**: il file system usa una struttura ad albero (B-tree) per non dover leggere tutti i file.
- **Git**: fa un `diff` (algoritmo di confronto di versioni) per mostrare le modifiche.
- **Autocompletamento**: cerca il prefisso più lungo corrispondente — problema di stringhe, servono algoritmi efficienti.

---

## Riepilogo

- **Dato** → **Informazione** (interpretazione)
- **Algoritmo** = metodo di risoluzione · **Programma** = algoritmo codificato
- Un algoritmo è finito e deterministico: se non lo è, non è un algoritmo
- Prima si ragiona in **pseudocodice**, poi si scrive il codice
- I metodi fondamentali: divide et impera, dinamica, greedy, backtracking

---

## Link

- [[Programma - Fondamenti dell'Informatica]] — il programma di questo corso
- [[Programma - Programmazione I]] — algoritmi e ricorsione nel C, con esercizi d'esame
- [[Programma - Ricerca Operativa]] — complessità computazionale e ottimizzazione
- [[Programma - Architettura degli Elaboratori]] — la traduzione algoritmo → linguaggio macchina
