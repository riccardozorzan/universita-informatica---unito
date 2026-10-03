# Funzioni Elementari

> [!info] Modulo 1 · Funzioni, grafici e modelli
> Corso di [[Programma - Analisi Matematica]] · Indice: [[Indice - Analisi Matematica]]

> [!warning] Da sapere prima
> Questa è la **prima nota del corso**: si presuppone che le funzioni si sappiano già manipolare. Se il dominio di $\sqrt{x-1}$ o la parità non ti sono famigliari, torna a [[6.1 Definizione di Funzione e Principali Caratteristiche]] del percorso OFA.

---

## 1. Cos'è una funzione

Una funzione $f : A \to B$ è una relazione tra due insiemi che soddisfa due condizioni:

- **Funzionalità**: a ogni elemento del dominio corrisponde **un solo** elemento del codominio, $|f(a \in A)| = 1$
- **Ovunque definita**: per ogni elemento del dominio esiste un'immagine, $f(a \in A) \neq \emptyset$ per ogni $a \in A$

Si scrive in due modi:

$$f(x) = x + 1 \qquad\text{oppure, più rigoroso:}\qquad f \ : \ A \to B,\quad x \mapsto x+1$$

La seconda forma dichiara esplicitamente dominio e codominio; la prima li lascia impliciti. **In un esame conta scrivere la seconda** quando il dominio non è tutto $\mathbb{R}$.

## 2. Le tre proprietà

| | Condizione | In linguaggio |
|---|---|---|
| **Suriettiva** | $f(A) = B$ | ogni elemento di $B$ è raggiunto |
| **Iniettiva** | $f(a_1) \neq f(a_2)$ per $a_1 \neq a_2$ | elementi distinti → immagini distinte |
| **Biiettiva** | suriettiva **e** iniettiva | corrispondenza uno-a-uno |

> 💡 **Il test grafico.** Una funzione è iniettiva se nessuna retta orizzontale la taglia in più di un punto. È surgettiva se ogni retta orizzontale la taglia **almeno** una volta, e illimitata in alto e in basso.

## 3. Funzioni affini, non "lineari"

$$f(x) = mx + q, \qquad m, q \in \mathbb{R}$$

> ⚠️ **Avvertenza terminologica.** In Analisi queste funzioni si chiamano **affini**, non lineari. Infatti una funzione lineare deve soddisfare $f(\alpha x + \beta y) = \alpha f(x) + \beta f(y)$, e per $f(x)=mx+q$ con $q \neq 0$ la proprietà **fallisce**.
>
> Verificalo: $f(2x + 3y) = m(2x+3y)+q$, mentre $2f(x)+3f(y) = 2mx+3my + 5q$. Diversi.
>
> Nel contesto **lineare** (Matematica Discreta) e in quello **omomorfico** le due accezioni coincidono. La differenza è solo terminologica, ma in un esame è un errore da non fare.

La funzione affine è la composizione di una funzione lineare ($x \mapsto mx$) e di una ** traslazione** ($x \mapsto x+q$) che sposta l'origine.

### Il ruolo di $m$ e di $q$

$m$ si chiama:

- **pendenza** della funzione
- **coefficiente angolare**
- coefficiente di proporzionalità fra la variazione di $f$ e quella di $x$

Il nome "angolare" viene dalla trigonometria: se $\theta$ è l'inclinazione della retta, allora $m = \tan\theta$.

> 💡 **Per $m = 0$** la funzione è costante, $f(x) = q$: retta orizzontale. Altrimenti, per $m \neq 0$:
> - lo **zero** è $x = -\dfrac{q}{m}$
> - $f(0) = q$ è l'**intercetta** con l'asse $y$

## 4. Rappresentazione delle funzioni

Una funzione di una variabile si rappresenta nel piano cartesiano con:
- **ascisse**: la variabile indipendente $x$
- **ordinate**: $f(x)$, cioè la variabile dipendente $y$

Il grafico è l'insieme $\{(x, f(x)) : x \in D\}$.

> 💡 **Perché si chiama dipendente.** Il valore di $y$ non si sceglie: è obbligato da $x$. Da qui la freccia $x \mapsto y$.

## 5. Le trasformazioni geometriche

Data una funzione $f$, queste sono le operazioni che ne modificano il grafico. **Saperle elencare è l'obiettivo di questa sezione**: quasi sempre l'esame chiede "cosa fa questo grafico".

| Operazione | Effetto | Nota |
|---|---|---|
| $f(x) + t$ | traslazione **verticale** di $t$ | su se $t>0$, giù se $t<0$ |
| $f(x - t)$ | traslazione **orizzontale** di $t$ | a **destra** se $t>0$ |
| $f(x + t)$ | traslazione **orizzontale** di $t$ | a **sinistra** se $t>0$ |
| $-f(x)$ | riflesso rispetto all'**asse $x$** | |
| $f(-x)$ | riflesso rispetto all'**asse $y$** | |
| $t \cdot f(x)$, $t>0$ | dilatazione **verticale** | contrazione se $0<t<1$ |
| $f(t \cdot x)$, $t>0$ | dilatazione **orizzontale** | contrazione se $0<t<1$ |
| $-t \cdot f(x)$ | riflesso sull'asse $x$ **+** dilatazione verticale | gli effetti si sommano |
| $\lvert f(x) \rvert$ | riflette in alto **solo** la parte sotto l'asse | la parte positiva resta identica |
| $f(\lvert x \rvert)$ | sostituisce la parte con $x<0$ con quella con $x>0$ | |

### 5.1 Le traslazioni: il segno va verificato

Questo è il punto su cui sbaglia più gente, quindi **verificalo con un esempio**.

Prendiamo $f(x) = x^2$ e $t = 2$:
- $f(x-2) = (x-2)^2$ ha il vertice in $x = 2$ → spostato a **destra** ✅
- $f(x+2) = (x+2)^2$ ha il vertice in $x = -2$ → spostato a **sinistra** ✅

> 💡 **La regola:** in $f(x - t)$ il vertice del grafico finisce a $x = t$. Nel caso verticale $f(x)+t$ le quote salgono di $t$. Non c'è simmetria tra i due casi, perché in uno si sposta l'ascissa e nell'altro l'ordinata.

### 5.2 Il valore assoluto su una funzione

Due operazioni diverse, spesso confuse:

| | Significato |
|---|---|
| $\lvert f(x) \rvert$ | si riflette la parte **negativa** del *valore* |
| $f(\lvert x \rvert)$ | si sostituisce $x<0$ con $\lvert x \rvert$ |

Verifica con $g(x) = x-1$:
- $\lvert g(x) \rvert = \lvert x - 1 \rvert$: la parte sotto l'asse ($x<1$) viene rispecchiata sopra
- $g(\lvert x \rvert) = \lvert x \rvert - 1$: per $x<0$ il grafico ricalca quello per $x>0$

### 5.3 Combinare le trasformazioni

Le trasformazioni si applicano in sequenza. Il modo corretto di ragionarci è **scomporle in trasformazioni elementari**, una alla volta.

> ⚠️ **L'ordine conta, ma solo per alcune coppie.** Due traslazioni (una verticale e una orizzontale) o due dilatazioni **commutano** tra loro. Ma una traslazione e un riflesso **no**.

Esempio guidato: disegna $f(x) = \ln(2x+1)$.

1. parte da $g(x) = \ln x$, il cui grafico è noto
2. $2x+1$: dilatazione orizzontale di $1/2$ **e** traslazione a **sinistra** di $1/2$ (perché è $2(x+\tfrac12)$)
3. per trovare l'intercetta con l'asse $x$: $2x+1 = 1 \Rightarrow x = 0$

> 💡 **Il trucco pratico:** per disegnare $g(ax+b)$ basta sapere che la funzione "è viva" per $ax+b>0$, cioè $x > -b/a$. Il dominio è quasi sempre il primo passo, ed è spesso il 90% della domanda.

## 6. Collegamento con il percorso OFA

Questa lezione riprende e **approfondisce** [[6.1 Definizione di Funzione e Principali Caratteristiche]] del Modulo 6 OFA. La differenza di livello è netta:

| Argomento | OFA (Modulo 6) | Analisi (questo corso) |
|---|---|---|
| Dominio | per **elenco** dei casi | per **caso generale** |
| Monotonia | dal grafico o dalla definizione | con $f' \geq 0$ |
| Parità | verifica $f(-x) = \pm f(x)$ | stessa nozione |
| Trasformazioni | un elenco | si ricavano da formule |
| Inverse | solo il metodo di scambio | + condizioni di esistenza rigorose |

> 💡 **Se ti senti solido su OFA 6.1, questa nota ti basterà.** Se qualcosa non torna, il problema è a monte: torna indietro di un passo, non avanti.

## 7. Da sapere per l'esame

L'esame è **informatizzato** e distinto in tre prove:

| Prova | Contenuto | Strumento |
|---|---|---|
| 1ª | quiz di sbarramento, 4/5 corrette | — |
| 2ª | calcolo **esatto** | **senza calcolatrice** |
| 3ª | calcolo **approssimato** | con calcolatrice |

> ⚠️ **Il vincolo della 2ª prova è il più importante da capire subito.** Nella prova di calcolo esatto non puoi usare strumenti: devi saper fare a mano esattamente le operazioni che poi verifichi con la calcolatrice. Questo rende necessaria la padronanza delle formule, non la sola comprensione.

Voto = media di 2ª e 3ª + bonus del quiz; superato con $\geq 18$.

## 8. Esercizi di verifica

**a)** Disegna il grafico di $f(x) = -2x^2 + 4$ partendo da $g(x) = x^2$.
> Rifletti $g$ sull'asse $x$, dilati verticalmente di $2$, poi traslhi in su di $4$. Vertice in $(0,4)$, concavità rivolta verso il basso.

**b)** Verifica la classificazione di $f(x) = 3x - 2$.
> $f$ è affine, non lineare: $f(0) = -2 \neq 0$. Zero in $x = 2/3$, pendenza $m = 3$.

**c)** Trova il dominio di $h(x) = \frac{\ln(5-x)}{x-2}$.
> Due condizioni: $5-x > 0$ e $x-2 \neq 0$ → $\left(-\infty, 2\right) \cup \left(2, 5\right)$

**d)** $f(x) = x^2$ è surgettiva su $[0,+\infty)$?
> Sì: ogni valore positivo o nullo è raggiunto da $x = \sqrt{y}$.

**e)** Spiega perché $\lvert f(x) \rvert$ non modifica la parte del grafico con $f(x) \geq 0$.
> Per $f(x) \geq 0$ si ha $\lvert f(x) \rvert = f(x)$, quindi il grafico coincide.

## 9. Errori da non ripetere

| Errore | Cosa succede invece |
|---|---|
| $f(x)=mx+q$ è "lineare" in Analisi | è **affine**; "lineare" vale per l'algebra lineare |
| $f(x-t)$ sposta a sinistra | sposta a **destra** se $t>0$ |
| $f(x+t)$ sposta a destra | sposta a **sinistra** se $t>0$ |
| $\lvert f(x) \rvert$ riflette tutta la funzione | riflette **solo** la parte negativa |
| confondere $\lvert f(x) \rvert$ e $f(\lvert x \rvert)$ | una agisce sui **valori**, l'altra sugli **argomenti** |
| usare la calcolatrice nella 2ª prova | è **espressoamente vietato** |

---

## Link

- [[Indice - Analisi Matematica]]
- [[Programma - Analisi Matematica]]
- [[6.1 Definizione di Funzione e Principali Caratteristiche]] — la versione OFA di questa lezione
- [[Trasformazioni dei Grafici]] — l'approfondimento
- [[Composizione di Funzioni]]
- [[Metodo di Studio]] — per come usare le prove d'esame