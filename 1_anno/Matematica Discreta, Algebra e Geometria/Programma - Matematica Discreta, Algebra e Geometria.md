> [!info] Programma ufficiale del corso
> Le note di studio sono in [[Indice - Matematica Discreta, Algebra e Geometria]] · la mappa di tutti i corsi è in [[Indice generale]]

# Matematica Discreta, Algebra e Geometria (12 CFU) - Guida all'Insegnamento

## 1. Informazioni Generali e Importanza
* **Codice Attività Didattica:** INF0328
* **Crediti Formativi (CFU):** 12 CFU (64 ore di lezioni frontali + 40 ore di esercitazioni)
* **Settore Scientifico-Disciplinare (SSD):** MAT/02 (Algebra) e MAT/03 (Geometria)
* **Periodo:** Primo anno, 1° semestre
* **Tipologia:** Insegnamento di base | **Frequenza:** Facoltativa (consigliata)
* **Importanza nel Corso di Studi:** È uno dei due esami di matematica fondamentali del primo anno (insieme ad Analisi Matematica). Fornisce il linguaggio logico-formale, le strutture algebriche e l'algebra lineare necessarie per comprendere i modelli teorici dell'informatica, la crittografia, la grafica vettoriale, la teoria dei grafi e gli algoritmi avanzati.

---

## 2. Prerequisiti
* Conoscenze matematiche di base della scuola secondaria di secondo grado:
  * Operazioni aritmetiche fondamentali e proprietà delle potenze.
  * Equazioni e disequazioni di primo e secondo grado.
  * Concetti elementari di logica e terminologia (proposizioni, quantificatori).
* **Insegnamenti propedeutici obbligatori:** Nessuno.
* **Nota:** Eventuali lacune di calcolo algebrico iniziale possono essere colmate tramite il *Corso di Riallineamento di Matematica* sulla piattaforma Orient@mente (OFA).

---

## 3. Obiettivi Formativi e Risultati di Apprendimento
L'insegnamento sviluppa le competenze necessarie per manipolare oggetti discreti e strutture vettoriali:
* **Matematica Discreta & Algebra:** Familiarità con insiemi, relazioni, funzioni, combinatoria, strutture algebriche (gruppi, anelli, campi) ed aritmetica modulare (utilissima per la sicurezza informatica e la crittografia).
* **Algebra Lineare & Geometria:** Capacità di operare con vettori, matrici, trasformazioni lineari, calcolo di autovalori/autovettori e risoluzione di sistemi lineari interpretandoli geometricamente (rette, piani, iperpiani).

---

## 4. Programma Dettagliato degli Argomenti

### Modulo A: Matematica Discreta e Algebra

1. **Linguaggio degli Insiemi, Relazioni e Funzioni:**
   * Insiemi: insieme vuoto, sottoinsiemi, unione, intersezione, complementare, insieme delle parti $\mathcal{P}(X)$.
   * Relazioni d'ordine, relazioni di equivalenza e partizioni di insiemi.
   * Corrispondenze e funzioni: composizione, inversione, iniettività, suriettività e biiettività.

2. **Calcolo Combinatorio:**
   * Cardinalità di insiemi finiti, principi fondamentali della somma e del prodotto.
   * Disposizioni e combinazioni (semplici e con ripetizione).
   * Teorema del binomio di Newton, triangolo di Pascal-Tartaglia e principio di inclusione-esclusione.

3. **Strutture Algebriche:**
   * Semigruppi, monoidi (monoide delle parole) e gruppi con relativi morfismi.
   * Esempi di strutture: numeri naturali $\mathbb{N}$, interi $\mathbb{Z}$, gruppo delle biiezioni.
   * Gruppi e sottogruppi ciclici, Teorema di Lagrange.
   * Corpi e campi: struttura del campo dei numeri razionali $\mathbb{Q}$.

4. **Aritmetica Modulare:**
   * Anelli degli interi $\mathbb{Z}$ e delle classi di resto $\mathbb{Z}_n$.
   * Teorema della divisione ed algoritmo di Euclide per il M.C.D.
   * Identità di Bézout ed equazioni diofantee lineari.
   * Congruenze lineari e Teorema di Eulero-Fermat.

5. **Gruppo delle Permutazioni:**
   * Composizione, potenze e inverse di permutazioni.
   * Decomposizione in cicli disgiunti e decomposizione in trasposizioni.
   * Parità di una permutazione e sottogruppi del gruppo delle permutazioni.

---

### Modulo B: Algebra Lineare e Geometria

1. **Numeri e Spazi Vettoriali:**
   * Richiami su polinomi, numeri reali $\mathbb{R}$ e numeri complessi $\mathbb{C}$.
   * Spazi vettoriali e spazi Euclidei: combinazioni lineari, indipendenza lineare, basi e dimensione.
   * **Formula di Grassmann:** $\dim(U + W) = \dim U + \dim W - \dim(U \cap W)$.

2. **Sistemi Lineari e Matrici:**
   * Sistemi di equazioni lineari e matrice associata.
   * Algoritmo di riduzione di Gauss-Jordan.
   * Teorema di Rouché-Capelli e struttura dello spazio delle soluzioni.
   * Algebra delle matrici, **matrici simmetriche e antisimmetriche**, determinante (sviluppo di Laplace, **regola di Binet**, calcolo dell'inversa).

3. **Geometria Analitica e Affine:**
   * Interpretazione geometrica di rette, piani e iperpiani (lineari e affini) in $\mathbb{R}^n$.
   * Rappresentazione in forma parametrica e cartesiana.
   * Condizioni di **parallelismo** e **incidenza**.

4. **Applicazioni Lineari e Diagonalizzazione:**
   * Applicazioni lineari tra spazi vettoriali: Nucleo ($\ker$) e Immagine ($\text{Im}$).
   * **Teorema della Dimensione:** $\dim V = \dim \ker f + \dim \operatorname{Im} f$.
   * Matrice associata a un'applicazione lineare, cambiamento di base e matrici simili.
   * Polinomio caratteristico $p(\lambda) = \det(A - \lambda I)$, autovalori e **autospazi** $V_\lambda = \ker(A - \lambda I)$.
   * Distinzione fra **molteplicità algebrica** $m_a(\lambda)$ e **geometrica** $m_g(\lambda)$; condizioni per la diagonalizzazione.

5. **Prodotti Scalari e Forme Quadratiche:**
   * Prodotti scalari, norma di un vettore, ortogonalità e complemento ortogonale $W^\perp$.
   * **Algoritmo di Gram-Schmidt** e basi ortonormali.
   * Forme quadratiche: definite, semidefinite, indefinite.
   * **Teorema Spettrale:** ogni matrice reale e simmetrica è diagonalizzabile tramite una matrice ortogonale.

---

## 5. Modalità d'Esame e Valutazione
* **Articolazione in Due Parti:** L'esame si compone di **due prove scritte indipendenti**:
  1. Parte di **Matematica Discreta**.
  2. Parte di **Algebra Lineare e Geometria**.
* **Flessibilità degli Appelli:** È possibile sostenere le due parti in appelli o sessioni differenti nello stesso anno accademico.
* **Tipologia della Prova:** Prova scritta contenente sia quesiti teorici (definizioni, enunciati e dimostrazioni) sia esercizi applicativi/numerici.
* **Calcolo del Voto Finale:** Espresso in trentesimi ($0 - 30$), calcolato come **media aritmetica** dei punteggi ottenuti nelle due parti scritte.

---

## Formule chiave, verificate

Sono quelle che compaiono più spesso nei compiti. Ognuna è stata controllata con il calcolo simbolico.

### Parte A — Matematica Discreta

| Argomento | Formula | Verifica |
|---|---|---|
| Eulero-Fermat | se $\gcd(a,n)=1$ allora $a^{\varphi(n)} \equiv 1 \pmod n$ | $\varphi(7)=6$ e $3^6 - 1 = 728 = 104 \cdot 7$ ✅ |
| CRT | $x \equiv 3 \pmod 7$, $x \equiv 4 \pmod{11} \Rightarrow x \equiv 59 \pmod{77}$ | $59 \bmod 7 = 3$ ✅ · $59 \bmod 11 = 4$ ✅ |
| Lagrange | $\lvert H\rvert$ divide $\lvert G\rvert$ se $H \subseteq G$ finito | — |
| Alterno | $A_n$ è il sottogruppo delle permutazioni di **parità pari** | — |

### Parte B — Algebra Lineare e Geometria

| Argomento | Formula | Verifica |
|---|---|---|
| Grassmann | $\dim(U+W) = \dim U + \dim W - \dim(U \cap W)$ | con $\dim U = 2$, $\dim W = 2$, $\dim(U \cap W) = 1$: risultato $3$ ✅ |
| Dimensione | $\dim V = \dim \ker f + \dim \operatorname{Im} f$ | $f : \mathbb{R}^3 \to \mathbb{R}^2$ con $\dim \ker = 1$, $\dim \operatorname{Im} = 2$: somma $3$ ✅ |
| Polinomio caratteristico | $p(\lambda) = \det(A - \lambda I)$ | per $A = \begin{pmatrix} 2 & 1 \\ 0 & 3\end{pmatrix}$: $p(\lambda) = \lambda^2 - 5\lambda + 6$ ✅ |
| Autospazio | $V_\lambda = \ker(A - \lambda I)$ | per $\lambda = 2$: $V_2 = \text{span}\{(1,0)\}$, dunque $m_g(2) = 1$ ✅ |
| Gram-Schmidt | $u_2 = w - \text{proiezione di } w \text{ su } u_1$ | con $v = (1,1,1)$, $w = (1,0,0)$: proiezione $\left(\tfrac13, \tfrac13, \tfrac13\right)$, $u_2 = \left(\tfrac23, -\tfrac13, -\tfrac13\right)$ con $v \cdot u_2 = 0$ ✅ |

> ⚠️ **Molteplicità algebrica e geometrica.** $m_a(\lambda)$ è quante volte $\lambda$ compare nel polinomio caratteristico; $m_g(\lambda)$ è la dimensione dell'autospazio $V_\lambda$. Vale sempre $m_g(\lambda) \leq m_a(\lambda)$, e una matrice è **diagonalizzabile** se e solo se $m_g(\lambda) = m_a(\lambda)$ per ogni autovalore.

---

## Consiglio strategico

Le due parti dell'esame si possono sostenere **separatamente**: conviene concentrarsi prima su **Matematica Discreta**, che si collegano direttamente a [[Programma - Fondamenti dell'Informatica]], e poi affrontare Algebra Lineare con una base computazionale già solida.

| Fase | Argomenti | Perché |
|---|---|---|
| 1ª | insiemi, relazioni, funzioni | è il ponte con l'OFA e con l'informatica |
| 2ª | aritmetica modulare, permutazioni | serve per crittografia e sicurezza |
| 3ª | strutture algebriche, gruppi | è la parte più astratta |
| 4ª | algebra lineare, geometria | ha bisogno del calcolo maturato prima |

> 💡 **I primi tre moduli dell'OFA (linguaggio, numeri, fattorizzazione) sono l'unico ponte fra i due corsi.** Insiemi, relazioni e funzioni compaiono sia nella Parte A dell'esame sia nel Modulo 1 dell'OFA: quel materiale è già scritto e verificato in [[1.1 Elementi di Teoria degli Insiemi e Logica]].

---

## 6. Testi Consigliati e Materiale Didattico
* **Matematica Discreta:** 
  * A. Mori, *Lezioni di Matematica Discreta* (CreateSpace Independent Publishing Platform).
  * A. Facchini, *Algebra e Matematica discreta* (Zanichelli/Decibel).
  * J. R. Durbin, *Modern Algebra: an introduction* (John Wiley & Sons).
* **Algebra Lineare e Geometria:**
  * S. Lang, *Algebra Lineare* (Bollati Boringhieri).
  * B. Martelli, *Geometria e algebra lineare*, dispense del corso (disponibili in PDF).
* **Materiale online:** Dispense, eserciziari con soluzioni e test di autovalutazione pubblicati dai docenti sulla piattaforma Moodle dell'Ateneo.
* **Materiale degli studenti:** prove d'esame degli anni passati **con le soluzioni**, formulari e appunti sono raccolti nel repository del Team Studentesco Informatica e sono indicati in [[Risorse esterne]]. Non sono materiale ufficiale: vanno usati come riferimento per capire il taglio dell'esame, non come autorità.
