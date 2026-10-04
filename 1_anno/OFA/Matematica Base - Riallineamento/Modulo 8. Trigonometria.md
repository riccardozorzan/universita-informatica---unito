# Modulo 8. Trigonometria

> [!info] Nota in corso
> Materiale del **Modulo 8** del Corso di Riallineamento di Matematica (Orient@mente).
> Indice del percorso: [[Indice - Matematica Base]] · Indice OFA: [[Indice - OFA]]

| | |
|---|---|
| **Modulo** | 8 |
| **Argomenti** | circonferenza goniometrica, funzioni trigonometriche, equazioni e disequazioni trigonometriche, applicazioni ai triangoli |
| **Materiali su Orient@mente** | 2 libri · 2 worksheet Maple T.A. · 3 pagine · 4 file · 3 compiti |
| **Stato** | ✅ **8.1 e 8.2 complete** |

---

## Teoria

### 8.1 Funzioni trigonometriche

✅ [[8.1 Funzioni Trigonometriche]] — **completa**, con i 4 esercizi ufficiali verificati.

**Prima di tutto, due definizioni di base:**

| Concetto | Definizione |
|---|---|
| **circonferenza goniometrica** | circonferenza di centro l'origine e raggio $r = 1$ |
| **radiante** | l'angolo al centro che sottende un arco di lunghezza **pari al raggio** |

$$\theta : 360^\circ = \rho : 2\pi \qquad 360^\circ = 2\pi \text{ radianti}$$

Le **4 funzioni**, definite sulla circonferenza di raggio 1:

| Funzione | Definizione | Dominio |
|---|---|---|
| $\sin\theta$ | ordinata del punto $P$ | tutto $\mathbb{R}$ |
| $\cos\theta$ | ascissa del punto $P$ | tutto $\mathbb{R}$ |
| $\tan\theta$ | $\dfrac{\sin\theta}{\cos\theta}$ | $\mathbb{R}\setminus\{\frac\pi2+k\pi\}$ ⚠️ |
| $\cot\theta$ | $\dfrac{\cos\theta}{\sin\theta}$ | $\mathbb{R}\setminus\{k\pi\}$ ⚠️ |

**Le proprietà dei grafici**, da sapere a memoria:

| | periodo | limitate | codominio | parità |
|---|---|---|---|---|
| $\sin x$ | $2\pi$ | ✅ $[-1,1]$ | $[-1,1]$ | dispari |
| $\cos x$ | $2\pi$ | ✅ $[-1,1]$ | $[-1,1]$ | pari |
| $\tan x$ | $\pi$ ⚠️ | ❌ no | $\mathbb{R}$ | dispari |
| $\cot x$ | $\pi$ | ❌ no | $\mathbb{R}$ | dispari |

> ⚠️ **Tre punti che i test sfruttano:**
> - la **relazione fondamentale** $\sin^2\theta+\cos^2\theta=1$ dà il valore **assoluto**: il segno si legge dal **quadrante**
> - il periodo di $\tan$ e $\cot$ è $\pi$, non $2\pi$
> - i **domini** di tangente e cotangente sono diversi: $\frac\pi2+k\pi$ contro $k\pi$

**Le formule**, raggruppate per uso:

| Famiglia | Formule |
|---|---|
| simmetria | $\sin(\pi-\theta)=\sin\theta$ · $\sin(-\theta)=-\sin\theta$ · $\sin(\frac\pi2-\theta)=\cos\theta$ |
| fondamentale | $\sin^2\theta+\cos^2\theta=1$ |
| addizione | $\sin(\theta_1\pm\theta_2)=\sin\theta_1\cos\theta_2\pm\cos\theta_1\sin\theta_2$ |
| duplicazione | $\sin 2\theta = 2\sin\theta\cos\theta$ · $\cos 2\theta = \cos^2\theta-\sin^2\theta$ |
| bisezione | $\sin^2\frac\theta2 = \frac{1-\cos\theta}{2}$ |

**Gli angoli notevoli**, da memorizzare solo $30^\circ$ e $45^\circ$:

| $\theta$ | $30^\circ$ | $45^\circ$ | $60^\circ$ | $90^\circ$ |
|---|---|---|---|---|
| $\sin\theta$ | $\frac12$ | $\frac{\sqrt2}{2}$ | $\frac{\sqrt3}{2}$ | $1$ |
| $\cos\theta$ | $\frac{\sqrt3}{2}$ | $\frac{\sqrt2}{2}$ | $\frac12$ | $0$ |

---

## Esercizi

**Esercizi ufficiali** (file *Ulteriori esercizi sulle funzioni trigonometriche*): i **4 esercizi con le soluzioni**, dentro [[8.1 Funzioni Trigonometriche]], tutti riverificati con SymPy.

| # | Esercizio | Il punto di attenzione |
|---|---|---|
| 1 | 7 valori esatti | $\cos 22{,}5^\circ = \frac{\sqrt{2+\sqrt2}}{2}$, non $\frac{2\sqrt2}{2}$ |
| 2 | Verificare 3 identità | sono **tutte vere**; (b) si riconosce come $\sin(2x-x)$ |
| 3 | $\cot\alpha$ con $\sin\alpha = \frac35$ | la condizione $0<\alpha<\frac\pi2$ **fissa il segno** del coseno |
| 4 | Grafici e periodi | il fattore **fuori** dall'argomento non cambia il periodo |

> 💡 **Il criterio per il periodo**, dai risultati dell'Esercizio 4: in $y = h\sin(kx)$ il periodo è $\frac{2\pi}{|k|}$. Il fattore $h$ cambia l'ampiezza, $k$ cambia la frequenza.

---

### 8.2 Equazioni e disequazioni trigonometriche

✅ [[8.2 Equazioni e Disequazioni Trigonometriche]] — **completa**, con i 10 esercizi ufficiali verificati.

**Le 3 equazioni fondamentali**, da applicare quando la stessa funzione compare a entrambi i membri:

| Funzione | Condizione | Periodo |
|---|---|---|
| $\sin\alpha = \sin\beta$ | $\alpha = \beta + 2k\pi$ oppure $\alpha = \pi - \beta + 2k\pi$ (**supplementari**) | $2\pi$ |
| $\cos\alpha = \cos\beta$ | $\alpha = \beta + 2k\pi$ oppure $\alpha = -\beta + 2k\pi$ (**opposti**) | $2\pi$ |
| $\tan\alpha = \tan\beta$ | $\alpha = \beta + k\pi$ (**un solo caso**) ⚠️ | $\pi$ |

> ⚠️ **Le tre righe non si scambiano.** "Supplementari" per il seno, "opposti" per il coseno, e la tangente ha un caso solo perché il periodo è $\pi$.

**Le equazioni elementari**, con i vincoli da controllare:

| Equazione | Condizione di esistenza | Soluzioni |
|---|---|---|
| $\sin x = c$ | $-1 \leq c \leq 1$ ⚠️ | $x = \alpha + 2k\pi$ oppure $x = \pi - \alpha + 2k\pi$ |
| $\cos x = c$ | $-1 \leq c \leq 1$ ⚠️ | $x = \pm\alpha + 2k\pi$ |
| $\tan x = c$ | $x \neq \frac\pi2 + k\pi$ | $x = \alpha + k\pi$ |

**I triangoli**, dove la trigonometria serve a trovare gli elementi ignoti:

| Contesto | Formule |
|---|---|
| rettangolo | $a = c\sin\alpha = c\cos\beta$ · $a = b\tan\alpha$ |
| **Carnot** | $a^2 = b^2+c^2-2bc\cos\alpha$ |
| **seni** | $a:\sin\alpha = b:\sin\beta = c:\sin\gamma$ |

> 💡 **Il teorema dei seni** risolve i triangoli **non rettangoli**: con un rapporto noto si trovano gli altri due lati.

---

## Test di autovalutazione

*(da scrivere)*

---

## Link

- [[Indice - Matematica Base]]
- [[6.1 Definizione di Funzione e Principali Caratteristiche]] — le proprietà delle funzioni, da cui parte l'analisi dei grafici
