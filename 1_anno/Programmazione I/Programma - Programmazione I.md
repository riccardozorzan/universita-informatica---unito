> [!info] Programma ufficiale del corso
> Le note di studio sono in [[Indice - Programmazione I]] · la mappa di tutti i corsi è in [[Indice generale]]

# Guida allo Studio: Programmazione I

* **Corso di Laurea:** Informatica (L-31) – Università degli Studi di Torino
* **Codice Attività Didattica:** MFN0582
* **SSD:** INF/01 (Informatica)
* **Crediti:** 9 CFU (48 ore di lezione in aula + 30 ore di esercitazioni in laboratorio)
* **Semestre:** 1° Semestre (1° Anno)
* **Tipologia:** Caratterizzante | **Frequenza:** Facoltativa (consigliata)
* **Lingua:** Italiano | **Tipologia Esame:** Scritto (informatizzato o cartaceo)

---

## 1. Descrizione e Obiettivi Formativi

L'insegnamento di **Programmazione I** rappresenta il pilastro d'ingresso per la formazione informatica. Ha l'obiettivo di introdurre i concetti fondamentali della **programmazione imperativa**, della progettazione algoritmica e dell'esecuzione a tempo di esecuzione (*runtime*). 

Il corso guida lo studente nell'astrazione dei problemi, nel ragionamento strutturato sul flusso di controllo e nella gestione accurata dello stato della memoria, fornendo le competenze essenziali necessarie per tutti i successivi corsi di ambito software e sistemi.

---

## 2. Prerequisiti

* **Prerequisiti ufficiali:** Nessuno. Non è richiesta alcuna conoscenza pregressa di programmazione.
* **Competenze consigliate:** 
  * Concetti di matematica di base (operazioni aritmetiche, potenze, radici, logaritmi, equazioni, funzioni e piano cartesiano).
  * Dimestichezza con l'uso base del calcolatore e di sistemi operativi a finestre.
  * Buona padronanza della lingua madre e propensione al ragionamento logico-strutturato.

---

## 3. Programma Dettagliato degli Argomenti

### Modello di Memoria e Tipi Elementari
* **Tipi di dati primitivi/elementari:** Struttura ed operazioni su interi, caratteri, numeri in virgola mobile e booleani.
* **Stato della memoria ed espressioni:** Il concetto di variabile come locazione di memoria, assegnamento e valutazione delle espressioni.
* **Istruzioni di selezione:** Costrutto condizionale `if-then-else`, selezioni annidate e selezioni multiple (`switch`).
* **Introduzione ai puntatori:** Concetto di indirizzo di memoria, operatore di dereferenziazione (`*`), indirizzamento (`&`), allocazione e deallocazione di base (`malloc()`, `free()`).

### Programmazione Iterativa
* **Costrutti iterativi:** Cicli controllati da contatore e da condizione (`while`, `for`, `do-while`).
* **Algoritmi iterativi su dati numerici:** Calcolo di somme, prodotti, serie numeriche e conteggi.
* **Array e Stringhe:** Array monodimensionali e bidimensionali (matrici), manipolazione di vettori, ricerca, filtri e riorganizzazione di elementi.
* **Gestione delle stringhe:** Rappresentazione come vettori di caratteri terminati dal carattere nullo (`\0`).

### Funzioni e Gestione del Frame-Stack
* **Struttura e Firma (Signature):** Definizione, prototipi e modularizzazione del codice.
* **Meccanismo di chiamata:** Passaggio dei parametri per valore e per indirizzo (tramite puntatori).
* **Gestione della memoria a runtime:** Ambito delle variabili (locali vs globali), pila dei frame (*frame-stack*), allocazione sullo stack e pile di operandi (*operand stack*).

### Ricorsione e Correttezza degli Algoritmi
* **Concetto di ricorsione:** Definizione di caso base e passo ricorsivo.
* **Classificazione ed esecuzione ricorsiva:** Ricorsione numerica, su stringhe, su array (approccio dicotomico/divide et impera).
* **Correttezza e terminazione:** Dimostrazione informale di correttezza parziale e totale, invarianti di ciclo e condizioni di terminazione.

### Schemi Algoritmici e Strutture Dati Aggregate
* **Tipi di dati eterogenei:** Definizione e uso delle strutture (`struct`).
* **Quantificatori alternati:** Risoluzione di problemi complessi con verifica di proprietà su coppie di array o matrici.

---

## 4. Modalità d'Esame e Valutazione

L'esame consiste in una **prova scritta** (svolta al calcolatore in laboratorio oppure su carta) focalizzata sulle seguenti abilità:
1. **Progettazione di algoritmi:** Sviluppo di soluzioni sia in modalità **iterativa** che **ricorsiva**.
2. **Codifica in linguaggio C:** Scrittura di codice C corretto, efficiente e aderente alle specifiche.
3. **Analisi del runtime:** Simulazione manuale dello stato della memoria e dello stack dei frame durante l'esecuzione di un programma.
4. **Domande teoriche:** Verifica dei concetti di correttezza, terminazione e proprietà dei tipi di dato.

*Nota:* La somma dei punteggi degli esercizi consente di raggiungere fino al voto massimo di **30 e Lode**.

---

## 5. Testi di Riferimento Consigliati

1. **P. J. Deitel, H. M. Deitel, G. Maselli**, *Il linguaggio C. Fondamenti e tecniche di programmazione* (IX Edizione), Pearson.
2. **Stephen Prata**, *C Primer Plus* (6th Edition), Addison-Wesley Professional.
3. **J. Hanly, E. Koffman**, *Problem solving e programmazione in C*, Pearson.
