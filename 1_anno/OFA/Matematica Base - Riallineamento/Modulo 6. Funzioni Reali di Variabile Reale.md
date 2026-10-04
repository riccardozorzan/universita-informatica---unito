# Modulo 6. Funzioni Reali di Variabile Reale

> [!warning] Nota in corso
> Materiale del **Modulo 6** del Corso di Riallineamento di Matematica (Orient@mente).
> Indice del percorso: [[Indice - Matematica Base]] · Indice OFA: [[Indice - OFA]]

| | |
|---|---|
| **Modulo** | 6 |
| **Argomenti** | funzione reale di variabile reale, caratteristiche principali, aspetti grafici, esempi di funzioni utili |
| **Materiali su Orient@mente** | 2 libri · 2 worksheet Maple T.A. · 2 pagine · 5 file · 3 compiti |
| **Stato** | ✅ **6.1 e 6.2 complete** |

---

## Teoria

### 6.1 Definizione di funzione e principali caratteristiche

✅ [[6.1 Definizione di Funzione e Principali Caratteristiche]] — **completa**, 17 sezioni

**Classificazione:** algebriche (da un polinomio con le 4 operazioni e la radice) vs **trascendenti** (esponenziali, logaritmiche, trigonometriche). Questo modulo tratta **solo** le prime: le altre sono oggetto dei Moduli 7 e 8.

**I 12 punti del sommario ufficiale**

| # | Argomento | Sezione |
|---|---|---|
| 1 | Definizione e nomenclatura | ✅ |
| 2 | Grafico di una funzione (test verticale) | ✅ |
| 3 | Iniettive, suriettive, biunivoche | ✅ |
| 4 | **Restrizione** | ✅ |
| 5 | Funzione inversa | ✅ |
| 6 | Composizione | ✅ |
| 7 | Funzioni pari o dispari | ✅ |
| 8 | **Funzioni periodiche** | ✅ |
| 9 | Crescenti, decrescenti, monotone | ✅ |
| 10 | **Funzioni limitate** | ✅ |
| 11 | **Funzioni continue** (solo intuitivo) | ✅ |
| 12 | Traslazione di funzioni | ✅ |

In più: **zeri e segno** (sezione 13), che è la base delle esercitazioni pur non figurando nel sommario.

> 💡 **Tre concetti che il sommario mette in evidenza e che vanno ricordati:**
> - **controimmagine**: l'insieme degli $x$ con $f(x)=y$; può avere più elementi, essere vuoto, o averne uno
> - **restrizione**: serve a rendere biunivoca una funzione che non lo è (è il ponte verso l'inversa)
> - **test verticale vs orizzontale**: il primo dice se è una funzione, il secondo se è iniettiva

### Lezione 6.2

✅ [[6.2 Esempi di Funzioni Utili]] — **completa**, 5 esempi + esercizi ufficiali.

I **5 esempi del sommario** ufficiale:

| # | Funzione | Forma | Grafico |
|---|---|---|---|
| 1 | **costante** | $y = k$ | retta orizzontale |
| 2 | **definita a tratti** | più espressioni su intervalli diversi | più tratti incollati |
| 3 | **valore assoluto** | $y = \lvert x \rvert$ | due semirette a V |
| 4 | **lineare** | $y = mx + q$ | retta |
| 5 | **$1/x$** | $y = \dfrac{1}{x}$ | iperbole equilatera |

> 💡 **Il punto che collega tutto.** Le due proporzionalità dell'Applicazione 6.2 (Newton) sono le stesse rette e iperboli viste nelle sezioni 4 e 5: $a = F/m$ è **retta** in $F$ e **iperbole** in $m$.

**Esercizi ufficiali** (file *Ulteriori esercizi sulle funzioni*): i **6 esercizi con le soluzioni**, tutti riverificati con SymPy. L'Esercizio 2 è il più utile, perché le tre funzioni a tratti si riconoscono dai **valori in $x=0$** e dal **segno**:

| Funzione | $f(0)$ | Forma | Grafico |
|---|---|---|---|
| $f$ | $+3$ | retta a sinistra, parabola a destra | C |
| $g$ | $+3$ | due rette, a "$\wedge$" | B |
| $h$ | $-3$ | tutta sotto l'asse $x$ | A |

> ⚠️ **Tutte e tre sono continue in $x=0$**: i due tratti si incollano. La trappola dell'esercizio è che $f$ e $g$ hanno lo stesso valore in $0$ e si distinguono solo **alla destra**, dove $f$ cresce e $g$ decresce.

**Worksheet *Esplora 6.2*:** traccia $f(x)$ e $\lvert f(x)\rvert$ affiancati, per vedere che le parti sotto l'asse $x$ vengono riflesse e quelle sopra restano invariate.

**Applicazioni 6.2:** la seconda legge del moto di Newton $F = ma$, da cui $a = F/m$ è **direttamente** proporzionale a $F$ e **inversamente** proporzionale a $m$.

---

## Esercizi

Sezione 14 di [[6.1 Definizione di Funzione e Principali Caratteristiche]]: **9 esercizi** (domini, controimmagini, parità, iniettività/surgettività, restrizione, inverse, composizione, zeri e segno, limitatezza e periodicità), tutti verificati con SymPy.

**Esercizi ufficiali** (file "Ulteriori esercizi su funzioni e loro caratteristiche"): i **10 esercizi della piattaforma con le soluzioni**, aggiunti sempre nella sezione 14 e tutti riverificati. Comprendono i casi che il testo non spiega a parole:

| # | Esercizio | Il punto interessante |
|---|---|---|
| 1 | Domini di $\sqrt{2x^2-x-3}$, $\sqrt[3]{x^4-4}$, $\dfrac{x^2+1}{(1-\sqrt5)x}$ | la radice **cubica** accetta argomento negativo: $g$ è definita su tutto $\mathbb{R}$ |
| 2-3 | Biunivocità e invertibilità da grafici | test della retta orizzontale e simmetria rispetto a $y=x$ |
| 4 | Pari/dispari di $3x^7-5x^3-x$, $6x^4-4x^2$, $3\sqrt{x^2}-1$, $\dfrac{2}{\sqrt{x^2+3x-10}}$ | $\sqrt{x^2} = |x|$ è **pari**, non $x$: da qui il risultato |
| 5 | Monotonia di $x^2-4x+4$ | vertice in $x=2$: decrescente a sinistra, crescente a destra |
| 6-7 | Zeri di $3x^2+7x$ e di $5+\dfrac{x}{x-2}-\dfrac{2}{x+1}$ | il secondo dà esattamente $x = \frac{1\pm\sqrt5}{2}$ |
| 8 | $1/\cos(x)$ è limitata? | **no né sopra né sotto**: il denominatore si avvicina a $0$ da entrambi i lati |
| 9 | Continuità nel mondo reale (semafori, soste, carburante) | i **conteggi discreti** non sono funzioni continue |
| 10 | Traslazioni di $\sin(x)$ | in orizzontale l'intervallo $[-1,1]$ si conserva, in verticale si sposta |

> ⚠️ **Attenzione all'Esercizio 7:** la formula sulla piattaforma è resa in modo ambiguo. Va letta $5 + \frac{x}{x-2} - \frac{2}{x+1}$, non $\frac{5+x}{x-2} - \frac{2}{x+1}$: con la seconda lettura il numeratore sarebbe $x^2+4x+9$, che non ha zeri reali.

> 💡 **Esercizi del Modulo 6 su Orient@mente:** da svolgere dopo aver letto il libro. Con Maple si possono tracciare i grafici per controllare a vista parità, simmetrie e monotonia.

---

## Worksheet "Esplora 6.1 — Grafici di funzione"

Strumento interattivo della piattaforma: si inserisce un'espressione e gli estremi $a$ e $b$, e traccia il grafico. Serve a verificare a vista le caratteristiche, **ma solo nell'intervallo inserito**: se scrivi $[-10, 10]$ e la funzione ha un comportamento diverso fuori, non lo vedi.

Le domande che il worksheet propone, nell'ordine in cui conviene affrontarle:

| Domanda | Cosa guardare | Test corrispondente |
|---|---|---|
| è iniettiva, surgettiva, biunivoca? | quante intersezioni per ogni retta **orizzontale** | una sola = biunivoca |
| presenta simmetrie? è pari o dispari? | simmetria rispetto all'asse $y$ o all'origine | il test $f(-x) \mp f(x)$ |
| ha comportamento periodico? | il tratto si ripete identico | $f(x+T) = f(x)$ |
| dove è crescente, dove decrescente? | il verso con cui il grafico sale e scende andando a destra | derivate di secondo grado |
| è limitata superiormente e inferiormente? | se il grafico resta in una striscia orizzontale | $-1 \leq f(x) \leq 1$ |
| è continua? | si può tracciare senza staccare la penna | assenza di salti |

> ⚠️ **L'errore da non fare con questo strumento.** Una funzione può sembrare iniettiva **nell'intervallo visualizzato** e non esserlo su tutto il dominio. Ad esempio $x^2$ su $[0,10]$ sembra biunivoca, ma su $\mathbb{R}$ non lo è. Vedi l'Esercizio ufficiale 5, dove $5x^2$ diventa biunivoca **proprio grazie alla restrizione** del dominio.

---

## Applicazioni 6.1 — Il legame tra grafici ed equazioni

**Zero** di una funzione $f$ è ogni $x$ del dominio tale che $f(x)=0$. La ricerca degli zeri equivale quindi alla ricerca delle soluzioni dell'equazione $f(x)=0$, e può essere riscritta come sistema:

$$\begin{cases} y = f(x) \\ y = 0 \end{cases}$$

Graficamente significa determinare le **intersezioni del grafico con l'asse $x$**: i punti in cui la curva taglia l'asse sono gli zeri. È il motivo per cui l'equazione si risolve **guardando** il grafico.

**Esempio ufficiale.** $f(x) = x^3 + x^2 - 2x$ si fattorizza come $x(x-1)(x+2)$ (vedi [[2.1 Polinomi e Fattorizzazione]]). L'equazione $x(x-1)(x+2) = 0$ dà tre soluzioni, $x = -2$, $x = 0$, $x = 1$: sono i tre punti in cui il grafico attraversa l'asse $x$.

> 💡 **Perché la fattorizzazione è la strada più rapida.** Su un grafico si vedono gli zeri, ma con precisione solo se sono "belli". L'esempio è scelto proprio perché la fattorizzazione **esatta** dà gli zeri per enumerazione, mentre il grafico serve a controllare che non se ne sia perso qualcuno.

---

## Test di autovalutazione

Sezione 15 di [[6.1 Definizione di Funzione e Principali Caratteristiche]]: **25 domande** con risposte e soluzioni ragionate.

> ⚠️ Nei test con grafici le domande si riferiscono **solo all'intervallo visualizzato**.

---

## Come studiare il modulo

1. Leggi la **lezione 6.1** → svolgi il **worksheet Maple** e il **test 6.1**
2. Leggi la **lezione 6.2** sugli esempi di funzioni utili
3. Fai il **test di fine modulo**

> 💡 **Il ponte con l'OFA e con l'Analisi.** Il dominio è la stessa nozione del *campo di esistenza* del Modulo 4 e della condizione sui radicandi del 4.2. Il Modulo 6 è il capitolo in cui le tre cose si uniscono, ed è il primo modulo di [[Programma - Analisi Matematica]].

> ⚠️ **Due confini da non oltrepassare.** Nel Modulo 6:
> - la **continuità** è solo intuitiva ("senza staccare la penna"); la definizione rigorosa richiede il concetto di limite
> - la **monotonia** si deduce dal grafico o dalla definizione, **non dalle derivate**: $f' \geq 0$ è materia di Analisi

---

## Link

- [[6.1 Definizione di Funzione e Principali Caratteristiche]]
- [[6.2 Esempi di Funzioni Utili]] 📄
- [[Indice - Matematica Base]]
- [[Prerequisiti del Primo Anno]] — dove questo modulo si colloca
- [[Quadro riassuntivo dei 9 moduli]]
