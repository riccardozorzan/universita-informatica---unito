# Modulo 9. Statistica e Probabilità

> [!info] Nota in corso
> Materiale del **Modulo 9** del Corso di Riallineamento di Matematica (Orient@mente).
> Indice del percorso: [[Indice - Matematica Base]] · Indice OFA: [[Indice - OFA]]

| | |
|---|---|
| **Modulo** | 9 |
| **Argomenti** | statistica descrittiva, lettura e interpretazione dei dati, calcolo delle probabilità, calcolo combinatorio |
| **Materiali su Orient@mente** | 2 libri · **nessun worksheet Maple** · 2 pagine · 4 file · 3 compiti |
| **Stato** | ✅ **9.1 e 9.2 complete** |

> ⚠️ **Questo modulo non fa parte di nessuno dei 9 esami del primo anno**, come segnala l'indice del percorso. È il meno utile se devi colmare il debito OFA in fretta.

---

## Teoria

### 9.1 Statistica descrittiva

✅ [[9.1 Statistica Descrittiva]] — **completa**, con i 3 esercizi ufficiali verificati.

Le **4 parti** del sommario, e la distinzione che le governa:

| # | Parte | Oggetto |
|---|---|---|
| 1 | **Dati e terminologia** | unità, popolazione, campione, caratteri |
| 2 | **Tabelle di frequenze** | assolute, relative, percentuali |
| 3 | **Rappresentazioni grafiche** | barre, torta, dispersione, istogramma |
| 4 | **Indici di sintesi** | moda, media, mediana, varianza, scarto quadratico |

> ⚠️ **La distinzione che decide tutto**: carattere **qualitativo** (non misurabile, categorie) ⟹ barre o torta, e l'indice è la **moda**. Carattere **quantitativo** (misurabile) ⟹ dispersione o istogramma, e gli indici sono **media** e **mediana**.

**Le tre frequenze**, con la loro somma di controllo:

| Tipo | Definizione | Somma |
|---|---|---|
| **assoluta** $n_i$ | quante unità hanno quella modalità | $= N$ |
| **relativa** | $n_i \div N$ | $= 1$ |
| **percentuale** | $n_i \div N \times 100$ | $= 100$ |

**Gli indici di sintesi**, divisi per famiglia:

| Indice | Famiglia | Formula |
|---|---|---|
| **moda** | posizione | la modalità più frequente (può non esistere) |
| **media** $\bar{x}$ | posizione | $\frac{\sum_{i=1}^{N} x_i}{N}$ |
| **mediana** | posizione | centrale se $N$ dispari, media dei due centrali se $N$ pari |
| **varianza** | **dispersione** | $\frac{\sum_{i=1}^{N}(x_i-\bar{x})^2}{N}$ |
| **scarto quadratico medio** $\sigma$ | **dispersione** | $\sqrt{\text{Var}}$ |

> 💡 **Perché esiste lo scarto quadratico medio.** La varianza è in unità **quadrate**, quindi non è confrontabile con la media. La radice la riporta alle unità dei dati: la coppia $\bar{x} \pm \sigma$ descrive l'intera distribuzione in due numeri.

**Barre o istogramma?** La domanda più frequente nei test:

| | Barre | Istogramma |
|---|---|---|
|rettangoli | **separati** | **adiacenti** |
| grandezza letta | l'**altezza** | l'**area** |
| dato adatto | qualitativo | quantitativo |

---

## Esercizi

**Esercizi ufficiali** (file *Ulteriori esercizi sulla statistica descrittiva*): i **3 esercizi con le soluzioni**, dentro [[9.1 Statistica Descrittiva]], tutti riverificati con SymPy.

| # | Esercizio | Il punto di attenzione |
|---|---|---|
| 1 | Tre tabelle su 80 studenti | i totali devono tornare a $80$, $1$, $100\%$ |
| 2 | Diagramma a barre | le frequenze assolute sull'asse verticale |
| 3 | 4 indici su 6 dati | media $11{,}83$ · mediana $9{,}5$ · varianza $65{,}14$ · scarto $8{,}07$ |

> 💡 **L'Esercizio 3 mostra perché servono entrambi gli indici.** Il dato $28$ è un valore anomalo: la media sale a $11{,}83$ ma la mediana resta $9{,}5$. In presenza di dati anomali la mediana descrive il campione meglio.

---

### 9.2 Probabilità

✅ [[9.2 Probabilità]] — **completa**, con i 5 esercizi ufficiali verificati.

> 💡 **L'idea che governa il modulo**: **gli eventi sono insiemi**. Le formule sono conseguenze delle operazioni di [[1.1 Elementi di Teoria degli Insiemi e Logica]]: $p(E) + p(\bar{E}) = 1$ discende dal fatto che $E$ e $\bar{E}$ sono complementari in $\Omega$.

**Definizione classica**

$$p(E) = \frac{\text{favorevoli}}{\text{possibili}} = \frac{\lvert E \rvert}{\lvert \Omega \rvert} \qquad 0 \leq p(E) \leq 1$$

> ⚠️ **Condizione indispensabile**: tutti gli esiti devono essere **ugualmente possibili**, altrimenti la definizione non si applica.

**I 5 teoremi**, ciascuno con la sua condizione:

| Teorema | Formula | Quando |
|---|---|---|
| unione incompatibili | $p(E_1 \cup E_2) = p(E_1) + p(E_2)$ | $E_1 \cap E_2 = \emptyset$ |
| unione generale | $p(E_1 \cup E_2) = p(E_1) + p(E_2) - p(E_1 \cap E_2)$ | sempre |
| complementare | $p(\bar{E}) = 1 - p(E)$ | sempre |
| **condizionata** | $p(E_1 \mid E_2) = \frac{p(E_1 \cap E_2)}{p(E_2)}$ | $p(E_2) > 0$ |
| **indipendenza** | $p(E_1 \cap E_2) = p(E_1) \cdot p(E_2)$ ⇔ $p(E_1 \mid E_2) = p(E_1)$ | — |

> 💡 **La regola operativa, in una riga.** Eventi **indipendenti** ⟹ si **moltiplicano**. Eventi **dipendenti** ⟹ si moltiplica la prima per la seconda **condizionata**. Il difficile non è la formula: è stabilire **se** siano indipendenti.

**Calcolo combinatorio**, con la tabella che decide:

| Tipo | Ordine conta? | Tutti gli elementi? | Formula |
|---|---|---|---|
| **disposizioni** | ✅ | ❌ ($k$ su $n$) | $D(n,k) = \frac{n!}{(n-k)!}$ |
| **combinazioni** | ❌ **no** | ❌ ($k$ su $n$) | $C(n,k) = \frac{n!}{k!\,(n-k)!}$ |
| **permutazioni** | ✅ | ✅ (tutti gli $n$) | $P(n) = n!$ |

**La legge dei grandi numeri**, con l'avvertenza che viene quasi sempre male interpretata: la frequenza osservata converge alla probabilità teorica, ma **gli eventi indipendenti non hanno memoria**. Il $2$ che non è uscito in 100 lanci non diventa più probabile al lancio 101.

---

## Test di autovalutazione

*(da scrivere)*

---

## Link

- [[Indice - Matematica Base]]
- [[1.1 Elementi di Teoria degli Insiemi e Logica]] — gli eventi sono insiemi: unione, intersezione, complementare
- [[4.1 Equazioni e Disequazioni Fratte]] — la notazione delle frazioni usata nelle frequenze relative
