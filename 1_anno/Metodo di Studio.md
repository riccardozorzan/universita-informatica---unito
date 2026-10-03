# Metodo di Studio — Primo Anno Informatica

> [!tip] Come studiare, non cosa studiare
> Vale per **tutti** i corsi del primo anno: OFA, Matematica Discreta, Programmazione I, Fondamenti dell'Informatica, Analisi. Mappa dei corsi: [[Indice generale]]

Un metodo in **4 fasi**, pensato per materie scientifiche e informatiche, in cui la difficoltà è fare da soli sotto tempo.

---

## Fase 1 — Comprensione attiva e formulari personali

> **Non leggere mai passivamente.** La lettura riassuntiva non basta per la matematica o la programmazione.

Quando studi un teorema o un algoritmo, prendi foglio e penna e prova a **riscriverne la dimostrazione o il flusso del codice a libro chiuso**. Se non ci riesci, non l'hai capito: l'hai solo riconosciuto.

### La scheda delle strutture

Per le materie matematiche, dividi i fogli in **tre colonne**:

| Concetto / Teorema | Ipotesi e Tesi | Idea chiave / Trabocchetti |
|---|---|---|
| Rouché-Capelli | quando: sistema $Ax=b$; cosa dice: compatibilità ⟺ $rk(A) = rk(A\lvert b)$ | verificare **sempre** il rango della incompleta sia uguale a quello della completa |
| Formula ridotta del 2° grado | quando: se $b$ è pari; cosa dà: stesse radici, meno conti | il denominatore è $a$, **non** $2a$ |
| De Morgan | quando: per i complementari; cosa dà: $(A\cap B)^c = A^c\cup B^c$ | il complementare è definito **solo** rispetto a un universo $X$ |

> 💡 **Perché la terza colonna è la più importante.** Il concetto lo recuperi sul libro in tre minuti. Il trabocchetto lo impari **solo** sbagliando: è la colonna che ti evita il secondo errore.
>
> ⚠️ **Compilala man mano che sbagli**, non dopo. Nel momento dell'errore sai perché è successo; tre settimane dopo non lo ricordi più.

---

## Fase 2 — Pratica a cicli intervallati

### Active Recall

> Piuttosto che guardare le soluzioni degli esercizi svolti, tenta di risolverli **almeno 10-15 minuti da solo**.

L'accumulo di sforzo cognitivo è ciò che fissa il ragionaggio nella memoria a lungo termine. Lo sforzo non è un costo da minimizzare: **è il meccanismo**.

### Interleaving

> Non fare 20 esercizi tutti uguali di fila. **Alterna le tipologie.**

| # | Esercizio |
|---|---|
| 1 | matrici |
| 2 | sistemi di congruenze |
| 3 | funzioni iniettive / suriettive |
| 4 | tracciamento di memoria in C |
| 5 | matrici |
| 6 | sistemi di congruenze |

Alternare allena il cervello a **riconoscere il problema prima di applicare la formula**. Il punto è che all'esame non ti viene detto "questo è un esercizio di matrici": devi **deciderlo tu**.

> ⚠️ **Il rischio oposto.** L'interleaving rende all'inizio più lento: fai meno esercizi "facili" di fila. Dopo qualche settimana è più rapido **e** più robusto, perché non sai più a cosa stai rispondendo.



---

## Fase 3 — Simulazione delle prove a sbarramento

Molti esami del primo anno usano quiz con **sbarramento iniziale** e **tempi stretti**.

**Allenati sempre con il cronometro e senza formulari sottomano.** Una simulazione fatta con il libro aperto non è una simulazione.

| Corso | Sbarramento |
|---|---|
| [[Programma - Fondamenti dell'Informatica]] | Parte 1 obbligatoria per accedere alla parte 2 |
| [[Programma - Architettura degli Elaboratori]] | Prova di ammissione, 10 punti |
| [[Programma - Analisi Matematica]] | Quiz, serve 4/5 |
| [[Programma - Lingua Inglese I]] | Parte A (60 min) senza la quale non si fa la B |

### Categorizza ogni errore

Quando sbagli un quiz, **classifica** l'errore. La causa determina il rimedio:

| Tipo di errore | Cosa è successo | Cosa fare |
|---|---|---|
| **Calcolo o distrazione** | il metodo era giusto, ti sei sbagliato nei conti | rallenta e ricontrolla i **passaggi intermedi**, non solo il risultato |
| **C.E. o domini dimenticati** | hai trovato una soluzione estranea | aggiungi il trabocchetto alla scheda personale |
| **Lacuna teorica** | non sapevi la formula o il teorema | **torna subito** sul libro prima di fare un altro quiz |

> ⚠️ **La terza riga è quella che viene saltata.** È la più veloce da correggere e la più importante: un quiz fatto senza chiudere la lacuna dà lo stesso risultato sbagliato. Il momento migliore per ripassare è **subito dopo** aver sbagliato, non tre giorni dopo.
>
> 💡 **Regola operativa.** Dopo un errore di tipo 2 o 3, il quiz successivo è **un quiz diverso**. Ripetere lo stesso senza aver chiuso la lacuna è tempo perso.

---

## Fase 4 — Tecnica di Feynman

Prendi un argomento complesso e **spiegalo a voce alta** come se dovessi insegnarlo a una persona digiuna della materia.

| Argomento | Cosa devi spiegare |
|---|---|
| Gram-Schmidt | perché si sottrae la **proiezione** e non il vettore stesso |
| Insieme delle parti | perché $\lvert\mathcal{P}(X)\rvert = 2^n$, senza dire "ogni elemento ha due scelte" |
| Parametri per riferimento in C | perché la modifica è visibile al chiamante |
| Intersezione contro unione | perché i sistemi usano l'una e le disequazioni l'altra |

> 💡 **Il momento in cui balbetti è il momento della diagnosi.** Se ti blocchi, stai usando un termine **vago** invece del concetto preciso: è lì che c'è la lacuna. Torna su quella parola, non sull'intero argomento.
>
> ⚠️ **Non vale spiegare a chi ha già il contesto.** Se l'ascoltatore lo ha, ti permetti scorciatoie che nascondono proprio il punto che ti serve chiarire. Scegli qualcuno che non sa niente, oppure immagina di spiegare a un primo anno.

---

## Il ciclo completo

Le quattro fasi non sono isolate: si ripetono **a ciclo**.

| Momento | Fase | Durata tipica |
|---|---|---|
| Sessione di teoria | 1 — comprensione attiva | 40 min |
| Subito dopo | 2 — esercizi a intervalli | 60-90 min |
| Pre-esame | 3 — simulazione cronometrata | 2-3 simulazioni |
| Quando non capisci qualcosa | 4 — spiegazione a voce alta | 10 min |
| Dopo un errore | torna alla fase giusta | — |

> 💡 **Il ciclo più importante è fra la fase 3 e la fase 1.** Ogni errore di quiz classificato come "lacuna teorica" ti dice **esattamente** dove tornare. È ciò che trasforma gli errori in progresso invece che in frustrazione.

---

## La regola che vale più di tutte

> ⚠️ **Se un esercizio non sai risolverlo da solo, l'hai capito solo a metà.**

La lettura capisce. La risoluzione autonoma verifica. Il margine fra le due è ciò che ti salva all'esame — e con i quiz a sbarramento, quel margine decide se passi.

---

## Link

- [[Indice generale]] — la mappa di tutti i corsi
- [[Quadro riassuntivo dei 9 moduli]] — le formule chiave dei 9 moduli OFA
- [[Indice - Matematica Base]] — il percorso di recupero OFA
- [[Indice - Matematica Discreta, Algebra e Geometria]] — il corso da 12 CFU
- [[Indice - Fondamenti dell'Informatica]] — il corso con sbarramento