> [!info] Programma ufficiale del corso
> Le note di studio sono in [[Indice - Analisi Matematica]] · la mappa di tutti i corsi è in [[Indice generale]]

# Guida di Studio: Analisi Matematica (UniTO)

* **Codice Attività Didattica:** MFN0570
* **Settore Scientifico-Disciplinare (SSD):** MAT/05 (Analisi Matematica)
* **Crediti Formativi Universitari (CFU):** 9 CFU (48 ore di lezione in aula + 30 ore di esercitazioni)
* **Anno e Semestre:** 1° Anno, 2° Semestre
* **Tipologia e Frequenza:** Insegnamento di base | Frequenza facoltativa
* **Prerequisiti:** Competenze di matematica di base della scuola secondaria di secondo grado (pendenza della retta, parabole, potenze, logaritmi, trigonometria elementare, studio qualitativo di funzioni). I prerequisiti possono essere recuperati tramite il Corso di Riallineamento di Matematica sulla piattaforma Orient@mente (OFA).

---

## 1. Descrizione e Obiettivi Formativi
L'insegnamento ha lo scopo di presentare le nozioni fondamentali dell'analisi matematica per funzioni reali di una variabile reale, con un'attenzione specifica all'applicazione nell'informatica (come l'analisi della complessità degli algoritmi e la modellizzazione di fenomeni discreti).

Il corso si propone di:
* Fornire padronanza con le funzioni elementari, i grafici e le loro trasformazioni.
* Sviluppare il concetto di limite sia in ambito continuo (funzioni) che discreto (successioni).
* Introdurre il calcolo differenziale (derivate, teoremi fondamentali, sviluppo di Taylor) e il calcolo integrale (integrali definiti, impropri e serie numeriche).
* Insegnare metodi numerici e approssimati per la risoluzione di equazioni (bisezione, Newton) e il calcolo di integrali.
* Rafforzare il ragionamento rigoroso e logico-deduttivo attraverso teoremi e dimostrazioni formali.

---

## 2. Programma Dettagliato degli Argomenti

### Modulo 1: Funzioni, Grafici e Modelli
* **Funzioni elementari:** Proprietà algebriche, domini, immagine, zeri, segno e monotonia di polinomi, funzioni potenza, esponenziali, logaritmiche e trigonometriche.
* **Trasformazioni geometriche:** Traslazioni, dilatazioni, riflessioni e valori assoluti applicati ai grafici.
* **Composizione di funzioni:** Grafici di funzioni composte e inversione di funzioni.

### Modulo 2: Il Concetto di Limite e Successioni
* **Limiti di funzioni (caso continuo):** Definizione intuitiva e formale di limite, limiti destri e sinistri, forme indeterminate e teoremi sui limiti.
* **Continuità:** Definizione di funzione continua, punti di discontinuità, Teorema degli zeri e Teorema di Weierstrass.
* **Limiti di successioni (caso discreto):** Comportamento asintotico delle successioni, successioni geometriche.
* **Successioni per ricorrenza:** Definizione, studio qualitativo e stabilità degli equilibri per successioni lineari del primo ordine.
* **Simboli di Landau e complessità:** Confronti di crescita tra funzioni/successioni, notazione $O, o, \Omega, \Theta$ e loro utilizzo nella discussione della complessità computazionale degli algoritmi.

### Modulo 3: Calcolo Differenziale
* **Derivata in un punto:** Definizione geometrica (pendenza della retta tangente) e cinematica (tasso di variazione istantaneo).
* **Regole di derivazione:** Derivate delle funzioni elementari, regole per somma, prodotto, quoziente e catena (funzioni composte).
* **Teoremi del calcolo differenziale:** Teorema di Rolle, Teorema di Lagrange (del valor medio) e sue conseguenze (caratterizzazione delle funzioni con derivata nulla, test di monotonia).
* **Studio di funzione:** Test di monotonia (segno della derivata prima), test di convessità/concavità (segno della derivata seconda) e ricerca di punti stazionari, massimi e minimi relativi/assoluti.
* **Approssimazione locale:** Polinomi di Taylor e Mac-Laurin con resto di Peano/Lagrange per l'approssimazione locale di funzioni.

### Modulo 4: Risoluzione Approssimata di Equazioni
* **Teorema degli Zeri e Metodo di Bisezione:** Algoritmo ricorsivo di bisezione per la stima delle radici di un'equazione $f(x)=0$ e stima dell'errore.
* **Metodo di Newton:** Schema iterativo di Newton-Raphson, condizioni di convergenza e confronto di efficienza con il metodo di bisezione.

### Modulo 5: Calcolo Integrale
* **Integrale Definito:** Definizione di integrale di Riemann, significato geometrico (area) e fisico (lavoro, spostamento).
* **Teoremi Fondamentali:**
  * Teorema della media integrale.
  * Teorema Fondamentale del Calcolo Integrale (funzione integrale e continuità).
  * Teorema di Torricelli-Barrow (formula fondamentale per il calcolo delle primitive).
* **Integrazione numerica/approssimata:** Formula del punto medio e stima dell'errore.
* **Integrali Impropri:** Integrali su intervalli illimitati o di funzioni illimitate, criteri di convergenza (confronto e confronto asintotico).

### Modulo 6: Serie Numeriche
* **Definizione di Serie:** Successione delle somme parziali, carattere di una serie (convergente, divergente, indeterminata).
* **Serie Geometrica:** Somma e condizione di convergenza $|q| < 1$.
* **Serie Armonica e Armoniche Generalizzate:** Studio della convergenza della serie $\sum \frac{1}{n^p}$.
* **Criteri di Convergenza:** Criterio del confronto, criterio del confronto asintotico, criterio della radice e del rapporto.
* **Legame tra Serie e Integrali Impropri:** Criterio integrale di convergenza.

---

## 3. Modalità d'Esame e Struttura della Prova

L'esame si svolge in **modalità informatizzata al computer** ed è composto da tre prove consecutive, tutte obbligatorie:

1. **Prima Prova (Quiz Preliminare di Sbarramento):**
   * **Struttura:** 5 domande a risposta multipla sui concetti e le competenze di base.
   * **Sbarramento:** È necessario rispondere correttamente ad almeno **4 domande su 5** per accedere alle prove successive.
   * **Bonus Punteggio:**
     * 4 risposte corrette: **+1 punto** sul voto finale.
     * 5 risposte corrette: **+2 punti** sul voto finale.

2. **Seconda Prova (Calcolo Esatto e Teoria):**
   * Verifico delle capacità di calcolo di derivate, primitive, polinomi di Taylor, serie geometriche e dimostrazioni di teoremi teorici. *Calcolatrice non consentita*.

3. **Terza Prova (Calcolo Approssimato e Applicato):**
   * Esercizi su algoritmi numerici (bisezione, Newton), formula del punto medio e integrali impropri/serie. *Uso della calcolatrice consentito*.

### Calcolo del Voto Finale
Il punteggio complessivo è calcolato come la **media aritmetica dei punteggi della Seconda e Terza Prova**, sommata al **bonus ottenuto nel Quiz Preliminare (+1 o +2)**. L'esame è superato con un punteggio finale $\ge 18/30$.

---

## 4. Testi Consigliati e Bibliografia
* **W. Dambrosio**, *Analisi Matematica*, Zanichelli Editore.
* **M. Bramanti, C.D. Pagani, S. Salsa**, *Analisi Matematica 1*, Zanichelli Editore.
