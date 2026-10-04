# Piano degli Studi e Programmi Dettagliati - Corso di Laurea in Informatica (UniTO)

Questo documento raccoglie la panoramica completa delle materie, dei crediti formativi universitari (CFU), delle descrizioni e degli argomenti d'esame per il primo anno del Corso di Laurea in Informatica dell'Università degli Studi di Torino.

---

## Panoramica Sintetica degli Insegnamenti (60 CFU Totali)

| Materia | CFU | Semestre | Tipologia | Modalità d'Esame |
| :--- | :---: | :---: | :--- | :--- |
| **Matematica Discreta, Algebra e Geometria** | 12 | 1° Semestre | Di base (MAT/02, MAT/03) | Scritto |
| **Programmazione I** | 9 | 1° Semestre | Caratterizzante (INF/01) | Scritto (al pc o cartaceo) |
| **Fondamenti dell'Informatica** | 9 | 1° Semestre | Di base (INF/01) | Scritto (2 parti su Moodle) |
| **Analisi Matematica** | 9 | 2° Semestre | Di base (MFN0570) | Scritto e Orale |
| **Architettura degli Elaboratori** | 6 | 2° Semestre | Caratterizzante (INF/01) | Scritto (Ammissione, Teoria, Lab) + Orale obbligatorio |
| **Programmazione II** | 6 | 2° Semestre | Caratterizzante (INF/01) | Scritto |
| **Ricerca Operativa** | 6 | 2° Semestre | Affine/Integrativo (MAT/09) | Scritto + Orale facoltativo |
| **Lingua Inglese I** | 3 | 2° Semestre | Prova Lingua Straniera (L-LIN/12) | Pratica al computer (Sistema SET, Parti A e B) |

---

## 1. Matematica Discreta, Algebra e Geometria (12 CFU)

* **Codice Attività Didattica:** INF0328 | **SSD:** MAT/02 (Algebra), MAT/03 (Geometria)
* **Carico Orario:** 104 ore complessive (64 ore di lezione in aula + 40 ore di esercitazioni).
* **Semestre:** Primo semestre | **Tipologia:** Di base | **Frequenza:** Facoltativa.
* **Prerequisiti:** Matematica di base delle scuole superiori (operazioni aritmetiche, potenze, equazioni di 1° e 2° grado).

### Descrizione e Obiettivi Formativi
L'insegnamento fornisce un'introduzione rigorosa alla matematica discreta, all'algebra lineare e alla geometria analitica. Ha lo scopo di sviluppare confidenza con le strutture algebriche, il calcolo combinatorio e vettoriale, fornendo i metodi dimostrativi necessari per l'informatica teorica e applicata.

### Programma e Argomenti Dettagliati
1. **Linguaggio degli Insiemi, Relazioni e Funzioni:**
   * Insieme vuoto, sottoinsiemi, unione, intersezione, complementare, insieme delle parti.
   * Relazioni d'ordine, relazioni di equivalenza e partizioni.
   * Corrispondenze e funzioni: iniettività, suriettività, biiettività, composizione e inversione.
2. **Calcolo Combinatorio:**
   * Cardinalità di insiemi finiti, principi della somma e del prodotto.
   * Disposizioni e combinazioni (semplici e con ripetizione).
   * Teorema del binomio di Newton, triangolo di Pascal-Tartaglia, principio di inclusione-esclusione.
3. **Strutture Algebriche:**
   * Semigruppi, monoidi (monoide delle parole) e gruppi con relativi morfismi.
   * Esempi principali: numeri naturali, interi, gruppo delle biiezioni.
   * Gruppi e sottogruppi ciclici, Teorema di Lagrange.
   * Corpi e campi (campo dei numeri razionali $\mathbb{Q}$).
4. **Aritmetica Modulare:**
   * Anelli degli interi ($\mathbb{Z}$) e delle classi di resto ($\mathbb{Z}_n$).
   * Teorema della divisione ed algoritmo di Euclide per il M.C.D.
   * Identità di Bézout ed equazioni diofantee lineari.
   * Congruenze lineari e Teorema di Eulero-Fermat.
5. **Gruppo delle Permutazioni:**
   * Composizione, potenze e inverse di permutazioni.
   * Decomposizione in cicli disgiunti e trasposizioni; parità di una permutazione.
6. **Algebra Lineare e Geometria:**
   * Spazi vettoriali, sottospazi, dipendenza lineare, basi e dimensione.
   * Calcolo matriciale, determinante, rango, algoritmi di riduzione (Gauss-Jordan).
   * Sistemi di equazioni lineari e Teorema di Rouché-Capelli.
   * Applicazioni lineari, matrici associate, nucleo e immagine.
   * Autovalori, autovettori, polinomi caratteristici e diagonalizzazione.
   * Prodotti scalari, ortogonalità, forme quadratiche e Teorema spettrale.

### Informazioni Utili ed Esame
* **Modalità d'esame:** Prova scritta obbligatoria su Moodle/carta. Supporto di tutorato opzionale (2 ore/settimana).
* **Testo consigliato:** Note del corso (Prof. A. Mori / Prof.ssa M. Roggero).

---

## 2. Programmazione I (9 CFU)

* **Codice Attività Didattica:** MFN0582 | **SSD:** INF/01 (Informatica)
* **Carico Orario:** 78 ore complessive (48 ore in aula + 30 ore in laboratorio).
* **Semestre:** Primo semestre | **Tipologia:** Caratterizzante | **Frequenza:** Facoltativa.
* **Prerequisiti:** Nessun requisito di programmazione; confidenza nell'uso del PC e logica matematica di base.

### Descrizione e Obiettivi Formativi
L'insegnamento introduce i concetti fondamentali della programmazione imperativa e l'uso di un interprete virtuale/runtime. Forma lo studente sulla progettazione di algoritmi risolutivi, la loro traduzione in codice C e la gestione della memoria.

### Programma e Argomenti Dettagliati
1. **Modello di Memoria e Tipi Elementari:**
   * Tipi di dati scalari/primitivi, operatori aritmetici e logico-relazionali.
   * Comando di assegnazione ed evoluzione dello stato della memoria.
   * Tipo puntatore, indirizzi di memoria, allocazione e deallocazione dinamica basica (`malloc()`, `free()`).
   * Costrutti di selezione (`if-else`, `switch`).
2. **Programmazione Iterativa:**
   * Cicli ed iterazione (`while`, `for`, `do-while`).
   * Risoluzione di problemi numerici e filtri/conteggi su array monodimensionali e puntatori.
3. **Funzioni e Gestione del Frame-Stack:**
   * Struttura e signature delle funzioni, passaggio dei parametri (per valore e per indirizzo/puntatore).
   * Meccanismo della chiamata: parametri formali/attuali, variabili locali, frame di attivazione, operand stack.
4. **Ricorsione e Correttezza:**
   * Progettazione di funzioni ricorsive su problemi numerici e su stringhe.
   * Algoritmi dicotomici e ricorsione su array monodimensionali e strutture puntate.
   * Dimostrazione informale di correttezza parziale e terminazione.
5. **Schemi Algoritmi e Strutture Dati:**
   * Collezioni di dati eterogenei (`struct`).
   * Gestione di quantificatori alternati su array e matrici bidimensionali.

### Informazioni Utili ed Esame
* **Modalità d'esame:** Prova scritta al calcolatore o su carta per la verifica di progettazione algoritmica, codifica C e simulazione runtime.
* **Testi consigliati:** P.J. Deitel, H.M. Deitel, *Il linguaggio C. Fondamenti e tecniche di programmazione* (Pearson); S. Prata, *C Primer Plus* (Addison-Wesley); J. Hanly et al., *Problem Solving e programmazione in C* (Apogeo).

---

## 3. Fondamenti dell'Informatica (English-Friendly Course) (9 CFU)

* **Codice Attività Didattica:** INF0348 | **SSD:** INF/01 (Informatica)
* **Carico Orario:** 72 ore di lezioni frontali in aula.
* **Semestre:** Primo semestre | **Tipologia:** Di base | **Frequenza:** Facoltativa.
* **Prerequisiti:** Nessuno specifico; costituisce il fondamento metodologico e propedeutico.

### Descrizione e Obiettivi Formativi
Fornisce un approccio formale e matematico all'informatica. Copre la rappresentazione digitale dell'informazione, la sintesi di circuiti logici, la logica matematica e la teoria degli automi e linguaggi formali.

### Programma e Argomenti Dettagliati
1. **Rappresentazione Digitale dell'Informazione:**
   * Unità di misura (bit, byte, multipli), notazione posizionale.
   * Codifica dei numeri naturali e interi: binario, ottale, esadecimale, complemento a 1 e complemento a 2.
   * Codifica dei numeri reali: virgola mobile (standard IEEE 754), notazione esponenziale.
2. **Circuiti Digitali e Algebra di Boole:**
   * Porte logiche, tabelle di verità, espressioni booleane e forme normali (CNF, DNF).
   * Progettazione e sintesi di circuiti combinatori e cenni sui circuiti sequenziali.
3. **Logica Matematica e Tecniche di Dimostrazione:**
   * Rappresentazione insiemistica di relazioni e funzioni (insieme potenza, prodotto cartesiano).
   * Logica proposizionale: tavole di verità, conseguenza logica, deduzione naturale.
   * Logica dei quantificatori: sintassi, semantica e leggi di de Morgan / dualità.
   * Tecniche di dimostrazione: diretta, per assurdo, per contrapposizione, per induzione.
4. **Linguaggi Formali ed Automi a Stati Finiti:**
   * Alfabeti, parole, operazioni su linguaggi (concatenazione, stella di Kleene).
   * Automi a Stati Finiti Deterministici (DFA) e Non Deterministici (NFA).
   * Teorema di equivalenza di Rabin-Scott (determinizzazione NFA $\rightarrow$ DFA).
   * Espressioni regolari e Teorema di Kleene.
   * Proprietà dei linguaggi regolari e Pumping Lemma per la non-regolarità.

### Informazioni Utili ed Esame
* **Modalità d'esame:** Esame scritto erogato tramite Moodle, suddiviso in due parti sequenziali (il superamento della prima è vincolante per l'accesso alla seconda).
* **Testo consigliato:** R. Johnsonbaugh, J.G. Brookshear, D. Brylow, *Fondamenti dell'Informatica* (Pearson).

---

## 4. Analisi Matematica (9 CFU)

* **Codice Attività Didattica:** MFN0570 | **SSD:** MAT/05 (Analisi Matematica)
* **Carico Orario:** 78 ore complessive (48 ore di lezione + 30 ore di esercitazioni).
* **Semestre:** Secondo semestre | **Tipologia:** Di base | **Frequenza:** Facoltativa.
* **Prerequisiti:** Concetti di base forniti dal Corso di Riallineamento di Matematica (Orient@mente).

### Descrizione e Obiettivi Formativi
Presenta lo studio di funzioni reali di variabile reale, il calcolo differenziale e integrale, la risoluzione approssimata di equazioni e il comportamento delle serie numeriche per l'analisi di fenomeni continui e discreti.

### Programma e Argomenti Dettagliati
1. **Funzioni, Grafici e Modelli:**
   * Funzioni elementari, dominio, codominio, simmetrie e trasformazioni geometriche dei grafici.
   * Composizione di funzioni.
2. **Concetto di Limite e Continuità:**
   * Limite di funzioni in ambito continuo e limiti di successioni nel discreto.
   * Principali teoremi sui limiti (Teorema dei carabinieri, permanenza del segno, ecc.).
   * Successioni definite per ricorrenza.
   * Confronti asintotici e stime di crescita: simboli di Landau ($O, o, \sim$).
3. **Calcolo Differenziale:**
   * Definizione di derivata e significato geometrico/fisico.
   * Regole di derivazione; relazione tra derivabilità e continuità.
   * Teoremi del calcolo differenziale (Rolle, Lagrange, Cauchy, De L'Hôpital).
   * Studio di funzione: monotonia, punti stazionari, concavità/convessità e flessi.
   * Approssimazione locale mediante polinomi di Taylor e Maclaurin.
4. **Risoluzione Approssimata di Equazioni:**
   * Teorema di esistenza degli zeri.
   * Algoritmo di bisezione e metodo delle tangenti di Newton.
5. **Calcolo Integrale:**
   * Integrale definito secondo Riemann e sue proprietà.
   * Teorema Fondamentale del Calcolo Integrale e formula di Torricelli-Barrow.
   * Tecniche di integrazione: per sostituzione, per parti, di funzioni razionali fratte.
   * Integrali impropri (su intervalli illimitati o per funzioni non limitate).
6. **Serie Numeriche:**
   * Definizioni, somme parziali e convergenza.
   * Serie notevoli: geometrica e armonica generalizzata.
   * Criteri di convergenza per serie a termini positivi (confronto, confronto asintotico, rapporto, radice) e serie alternate (Leibniz).

### Informazioni Utili ed Esame
* **Modalità d'esame:** Prova scritta e/o orale.
* **Testi consigliati:** M. Bramanti, C.D. Pagani, S. Salsa, *Analisi Matematica 1* (Zanichelli).

---

## 5. Architettura degli Elaboratori (English-Friendly Course) (6 CFU)

* **Codice Attività Didattica:** INF0326 | **SSD:** INF/01 (Informatica)
* **Carico Orario:** 52 ore complessive (32 ore di teoria + 20 ore di laboratorio).
* **Semestre:** Secondo semestre | **Tipologia:** Caratterizzante | **Frequenza:** Facoltativa.
* **Prerequisiti:** Competenze di Programmazione I (C) e Fondamenti dell'Informatica.

### Descrizione e Obiettivi Formativi
Illustra la struttura hardware dei moderni calcolatori digitali, la gerarchia delle macchine virtuali e i processi di traduzione dai linguaggi ad alto livello al linguaggio macchina, con esercitazioni pratiche in Assembly RISC-V.

### Programma e Argomenti Dettagliati
1. **Modulo Teorico (4 CFU - 32 ore):**
   * **Astrazioni e tecnologia:** Prestazioni dei calcolatori e legge di Moore.
   * **Instruction Set Architecture (ISA) RISC-V:** Registri, operandi di memoria, formato delle istruzioni, aritmetica intera e in virgola mobile.
   * **Traduzione ed Esecuzione:** Fasi di compilazione, assemblaggio, linking e loading (assembler, linker, loader).
   * **Il Processore RISC-V:** Datapath a singolo ciclo, unità di controllo, ALU, registri e metodologia di temporizzazione.
   * **Bus e Gestione I/O:** Tipi di bus, arbitraggio, I/O programmato (busy waiting/polling), I/O a interruzioni (interrupts) e Direct Memory Access (DMA).
   * **Gerarchia di Memoria:** Principi di località spaziale e temporale, tecnologie (RAM, DRAM, SRAM), organizzazione e prestazioni delle memorie cache.
2. **Modulo di Laboratorio (2 CFU - 20 ore):**
   * Programmazione in linguaggio Assembly RISC-V tramite simulatori (es. RARS / Venus).
   * Implementazione di istruzioni condizionali, cicli, operazioni logico-aritmetiche.
   * Gestione delle procedure: passaggio parametri, salvataggio registri, stack frame e heap.

### Informazioni Utili ed Esame
* **Modalità d'esame:** L'esame si compone di:
  1. Prova di ammissione a risposte chiuse/aperte (10 punti).
  2. Prova scritta di teoria (14 punti) e laboratorio/assembly (8 punti).
  3. Prova orale obbligatoria.
* **Testo obbligatorio:** D.A. Patterson, J.L. Hennessy, *Struttura e progetto dei calcolatori - Progettare con RISC-V* (Zanichelli).

---

## 6. Programmazione II (6 CFU)

* **Codice Attività Didattica:** INF0330 | **SSD:** INF/01 (Informatica)
* **Carico Orario:** 52 ore complessive (32 ore in aula + 20 ore in laboratorio).
* **Semestre:** Secondo semestre | **Tipologia:** Caratterizzante | **Frequenza:** Facoltativa.
* **Prerequisiti:** Solide basi di C fornite da Programmazione I.

### Descrizione e Obiettivi Formativi
Approfondisce la programmazione imperativa avanzata in C, focalizzandosi sull'allocazione dinamica complessa, strutture dati ricorsive, tipi astratti di dato (ADT), sviluppo modulare su più file e principi di ingegneria del software (testing, invarianti).

### Programma e Argomenti Dettagliati
1. **Ripasso ed Ingegneria del Software:**
   * Analisi formale dei requisiti e specifiche non ambigue.
   * Testing guidato (Test-Driven Development) e programmazione basata su invarianti.
2. **Gestione Dinamica Avanzata della Memoria:**
   * Pointers avanzati, gestione di memory leak, allocazione di strutture complesse.
3. **Strutture Dati Dinamiche Lineari:**
   * Liste collegate (singole, doppie, circolari, ordinate).
   * Inserimento, cancellazione, ricerca e sintesi dati via iterazione e ricorsione.
4. **Tipi di Dati Astratti (ADT):**
   * Realizzazione di Pila (Stack) e Coda (Queue) tramite array e liste collegate.
5. **Modularità e Compilazione Multi-file:**
   * Suddivisione del codice in file d'intestazione (`.h`) e file sorgente (`.c`).
   * Direttive al precompilatore, guardie d'inclusione (`#ifndef`), makefile e compilazione separata.
6. **Strutture Dati Non Lineari e Tipi Avanzati:**
   * Alberi binari: definizione, visita (anticipata, simmetrica, posticipata), alberi binari di ricerca (BST).
   * Tipi `union` ed enumerazioni (`enum`).
7. **Input/Output su File:**
   * Gestione dei file formattati in C (`fopen`, `fclose`, `fscanf`, `fprintf`, `fseek`).

### Informazioni Utili ed Esame
* **Modalità d'esame:** Prova scritta (teoria e laboratorio al pc) con sviluppo di codice C funzionante e test suite.
* **Testi consigliati:** Materiale didattico ufficiale fornito su Moodle e testi di riferimento di C.

---

## 7. Ricerca Operativa (6 CFU)

* **Codice Attività Didattica:** INF0327 | **SSD:** MAT/09 (Ricerca Operativa)
* **Carico Orario:** 52 ore complessive (32 ore in aula + 20 ore di esercitazioni).
* **Semestre:** Secondo semestre | **Tipologia:** Affine/Integrativo | **Frequenza:** Facoltativa.
* **Prerequisiti:** Matematica Discreta, Algebra e Geometria (sistemi lineari, matrici, vettori).

### Descrizione e Obiettivi Formativi
Insegna i modelli matematici e gli algoritmi per l'ottimizzazione decisionale e la gestione di risorse scarse, con focus sulla Programmazione Lineare (PL) continua ed intera e sui problemi di flusso su rete.

### Programma e Argomenti Dettagliati
1. **Introduzione e Modellistica:**
   * Concetto di ottimizzazione, funzione obiettivo, vincoli e regione ammissibile.
   * Cenni di teoria della complessità computazionale.
   * Formulazione di problemi reali come programmi lineari (PL).
2. **Programmazione Lineare Continua:**
   * Geometria della PL: vertici, soluzioni base ammissibili.
   * Algoritmo del Simplesso primale (fase I e fase II, tabelle del simplesso).
3. **Teoria della Dualità Lineare:**
   * Costruzione del problema duale, teoremi della dualità debole e forte, condizioni di complementarità.
   * Algoritmo del Simplesso Duale ed analisi di sensibilità.
4. **Programmazione Lineare Intera (PLI):**
   * Modelli con variabili discrete/binarie.
   * Metodi di risoluzione esatta: algoritmo di Branch and Bound e rilassamento lineare.
5. **Problemi di Flusso su Rete:**
   * Grafi, reti di flusso, problema del cammino minimo (Shortest Path - algoritmo di Dijkstra / Bellman-Ford).

### Informazioni Utili ed Esame
* **Modalità d'esame:** Prova scritta (durata min. 1.5 ore, erogata anche in laboratorio) + Prova orale facoltativa (da -16 a +6 punti sul voto dello scritto).
* **Testi consigliati:** Appunti dei docenti; R.J. Vanderbei, *Linear Programming: Foundations and Extensions* (Springer).

---

## 8. Lingua Inglese I (3 CFU)

* **Codice Attività Didattica:** MFN0590 | **SSD:** L-LIN/12 (Lingua e Traduzione Inglese)
* **Carico Orario:** 30 ore di esercitazioni erogate in streaming da Esperto Linguistico.
* **Semestre:** Secondo semestre | **Tipologia:** Prova Lingua Straniera | **Frequenza:** Facoltativa.
* **Prerequisiti:** Nessuno. Possibile esonero con riconoscimento certificazioni esterne B1/B2 (domanda APU).

### Descrizione e Obiettivi Formativi
Garantisce e verifica la conoscenza della lingua inglese al livello B1-B2 del QCER, focalizzandosi sulla grammatica di base, il lessico informatico e la comprensione del testo scritto (reading).

### Programma Articolato nei 14 Moduli Ufficiali
1. **Modulo 1:** *Verb Patterns* (`-ing` / `to`), uso di *Make* vs *Do*.
2. **Modulo 2:** Pronomi relativi (*who, which, that, whose*), comparativi e superlativi.
3. **Modulo 3:** Struttura *Have/Has something done*, verbi modali d'obbligo (*must, have to, mustn't*), *Present Simple*.
4. **Modulo 4:** Avverbi di frequenza, *Present Continuous*, preposizioni di tempo/luogo, *phrasal verbs*.
5. **Modulo 5:** Gerundio, *Simple Past* e *Past Continuous*.
6. **Modulo 6:** Connettivi (*linkers*), espressioni condizionali (*provided, as long as, unless*), strutture *Used to / Be used to / Get used to*.
7. **Modulo 7:** Forme future (*will, be going to, present continuous*) e *First Conditional*.
8. **Modulo 8:** Sostantivi *Countable / Uncountable*, *Present Perfect* con *since* e *for*.
9. **Modulo 9:** Tempi composti avanzati (*Past Perfect, Past Perfect Continuous, Future Perfect*).
10. **Modulo 10:** Modali di abilità/permesso, acronimi informatici (API, CPU, RAM) e lettura di segnali/cartelli (*Reading Signs*).
11. **Modulo 11:** Forma Passiva (*Passive Voice*).
12. **Modulo 12:** Discorso Indiretto (*Reported Speech*).
13. **Modulo 13:** *Social English*, registro formale/informale, tipologie di testi d'esame.
14. **Modulo 14:** Articoli (*a, an, the, zero article*), pronomi e possessivi.

### Informazioni Utili ed Esame
* **Modalità d'esame:** Prova pratica informatizzata nei laboratori tramite il sistema **SET**, divisa in:
  * **Parte A (60 min):** Test di sbarramento grammaticale (obbligatorio).
  * **Parte B (30 min):** Lettura e comprensione di testi informatici.
* **Testo consigliato:** R. Murphy, *English Grammar in Use* (Cambridge University Press).
* **Contatto commissione:** `commissione-inglese@di.unito.it`
