# Modulo 7. Esponenziali e Logaritmi

> [!info] Nota in corso
> Materiale del **Modulo 7** del Corso di Riallineamento di Matematica (Orient@mente).
> Indice del percorso: [[Indice - Matematica Base]] · Indice OFA: [[Indice - OFA]]

| | |
|---|---|
| **Modulo** | 7 |
| **Argomenti** | esponenziali e logaritmi, equazioni e disequazioni corrispondenti, modellazione di fenomeni reali |
| **Materiali su Orient@mente** | 2 libri · 2 worksheet Maple T.A. · 3 pagine · 4 file · 3 compiti |
| **Stato** | ✅ **7.1 e 7.2 complete** |

---

## Teoria

### 7.1 Esponenziali e logaritmi

✅ [[7.1 Esponenziali e Logaritmi]] — **completa**, con i 3 esercizi ufficiali verificati.

Le **3 parti** del sommario, e la distinzione che le governa:

| # | Parte | Oggetto |
|---|---|---|
| 1 | **Esponenziale** | $y = a^x$ |
| 2 | **Logaritmo** | $\log_a k$ e le sue proprietà |
| 3 | **Legame fra le due** | sono l'una l'inversa dell'altra |

> ⚠️ **La trappola dell'intero modulo:** $a^x$ (la $x$ è **l'esponente**) è diverso da $x^a$ (la $x$ è **la base**). Sono due famiglie di funzioni diverse: $x^2$ non è definita per $x<0$ e non è definita in $0$, $2^x$ invece lo è ovunque.

**Le condizioni sulla base** ($a>0$, $a \neq 1$) si spiegano passo per passo, e la condizione $a>0$ emerge proprio al **3° passaggio** dell'estensione degli esponenti, quello **razionale**: con $n$ pari si deve calcolare $\sqrt[n]{a^m}$, che in $\mathbb{R}$ richiede argomento positivo.

**Le caratteristiche a confronto**, da sapere a memoria:

| | $a^x$ | $\log_a x$ |
|---|---|---|
| dominio | $\mathbb{R}$ | $\mathbb{R}^+$ ⚠️ |
| punto fisso | $(0,1)$ | $(1,0)$ |
| $a > 1$ | crescente | crescente |
| $0 < a < 1$ | decrescente | decrescente |

> 💡 **I due punti fissi sono scambiati** perché le due funzioni sono inverse: si scambiano dominio e codominio. I grafici sono simmetrici rispetto alla bisettrice del I e III quadrante ($y=x$).

**La Nota 7.1**: $e \approx 2{,}71828$ (numero di Nepero, da cui il nome), $\ln(1+y) \sim y$, e la base $10$ con **caratteristica** (parte intera) e **mantissa** (parte decimale). Proprietà che **valgono solo in base 10**: $1325$ e $13{,}25$ hanno la stessa mantissa ma caratteristica diversa di $2$.

---

### 7.2 Equazioni e disequazioni esponenziali e logaritmiche

✅ [[7.2 Equazioni e Disequazioni Esponenziali e Logaritmiche]] — **completa**, con i 10 esercizi ufficiali verificati.

Le **4 parti** del sommario, tutte costruite sulla stessa idea: **trasformare finché la $x$ esce dalle funzioni**.

| # | Parte | Tipo |
|---|---|---|
| 1 | **Equazioni esponenziali** | la $x$ all'esponente |
| 2 | **Equazioni logaritmiche** | la $x$ nell'argomento |
| 3 | **Disequazioni esponenziali** | idem, con disuguaglianza |
| 4 | **Disequazioni logaritmiche** | idem, con disuguaglianza |

**Le 3 regole che risolvono quasi tutto il modulo:**

| Situazione | Regola |
|---|---|
| stessa base $a>1$ | si confrontano gli esponenti/argomenti, **verso mantenuto** |
| stessa base $0<a<1$ | si confrontano gli esponenti/argomenti, **verso invertito** ⚠️ |
| basi diverse | si applica il logaritmo (in base $c>1$, così il verso non si altera) |

> ⚠️ **L'errore più grave: dimenticare l'inversione con $0<a<1$.** Vale sia per gli esponenziali sia per i logaritmi, perché le due funzioni hanno la stessa monotonia.

**Esercizi ufficiali** (file *Ulteriori esercizi su equazioni e disequazioni*): i **10 esercizi con le soluzioni**, dentro [[7.2 Equazioni e Disequazioni Esponenziali e Logaritmiche]], tutti riverificati con SymPy.

| # | Esercizi | Tipo |
|---|---|---|
| 1-5 | risolvere 5 equazioni | basi uguali, basi diverse, logaritmi |
| 6-10 | risolvere 5 disequazioni | inversione del verso, condizioni di esistenza |

> ⚠️ **Due soluzioni del file ufficiale sono errate** (esercizi 6 e 7), documentate e corrette nella lezione con la verifica numerica.

**Applicazioni 7.2:** il pH, cioè $\text{pH} = -\log_{10}[H^+]$. Noto il pH, la concentrazione si ottiene risolvendo l'equazione logaritmica inversa.

---

## Test di autovalutazione

*(da scrivere)*

---

## Link

- [[Indice - Matematica Base]]
- [[6.1 Definizione di Funzione e Principali Caratteristiche]] — le proprietà delle funzioni, da cui si parte
- [[6.2 Esempi di Funzioni Utili]] — funzioni-esempio a cui fare riferimento
