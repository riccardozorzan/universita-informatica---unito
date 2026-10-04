# Quadro riassuntivo dei 9 moduli

> [!info] Vista d'insieme del Corso di Riallineamento di Matematica (Orient@mente)
> Per lo studio di un singolo modulo: lezioni in [[Indice - Matematica Base]] · Indice OFA: [[Indice - OFA]]

| | |
|---|---|
| **Perché questa nota** | formule e trabocchetti di tutti i 9 moduli, tutte **verificate**, da usare come scheletro nei test |
| **Copertura** | dal linguaggio alla probabilità |
| **Stato** | ✅ **tutti e 9 i moduli** (lezioni, esercizi e test dove disponibili) |

---

## La mappa in una riga

$$\text{linguaggio} \to \text{algebra} \to \text{geometria} \to \text{funzioni} \to \text{probabilità}$$

Ogni modulo **poggia** sul precedente. Se una formula non ti torna, il problema quasi mai è nel modulo che stai studiando: è nel precedente.

| # | Modulo | Domanda a cui risponde | Lezione |
|---|---|---|---|
| 1 | Linguaggio, numeri, simbologia | *che cosa è un oggetto matematico?* | [[1.1 Elementi di Teoria degli Insiemi e Logica]] · [[1.2 Numeri]] |
| 2 | Fattorizzazione | *come si scompone in fattori?* | [[2.1 Polinomi e Fattorizzazione]] |
| 3 | Equazioni, disequazioni, sistemi | *come si risolve e come si rappresentano le soluzioni?* | [[3.1 Equazioni e Disequazioni di 1 Grado]] · [[3.2 Equazioni e Disequazioni di 2 Grado]] · [[3.3 Sistemi di Equazioni]] |
| 4 | Fratte, irrazionali, valore assoluto | *e quando l'incognita è a denominatore, sotto radice o con modulo?* | [[4.1 Equazioni e Disequazioni Fratte]] · [[4.2 Equazioni e Disequazioni Irrazionali]] · [[4.3 Equazioni e Disequazioni con Valore Assoluto]] |
| 5 | Geometria analitica | *come si porta la geometria nel piano cartesiano?* | [[Modulo 5. Geometria Analitica]] |
| 6 | Funzioni reali di variabile reale | *che cosa è una funzione e come si studia?* | [[Modulo 6. Funzioni Reali di Variabile Reale]] |
| 7 | Esponenziali e logaritmi | *e quando la variabile sale a potenza?* | [[Modulo 7. Esponenziali e Logaritmi]] |
| 8 | Trigonometria | *e quando compare il cerchio?* | [[Modulo 8. Trigonometria]] |
| 9 | Statistica e probabilità | *come si ragiona sui dati e sugli eventi?* | [[Modulo 9. Statistica e Probabilità]] |

---

## Modulo 1 — Linguaggio, numeri e simbologia

### Punti chiave

| Concetto | Formula |
|---|---|
| Appartenenza vs inclusione | $x \in A$ (elemento) · $B \subseteq A$ (sottoinsieme) |
| Insieme delle parti | $\lvert \mathcal{P}(X)\rvert = 2^n$ se $\lvert X\rvert = n$ |
| Catena numerica | $\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$ |
| Relazione di equivalenza | **RST** (Riflessiva, Simmetrica, Transitiva) |
| Relazione d'ordine | **RAT** (Riflessiva, Antisimmetrica, Transitiva) |
| Funzione iniettiva | elementi distinti ⟹ immagini distinte |
| Funzione suriettiva | $f(A) = B$ |
| Funzione biiettiva | iniettiva ∧ suriettiva ⟹ ammette inversa |
| **De Morgan (logica)** | $\neg(p \land q) \iff \neg p \lor \neg q$ · $\neg(p \lor q) \iff \neg p \land \neg q$ |
| **De Morgan (insiemi)** | $(A \cap B)^c = A^c \cup B^c$ · $(A \cup B)^c = A^c \cap B^c$ |
| Implicazione | $p \Rightarrow q \iff \neg p \lor q$ · negazione: $p \land \neg q$ |

**Accorgimento.** Pensa **binario** per l'insieme delle parti: ogni elemento ha esattamente 2 scelte, entra o no.

**La regola madre di tutto il modulo.** Negare significa **cambiare il connettivo** e **negare ogni termine**. Vale per $\land \leftrightarrow \lor$, per $\forall \leftrightarrow \exists$, per $\cap \leftrightarrow \cup$:

$$\neg (\forall x \mid P(x)) \iff \exists x \mid \neg P(x) \qquad \neg (\exists x \mid P(x)) \iff \forall x \mid \neg P(x)$$

**In una riga, in italiano.** «Non (P **e** Q)» vuol dire «non P **o** non Q»: se per smentire una frase con un "e" basta **una** delle due negazioni, per smentire una frase con un "o" servono **entrambe». Nei cerchi: si toglie il centro **unendo** i complementari, si prende lo sfondo **intersecandoli**.

In programmazione è la stessa regola: `not (a and b)` ≡ `not a or not b` e `not (a or b)` ≡ `not a and not b`, entrambe verificate esaustivamente. Da NOT sopra AND esce OR, e viceversa.

> ⚠️ **Equivalente ≠ negazione.** $p \Rightarrow q$ equivale a $\neg p \lor q$ (e a $\neg q \Rightarrow \neg p$); la sua **negazione** è $p \land \neg q$. Sono le due risposte da non scambiare.

### 🛑 Trabocchetti

| Errore | Perché è sbagliato |
|---|---|
| scrivere $1 \subseteq A$ con $A = \{1,2\}$ | $1$ è un **elemento**, non un insieme: si scrive $1 \in A$ |
| scrivere $\{1\} \in A$ con $A = \{1,2\}$ | $\{1\}$ è un **sottoinsieme**: si scrive $\{1\} \subseteq A$ |
| dimenticare che $\emptyset \subseteq A$ **sempre** | il vuoto è sottoinsieme di **qualunque** insieme |
| dimenticare che $\emptyset \in \mathcal{P}(A)$ | il vuoto è uno degli **elementi** dell'insieme delle parti |
| scrivere $(A \cup B)^c = A^c \cup B^c$ | il complementare **scambia** ∪ in ∩: è $A^c \cap B^c$ |
| scrivere $A \setminus B = A \cap B$ | serve il complementare del **secondo**: è $A \cap B^c$ |
| dare $\neg p \lor q$ come *negazione* di $p \Rightarrow q$ | quello è l'**equivalente**; la negazione è $p \land \neg q$ |
| dire che $p \Rightarrow q$ è falsa perché $q$ è falsa | è falsa **solo** se $p$ è vera e $q$ falsa |
| scrivere $A \cap B \cap C$ per «almeno due su tre» | serve $(A\cap B) \cup (B\cap C) \cup (A\cap C)$ |
| negare «tutti» scrivendo «nessuno» | la negazione di $\forall$ è $\exists$, non "zero" |
| applicare De Morgan **a metà**: `not (a and b)` → `not a and not b` | la forma corretta è `not a **or** not b`: metà delle volte dà comunque lo stesso risultato, quindi l'errore passa inosservato |

---

## Modulo 2 — Fattorizzazione di polinomi

### Prodotti notevoli

| Nome | Formula |
|---|---|
| Differenza di quadrati | $a^2 - b^2 = (a-b)(a+b)$ |
| Quadrato di binomio | $(a \pm b)^2 = a^2 \pm 2ab + b^2$ |
| Somma / differenza di cubi | $a^3 \pm b^3 = (a \pm b)(a^2 \mp ab + b^2)$ |
| Trinomio notevole | $x^2 + sx + p = (x+a)(x+b)$ con $s = a+b$, $p = a \cdot b$ |

**Ruffini.** $P(x)$ è divisibile per $(x-a)$ se e solo se $P(a) = 0$.

**Ordine di attacco.**

| N. termini | Prova prima |
|---|---|
| 2 | differenza di quadrati o di cubi |
| 3 | quadrato di binomio o trinomio notevole |
| 4 | cubo di binomio, raccoglimento parziale |
| 6 | raccoglimento parziale |

Prima di tutto: **raccoglimento totale a fattor comune**. Poi, se i metodi immediati falliscono, Ruffini. I candidati zeri vanno cercati tra i **divisori del termine noto** divisi per i **divisori del coefficiente di grado massimo**.

### 🛑 Trabocchetti

| Errore | Perché è sbagliato |
|---|---|
| scomporre $a^2 + b^2$ | **non** si scompone sui reali: $\Delta < 0$ |
| nel cubo, cercare il fattore $2$ davanti ad $ab$ | in $a^3 - b^3$ il fattore è $a^2 + ab + b^2$, **senza** $2ab$ |

> 💡 **Verifica utile:** $a^2 + ab + b^2$ ha $\Delta = -3a^2 < 0$ come polinomio in $b$, quindi **non** ha radici reali e non si scompone ulteriormente.


---

## Modulo 3 — Equazioni, disequazioni e sistemi

### Equazioni di 2° grado

$$ax^2 + bx + c = 0 \implies x_{1,2} = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a} = \frac{-b \pm \sqrt{\Delta}}{2a}$$

| $\Delta$ | Significato | Soluzioni |
|---|---|---|
| $> 0$ | due reali **distinte** | $x_1 \neq x_2$ |
| $= 0$ | due reali **coincidenti** | $x = -\frac{b}{2a}$ |
| $< 0$ | **nessuna** reale | $\varnothing$ |

### Metodo della parabola

Se $a > 0$ e $\Delta > 0$: il segno $> 0$ prende i valori **esterni**, il segno $< 0$ quelli **interni**.

$$\Delta > 0,\ a > 0: \quad x < x_1 \;\vee\; x > x_2 \qquad\text{e}\qquad x_1 < x < x_2$$

### Accorgimenti

**Formula ridotta**, se $b$ è pari: evita metà dei conti.

$$\frac{\Delta}{4} = \left(\frac{b}{2}\right)^2 - ac \qquad\Longrightarrow\qquad x_{1,2} = \frac{-\frac{b}{2} \pm \sqrt{\Delta/4}}{a}$$

> 💡 Verificato su $2x^2 + 6x + 4$: $\Delta = 4$ e $\Delta/4 = 1$; la formula ridotta dà $x = \frac{-3 \pm 1}{2} = -1, -2$, gli stessi risultati.

**Standardizzazione**: se $a < 0$, cambia **subito** tutti i segni e **inverti** il verso. Esempio $-x^2 + 3x - 2 > 0$ diventa $x^2 - 3x + 2 < 0$ ⟹ $1 < x < 2$ ✅

### 🛑 Trabocchetti

| Errore | Perché è sbagliato |
|---|---|
| confondere **sistema** con **tabella dei segni** | nel sistema cerchi la **intersezione** (tutte vere insieme); nel prodotto/fratta **moltichi** i segni |
| dividere per $x$ in $x^2 = 3x$ | perdi $x = 0$! Porta tutto a sinistra: $x(x-3) = 0 \Rightarrow x = 0 \vee x = 3$ ✅ |
| non standardizzare quando $a < 0$ | il verso si inverte: le soluzioni vengono **capovolte** |

---

## Modulo 4 — Fratte, irrazionali e valore assoluto

### Fratte

Le **C.E.** ($D(x) \neq 0$) si impongono **prima** di ogni calcolo. Nelle disequazioni si studia il segno di $N$ e $D$ **separatamente** e si costruisce la griglia dei segni.

### Irrazionali con indice pari

| Problema | Sistema |
|---|---|
| $\sqrt{A(x)} = B(x)$ | $\begin{cases} B(x) \geq 0 \\ A(x) = [B(x)]^2 \end{cases}$ |
| $\sqrt{A(x)} < B(x)$ | $\begin{cases} A(x) \geq 0 \\ B(x) > 0 \\ A(x) < [B(x)]^2 \end{cases}$ |
| $\sqrt{A(x)} > B(x)$ | $\begin{cases} A(x) \geq 0 \\ B(x) < 0 \end{cases}$ $\cup$ $\begin{cases} B(x) \geq 0 \\ A(x) > [B(x)]^2 \end{cases}$ |

### Valore assoluto

$$|A(x)| = \begin{cases} A(x) & \text{se } A(x) \geq 0 \\ -A(x) & \text{se } A(x) < 0 \end{cases}$$

$$|A(x)| < k \iff -k < A(x) < k \qquad |A(x)| > k \iff A(x) < -k \;\vee\; A(x) > k \qquad (k > 0)$$

### 🛑 Trabocchetti

| Errore | Perché è sbagliato |
|---|---|
| eliminare il denominatore nelle **disequazioni** fratte | il suo segno **varia** e determinerebbe il verso: usa la tabella dei segni |
| includere gli zeri del denominatore con $\geq 0$ | il denominatore deve essere **sempre** $\neq 0$: pallino vuoto |

---

## Modulo 5 — Geometria analitica

### Retta

| Concetto | Formula |
|---|---|
| Forma implicita | $ax + by + c = 0$ |
| Forma esplicita | $y = mx + q$ |
| Parallelismo | $m_1 = m_2$ |
| Perpendicolarità | $m_1 \cdot m_2 = -1 \iff m_2 = -\frac{1}{m_1}$ |
| Distanza punto-retta | $d = \dfrac{\lvert ax_0 + by_0 + c\rvert}{\sqrt{a^2+b^2}}$ |

> ⚠️ **Le rette verticali** hanno equazione $x = k$ e **non hanno** coefficiente angolare $m$: non esiste $q$ tale che $k = mq + q$. Perciò **mai** usare $y = mx + q$ per esse.

### Parabola

$$y = ax^2 + bx + c \qquad V\left(-\frac{b}{2a},\; -\frac{\Delta}{4a}\right)$$

Concavità verso l'alto se $a > 0$, verso il basso se $a < 0$.

> 💡 **Per l'ordinata del vertice è spesso più rapido sostituire** $x_V = -\frac{b}{2a}$ direttamente nell'equazione, invece di calcolare $-\frac{\Delta}{4a}$. Verificato su $y = x^2 - 4x + 1$: $\Delta = 12$, $x_V = 2$, $y_V = -3$ ✅

### Circonferenza

$$x^2 + y^2 + ax + by + c = 0 \qquad C\left(-\frac{a}{2}, -\frac{b}{2}\right) \qquad r = \sqrt{\frac{a^2}{4} + \frac{b^2}{4} - c}$$

**Condizione di esistenza:** perché sia una circonferenza reale deve essere $\frac{a^2}{4} + \frac{b^2}{4} - c > 0$.

> 💡 Verificato su $x^2 + y^2 - 4x - 6y + 3 = 0$: centro $(2, 3)$, $r^2 = 4 + 9 - 3 = 10$. Il punto $(2, 3 + \sqrt{10})$ soddisfa l'equazione ✅

### 🛑 Trabocchetti

| Errore | Perché è sbagliato |
|---|---|
| dimenticare il valore assoluto nella distanza | la distanza è una **lunghezza**: deve essere $\geq 0$ sempre |
| invertire le coordinate del vertice | $x_V = -\frac{b}{2a}$; l'ordinata è **l'altra** |
| usare $y = mx+q$ per una retta verticale | non ha coefficiente angolare |

---

## Modulo 6 — Funzioni reali di variabile reale

### Dominio

| Vincolo | Condizione |
|---|---|
| Denominatori | $\neq 0$ |
| Radici di indice pari | $\geq 0$ |
| Argomenti di logaritmi | $> 0$ |

### Simmetrie e monotonia

| Tipo | Condizione | Simmetria |
|---|---|---|
| **pari** | $f(-x) = f(x)$ | asse $y$ |
| **dispari** | $f(-x) = -f(x)$ | origine $O$ |
| crescente | $x_1 < x_2 \Rightarrow f(x_1) < f(x_2)$ | — |

---

## Modulo 7 — Esponenziali e logaritmi

### Funzioni

$$\text{Esponenziale } y = a^x, \quad a > 0,\ a \neq 1: \quad \mathcal{D} = \mathbb{R}, \quad \mathcal{I} = (0, +\infty)$$

$$\text{Logaritmica } y = \log_a(x), \quad a > 0,\ a \neq 1: \quad \mathcal{D} = (0, +\infty), \quad \mathcal{I} = \mathbb{R}$$

Sono **inverse**: $y = \log_a(x) \iff a^y = x$.

### Proprietà

$$\log_a(xy) = \log_a(x) + \log_a(y) \qquad \log_a\left(\frac{x}{y}\right) = \log_a(x) - \log_a(y) \qquad \log_a(x^k) = k\log_a(x)$$

$$\log_b(x) = \frac{\log_a(x)}{\log_a(b)}$$

### 🛑 Trabocchetti

| Errore | Perché è sbagliato |
|---|---|
| $\log(a+b) = \log(a) + \log(b)$ | l'**addizione** dentro il logaritmo **non** si spezza |
| $\frac{\log a}{\log b} = \log(a-b)$ | il rapporto non è un logaritmo |
| $\log(x^2) = 2\log(x)$ | **restringe** il dominio! La forma corretta è $2\log\lvert x\rvert$ |

> ⚠️ **Il caso $\log(x^2)$ è il più sottile.** $\log(x^2)$ è definita per ogni $x \neq 0$; scrivendo $2\log(x)$ si ottiene il dominio $x > 0$, che **perde** tutti gli $x < 0$. Verificato: per $x = -2$, $\log(4) = 2\log 2$ è definita, mentre $2\log(-2)$ non lo è.

**Base compresa tra 0 e 1.** Se $0 < a < 1$ la funzione è **decrescente**, quindi il verso si **inverte**:

$$\left(\frac{1}{2}\right)^x > \left(\frac{1}{2}\right)^3 \;\Longrightarrow\; x < 3$$

### Le 3 regole che risolvono equazioni e disequazioni

| Situazione | Regola |
|---|---|
| stessa base, $a>1$ | si confrontano gli **esponenti** (o gli argomenti), verso **mantenuto** |
| stessa base, $0<a<1$ | si confrontano gli esponenti (o gli argomenti), verso **invertito** ⚠️ |
| **basi diverse** | si applica $\log$ ad ambo i membri, scegliendo base $c>1$ perché il verso resti invariato |

$$\log_c a^{f(x)} = \log_c b^{g(x)} \;\Longrightarrow\; f(x)\log_c a = g(x)\log_c b$$

$$\log_a f(x) = c \;\Longleftrightarrow\; a^c = f(x) \qquad\qquad \log_a f(x) = \log_a g(x) \;\Longrightarrow\; f(x) = g(x)$$

> ⚠️ **Il verso si può invertire due volte.** Nelle basi diverse, se il denominatore finale è **negativo**, spostare la $x$ **inverte** di nuovo il verso. Verificare sempre il segno.

> ⚠️ **Le condizioni di esistenza non sono un dettaglio.** Un logaritmo con argomento $\leq 0$ **non esiste**: la soluzione trovata che le viola va **rifiutata**. E la disequazione finale va sempre intersecata con il dominio, a volte restringendolo.

> ⚠️ **Esponenziale $\neq$ potenza.** In $a^x$ la $x$ è l'esponente, in $x^a$ è la base. Cambia tutto: $x^2$ non è definita per $x<0$ e non è definita in $0$, $2^x$ lo è ovunque.

---

## Modulo 8 — Trigonometria

### Misure e relazioni

$$\alpha_{\text{rad}} = \alpha_{\text{gradi}} \cdot \frac{\pi}{180^\circ} \qquad \sin^2 x + \cos^2 x = 1 \qquad \tan x = \frac{\sin x}{\cos x}$$

**C.E. della tangente:** $x \neq \frac{\pi}{2} + k\pi$. **C.E. della cotangente:** $x \neq k\pi$.

### Valori notevoli

| $x$ | $0$ | $\frac{\pi}{6}$ $(30^\circ)$ | $\frac{\pi}{4}$ $(45^\circ)$ | $\frac{\pi}{3}$ $(60^\circ)$ | $\frac{\pi}{2}$ $(90^\circ)$ |
|---|---|---|---|---|---|
| $\sin x$ | $0$ | $\frac{1}{2}$ | $\frac{\sqrt2}{2}$ | $\frac{\sqrt3}{2}$ | $1$ |
| $\cos x$ | $1$ | $\frac{\sqrt3}{2}$ | $\frac{\sqrt2}{2}$ | $\frac{1}{2}$ | $0$ |
| $\tan x$ | $0$ | $\frac{\sqrt3}{3}$ | $1$ | $\sqrt3$ | **N.D.** |

> ⚠️ **Memorizza solo $30^\circ$ e $45^\circ$**, deriva il resto: $\cos 60^\circ = \sin 30^\circ = \frac12$ e $\sin 45^\circ = \cos 45^\circ = \frac{\sqrt2}{2}$.

### Le 3 equazioni da sapere a memoria

| | Condizione | Periodo |
|---|---|---|
| $\sin\alpha = \sin\beta$ | $\alpha = \beta + 2k\pi$ **oppure** $\alpha = \pi - \beta + 2k\pi$ (**supplementari**) | $2\pi$ |
| $\cos\alpha = \cos\beta$ | $\alpha = \beta + 2k\pi$ **oppure** $\alpha = -\beta + 2k\pi$ (**opposti**) | $2\pi$ |
| $\tan\alpha = \tan\beta$ | $\alpha = \beta + k\pi$ (**un solo caso**) ⚠️ | $\pi$ |

### Le proprietà dei grafici

| | periodo | dominio | limitate | parità |
|---|---|---|---|---|
| $\sin x$ | $2\pi$ | $\mathbb{R}$ | ✅ $[-1,1]$ | dispari |
| $\cos x$ | $2\pi$ | $\mathbb{R}$ | ✅ $[-1,1]$ | pari |
| $\tan x$ | $\pi$ | $\mathbb{R}\setminus\{\frac\pi2+k\pi\}$ | ❌ no | dispari |

> ⚠️ **Tre controlli che i test sfruttano:**
> - $\sin x = c$ e $\cos x = c$ hanno soluzione **solo se** $|c| \leq 1$
> - la relazione $\sin^2+\cos^2=1$ dà il valore **assoluto**: il **segno** si legge dal quadrante
> - il periodo di $h\sin(kx)$ è $\frac{2\pi}{|k|}$, e il fattore **fuori** dall'argomento non lo cambia

### I triangoli

| Contesto | Formule |
|---|---|
| rettangolo | $a = c\sin\alpha = c\cos\beta$ · $a = b\tan\alpha = b\cot\beta$ |
| **Carnot** | $a^2 = b^2+c^2-2bc\cos\alpha$ |
| **seni** | $a:\sin\alpha = b:\sin\beta = c:\sin\gamma$ |

---

## Modulo 9 — Statistica e probabilità

### Indici di posizione

| Indice | Definizione |
|---|---|
| **Media** $\bar{x}$ | $\bar{x} = \dfrac{\sum x_i}{n}$ |
| **Mediana** | il valore in **posizione centrale** dei dati **ordinati** |
| **Moda** | il valore con **massima frequenza** |

**Mediana.** Ordina sempre i dati.

| $n$ | Posizione |
|---|---|
| **dispari** | $\frac{n+1}{2}$ |
| **pari** | media dei valori in posizione $\frac{n}{2}$ e $\frac{n}{2}+1$ |

> 💡 Verificato: su $[3,1,4,1,5,9,2,6]$ ordinati $[1,1,2,3,4,5,6,9]$, $n = 8$ ⟹ posizioni 4 e 5 ⟹ mediana $\frac{3+4}{2} = 3{,}5$.

### Indici di dispersione

$$\sigma^2 = \frac{\sum (x_i - \bar{x})^2}{n} \qquad \sigma = \sqrt{\sigma^2}$$

> ⚠️ Questa è la **varianza** (divisione per $n$). La divisione per $n - 1$ dà la **varianza campione**, che è un'altra cosa.

### Probabilità

$$P(E) = \frac{\text{casi favorevoli}}{\text{casi possibili}} \qquad P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

$$P(A \cap B) = P(A)\cdot P(B) \quad \text{(indipendenti)} \qquad P(A \mid B) = \frac{P(A \cap B)}{P(B)}$$

> 💡 Verificato: $P(\text{maggiore di 3} \mid \text{pari}) = \frac{P(4,6)}{P(2,4,6)} = \frac{2/6}{3/6} = \frac{2}{3}$ ✅

### 🛑 Trabocchetti

| Errore | Perché è sbagliato |
|---|---|
| calcolare la mediana **senza ordinare** | è l'errore **più comune** in assoluto nei quiz |
| confondere **incompatibili** e **indipendenti** | incompatibili ⟹ $P(A \cap B) = 0$; indipendenti ⟹ $P(A\cap B) = P(A)P(B)$ |
| leggere $P(A\mid B)$ come "A e B" | la condizionata **filtra**: si lavora **dentro** $B$ |

> 💡 **La differenza in una frase.** *Incompatibili*: non possono accadere insieme, quindi $P(A \cap B) = 0$. *Indipendenti*: possono accadere insieme, ma accadere l'uno **non cambia** la probabilità dell'altro. La chiave è che per gli incompatibili il prodotto $P(A)P(B)$ **non** vale (a meno di non essere entrambi nulli).

---

## Le trappole trasversali

Sono gli errori che **ritornano** in più moduli. Se li hai interiorizzati, copri metà dei test.

| # | Trappola | Moduli | Come evitarla |
|---|---|---|---|
| 1 | **Dividere per un'incognita** che può essere zero | 2, 3, 4, 7 | porta tutto a un lato e usa il prodotto nullo |
| 2 | **Dimenticare i vincoli** di esistenza | 3, 4, 6, 7 | scrivili **prima**, non dopo |
| 3 | **Intersezione** scambiata con **unione** | 3, 4, 6, 9 | "tutte insieme" = intersezione; "una delle due" = unione |
| 4 | **Non standardizzare** il segno di $a$ | 2, 3 | se $a < 0$, cambia i segni e **inverti** il verso |
| 5 | **Estrapolare** da un grafico | 5, 6 | i test si riferiscono **solo** all'intervallo mostrato |
| 6 | **Elevare al quadrato** senza condizioni | 4 | imponi $B(x) \geq 0$ o verifica a posteriori |
| 7 | **Confondere** dominio e immagine | 6, 7 | dominio ⟶ ascisse $x$; immagine ⟶ ordinate $y$ |
| 8 | **Perdere soluzioni** speciali ($x = 0$, $k = 0$) | 3, 4 | verifica sempre le soluzioni "scomode" |

> ⚠️ **La numero 1 è la più costosa.** In $x^2 = 3x$ dividere per $x$ cancella $x = 0$, che invece è una soluzione **valida** (verificato: $0 = 0$). Lo stesso vale per $\frac{x}{x-2} = 1$ moltiplicando per $x - 2$: si perde $x = 2$. È la regola che collega il Modulo 3, il 4 e il 5.

---

## Come usare questa nota

1. **Prima di un test**, rileggi solo la sezione del modulo e la pagina dei trabocchetti.
2. **Se una domanda ti confonde**, torna alla lezione completa (link in testa alla sezione).
3. **Se un risultato ti sembra strano**, verificalo: le formule qui sono state controllate con il calcolo simbolico.

> 💡 **Il consiglio più utile di tutti.** Nei test a risposta multipla, quando un quesito non ti torna, il dubbio è quasi sempre **su di te**, non sul testo. Rileggi l'enunciato cercando una parola che cambia tutto: *sempre*, *solo*, *almeno uno*, *esattamente*, *nessuno*. Sono quelle che danno la risposta.

---

## Link

- [[Indice - Matematica Base]] — l'indice dei 9 moduli con lo stato delle lezioni
- [[Indice - OFA]] — l'indice degli OFA e come assolverli
- [[Programma - OFA]] — programma ufficiale e modalità di assolvimento
> 💡 **Regola mnemonica dei seni:** $\sin\left(\frac{\pi}{n}\right) = \frac{\sqrt{n-2}}{2}$ per $n = 2, 3, 4, 6$. Cioè $\frac{\sqrt0}{2}$, $\frac{\sqrt1}{2}$, $\frac{\sqrt2}{2}$, $\frac{\sqrt3}{2}$, $\frac{\sqrt4}{2} = 1$.

### Periodicità

| Equazione | Soluzioni |
|---|---|
| $\sin x = m$ | $x = \alpha + 2k\pi \;\vee\; x = (\pi - \alpha) + 2k\pi$ |
| $\cos x = m$ | $x = \pm \alpha + 2k\pi$ |
| $\tan x = m$ | $x = \alpha + k\pi$ |

> ⚠️ **La tangente ha periodo $\pi$, non $2\pi$.** È l'unica delle tre. Verificato: $\tan x = 1$ dà $x = \frac{\pi}{4} + k\pi$.

### 🛑 Trabocchetti

| Errore | Perché è sbagliato |
|---|---|
| dimenticare la periodicità | $\sin x = \frac12$ ha **infiniti** risultati: servono i $2k\pi$ |
| usare $2k\pi$ per la tangente | il periodo di $\tan$ è $\pi$ |
| ignorare la C.E. di $\tan$ | a $x = \frac{\pi}{2}$ la tangente **non esiste** |



> 💡 **Test della retta verticale.** Una curva è il grafico di una funzione se e solo se ogni retta verticale la interseca **al massimo una volta**.

### 🛑 Trabocchetti

| Errore | Perché è sbagliato |
|---|---|
| estrapolare un grafico fuori dal riquadro | nei test le domande si riferiscono **solo all'intervallo visualizzato** |
| leggere il dominio sull'asse $y$ | il dominio si legge sulle **ascisse** ($x$), l'immagine sulle **ordinate** ($y$) |

> ⚠️ **Nota sui test.** Questa è la regola che vale per **tutti** i test con grafici dei Moduli 5 e 6.


| $\sqrt{x} = -3 \Rightarrow x = 9$ | $\sqrt{9} = 3 \neq -3$: **soluzione parassita**. Serve $B(x) \geq 0$ |
| pensare che $-A(x)$ sia negativo | se $A(x) = -5$, allora $-A(x) = +5$ |

