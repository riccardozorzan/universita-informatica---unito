# Calcolo Combinatorio

> [!info] Matematica Discreta, Algebra e Geometria — A2
> Indice del corso: [[Indice - Matematica Discreta, Algebra e Geometria]] · Programma: [[Programma - Matematica Discreta, Algebra e Geometria]]

| | |
|---|---|
| **Argomenti** | principi di conteggio · disposizioni e permutazioni · combinazioni · binomio di Newton · inclusione-esclusione |
| **Prerequisiti** | fattoriali e cardinalità |
| **Tutte le formule** | verificate con calcolo enumerativo diretto |

---

## I principi fondamentali

**Principio della somma.** Se $E$ è l'**unione disgiunta** di due sottoinsiemi $E_1$ ed $E_2$, allora $|E| = |E_1| + |E_2|$.

> ⚠️ La condizione **disgiunta** è indispensabile: se $E_1$ ed $E_2$ hanno elementi in comune, gli elementi condivisi verrebbero contati **due volte**.

**Principio del prodotto.** Se un oggetto si costruisce in due fasi indipendenti, con $m$ possibilità per la prima e $n$ per la seconda: $|E| = m \cdot n$.

> 💡 In catena: con $n_1, n_2, \dots, n_k$ possibilità si ottiene $n_1 \cdot n_2 \cdots n_k$.

---

## Disposizioni

Le disposizioni sono scelte **ordinate**, in cui gli elementi **non** si ripetono.

$$D_{n,k} = \frac{n!}{(n-k)!} = n(n-1)\cdots(n-k+1)$$

> 💡 **Perché questa formula.** Il fattoriale $\frac{n!}{(n-k)!}$ è il prodotto dei primi $k$ numeri a partire da $n$: si sceglie il primo elemento in $n$ modi, il secondo in $n-1$, e così via. Equivale a $\binom{n}{k} \cdot k!$.

**Verificato:** $D_{5,3} = \frac{5!}{2!} = 60$, e il conteggio diretto dà $60$ ✅

### Disposizioni con ripetizione

$$D^r_{n,k} = n^k$$

Ogni posizione si sceglie **indipendentemente**: $n$ scelte per $k$ posti.

**Verificato:** $D^r_{5,3} = 5^3 = 125$ ✅

### Permutazioni e anagrammi

Le disposizioni di $n$ elementi su $n$ posti sono le **permutazioni**: $n!$, cioè le $n!$ biiezioni di un insieme in sé (il gruppo $S_n$).

Se una parola di $n$ lettere ha $r_1$ occorrenze di una lettera, $r_2$ di un'altra, e così via:

$$\text{anagrammi} = \frac{n!}{r_1! \, r_2! \cdots r_k!}$$

> ⚠️ **Perché si divide.** Le $n!$ permutazioni "distinte" non lo sono: scambiare due $M$ produce la stessa parola. Ogni lettera ripetuta produce $r_i!$ sovrabbondanze, e si divide per eliminarle.

**Verificato con "MAMMA"**: $n=5$, con $3$ lettere $M$ e $2$ lettere $A$.

$$\frac{5!}{3!\,2!} = \frac{120}{12} = \mathbf{10}$$

Il conteggio diretto dà esattamente $10$: AAMMM, AMAMM, AMMAM, AMMMA, MAAMM, MAMAM, MAMMA, MMAAM, MMAMA, MMMAA ✅

> 💡 **Il conto in un attimo**: si scelgono le **posizioni** delle $M$, cioè $\binom{5}{3} = 10$. Le combinazioni danno lo stesso risultato.

---

## Combinazioni

Le combinazioni sono scelte **senza ordine**: conta solo **quali** elementi si scelgono.

$$C_{n,k} = \binom{n}{k} = \frac{n!}{k!\,(n-k)!}$$

> 💡 **Perché compare $k!$.** Le disposizioni contano anche l'ordine; ogni combinazione è stata contata $k!$ volte. Dividendo si ottiene il conteggio senza ordine.

**Verificato:** $C_{5,3} = \binom{5}{3} = 10$ ✅

### Combinazioni con ripetizione

$$C^r_{n,k} = \binom{n+k-1}{k}$$

Il nome **"stelle e barre"** aiuta: $k$ stelle distribuite fra $n$ barre.

**Verificato:** $C^r_{5,3} = \binom{7}{3} = 35$ ✅

---

## Riepilogo: le quattro formule a confronto

| | Ordine conta? | Ripetizioni | Formula | $n=5, k=3$ |
|---|---|---|---|---|
| Disposizioni semplici | ✅ | ❌ | $\dfrac{n!}{(n-k)!}$ | $60$ |
| Disposizioni con ripetizione | ✅ | ✅ | $n^k$ | $125$ |
| Combinazioni semplici | ❌ | ❌ | $\binom{n}{k}$ | $10$ |
| Combinazioni con ripetizione | ❌ | ✅ | $\binom{n+k-1}{k}$ | $35$ |

> ⚠️ **L'errore più comune è confondere le colonne.** Le combinazioni semplici danno $10$, le disposizioni semplici $60$: il rapporto è $k! = 6$. Se il risultato ti sembra "troppo grande", hai probabilmente contato l'ordine quando non andava contato.



---

## Il binomio di Newton e il triangolo di Pascal

$$(X + Y)^n = \sum_{k=0}^{n} \binom{n}{k} X^{n-k} Y^k$$

**Verificato** per $n = 4$:

$$(X+Y)^4 = X^4 + 4X^3Y + 6X^2Y^2 + 4XY^3 + Y^4$$

e la somma con i binomi dà esattamente lo stesso polinomio ✅

### Triangolo di Pascal-Tartaglia

Ogni elemento è la **somma dei due sopra**; i bordi sono sempre $1$.

| $n$ \ $k$ | 0 | 1 | 2 | 3 | 4 | 5 | 6 |
|---|---|---|---|---|---|---|---|
| 0 | 1 | | | | | | |
| 1 | 1 | 1 | | | | | |
| 2 | 1 | 2 | 1 | | | | |
| 3 | 1 | 3 | 3 | 1 | | | |
| 4 | 1 | 4 | 6 | 4 | 1 | | |
| 5 | 1 | 5 | 10 | 10 | 5 | 1 | |
| 6 | 1 | 6 | 15 | 20 | 15 | 6 | 1 |

> 💡 **Il triangolo si costruisce da sinistra a destra**, mentre il binomio di Newton si legge **da destra a sinistra** (partendo da $X^n$ e scambiando $X$ con $Y$ a ogni passo).
>
> 💡 **Serve a risparmiare i calcoli.** Se compare $\binom{20}{3}$, costruire le prime righe dà il risultato senza fare prodotti enormi.

---

## Inclusione-esclusione

Per contare l'unione di $k$ insiemi si **alternano** somme e sottrazioni delle intersezioni:

$$|A_1 \cup \cdots \cup A_k| = \sum_i |A_i| - \sum_{i<j} |A_i \cap A_j| + \sum_{i<j<l} |A_i \cap A_j \cap A_l| - \dots$$

Per due insiemi:

$$|A \cup B| = |A| + |B| - |A \cap B|$$

> ⚠️ **Perché si sottrae l'intersezione.** Nella somma $|A| + |B|$ gli elementi comuni sono stati contati **due volte**; sottraendo $|A \cap B|$ si torna a contarli una volta sola.
>
> 💡 È il **principio di correzione degli errori**: ogni volta che si sommano insiemi che si sovrappongono, si sottrae quanto è stato contato in eccesso. È la ragione dell'aspetto alternata della formula.

---

## Esercizi

| # | Problema | Risposta |
|---|---|---|
| 1 | Disposizioni semplici di 6 oggetti, 4 posti | ❓ |
| 2 | Combinazioni semplici di 8 elementi, 3 scelti | ❓ |
| 3 | Disposizioni con ripetizione di 4 lettere su 3 posti | ❓ |
| 4 | Anagrammi distinti di "BANANA" | ❓ |
| 5 | Combinazioni con ripetizione di 4 tipi, 3 scelti | ❓ |
| 6 | Coefficienti di $(X+1)^6$ | ❓ |
| 7 | $\lvert A \cup B\rvert$ con $\lvert A\rvert = 12$, $\lvert B\rvert = 7$, $\lvert A \cap B\rvert = 4$ | ❓ |

<details>
<summary>Soluzioni verificate</summary>

| # | Sviluppo | Risposta |
|---|---|---|
| 1 | $D_{6,4} = \dfrac{6!}{2!} = \dfrac{720}{2}$ | $360$ ✅ |
| 2 | $C_{8,3} = \binom{8}{3} = \dfrac{8 \cdot 7 \cdot 6}{3 \cdot 2 \cdot 1}$ | $56$ ✅ |
| 3 | $D^r_{4,3} = 4^3$ | $64$ ✅ |
| 4 | B,A,N,A,N,A ⟹ $n=6$, $A:3$, $N:2$, $B:1$: $\dfrac{6!}{3!\,2!\,1!} = \dfrac{720}{12}$ | $60$ ✅ |
| 5 | $C^r_{4,3} = \binom{6}{3}$ | $20$ ✅ |
| 6 | 6ª riga del triangolo di Pascal | $1, 6, 15, 20, 15, 6, 1$ ✅ |
| 7 | $12 + 7 - 4$ | $15$ ✅ |

</details>

> 💡 **L'esercizio 4** è l'esempio classico: "BANANA" ha $6$ lettere con $A$ ripetuta $3$ volte e $N$ ripetuta $2$ volte. Il risultato è $\frac{6!}{3!\,2!} = 60$, **non** $6! = 720$.
>
> ⚠️ **L'esercizio 2** è l'errore da non fare: $\binom{8}{3} = 56$ e **non** $8^3 = 512$. Se ottieni $512$, hai usato la formula delle disposizioni con ripetizione.

---

## Test di autovalutazione

**Parte A — teoria.**

| # | Domanda | Risposta attesa |
|---|---|---|
| 1 | Enunciate il **principio della somma** | $\lvert E\rvert = \lvert E_1\rvert + \lvert E_2\rvert$ per $E_1, E_2$ **disgiunti** |
| 2 | Perché la disgiunzione è indispensabile? | altrimenti gli elementi comuni sarebbero contati **due volte** |
| 3 | Formula delle disposizioni semplici | $D_{n,k} = \dfrac{n!}{(n-k)!}$ |
| 4 | Formula delle disposizioni con ripetizione | $D^r_{n,k} = n^k$ |
| 5 | Formula delle combinazioni semplici | $C_{n,k} = \binom{n}{k} = \dfrac{n!}{k!(n-k)!}$ |
| 6 | Come si contano gli anagrammi con lettere ripetute? | $\dfrac{n!}{r_1!\,r_2!\cdots r_k!}$ |
| 7 | Enunciate il **binomio di Newton** | $(X+Y)^n = \sum_{k=0}^{n}\binom{n}{k}X^{n-k}Y^k$ |
| 8 | Come si costruisce una riga del triangolo di Pascal? | ogni elemento è la **somma dei due** sopra; i bordi sono $1$ |
| 9 | Perché in $\lvert A \cup B\rvert = \lvert A\rvert + \lvert B\rvert - \lvert A \cap B\rvert$ si sottrae? | perché gli elementi comuni sono stati contati **due volte** |

**Parte B — distinguere le formule.**

| # | Situazione | Formula |
|---|---|---|
| 1 | 3 primi posti di una gara, con distacco | ❓ |
| 2 | 3 premi a 10 concorrenti, un premio ciascuno | ❓ |
| 3 | password di 4 caratteri da 8 lettere, ripetizioni ammesse | ❓ |
| 4 | 3 birre fra 6 tipi, ripetizioni ammesse | ❓ |

<details>
<summary>Soluzioni</summary>

| # | Perché | Formula | Risposta |
|---|---|---|---|
| 1 | l'ordine conta (1ª, 2ª, 3ª), nessuna ripetizione | disposizioni semplici | $D_{5,3} = \dfrac{5!}{2!} = 60$ |
| 2 | l'ordine **non** conta (il vincitore di A è diverso da quello di B) | combinazioni semplici | $C_{10,3} = 120$ |
| 3 | l'ordine conta (la sequenza **è** la password) e si ripetono | disposizioni con ripetizione | $D^r_{8,4} = 8^4 = 4096$ |
| 4 | l'ordine **non** conta e si ripetono | combinazioni con ripetizione | $C^r_{6,3} = \binom{8}{3} = 56$ |

</details>

> ⚠️ **Il caso 1 e il caso 2 sono la coppia da non confondere.** Se nell'oggetto 1 non si dicesse "con distacco", e i primi tre posti fossero semplicemente tre persone ammesse, la risposta cambierebbe da $60$ a $C_{5,3} = 10$. **È la formulazione del testo a decidere**, non l'oggetto.

---

## Link

- [[Indice - Matematica Discreta, Algebra e Geometria]] — l'indice del corso
- [[Programma - Matematica Discreta, Algebra e Geometria]] — programma e formule chiave
- [[1.1 Elementi di Teoria degli Insiemi e Logica]] — cardinalità, insieme delle parti e partizioni