# Indice - Architettura Avanzata degli Elaboratori

> [!info] Mappa del corso
> **Legenda:** ✅ scritto · 📄 da scrivere
> **Docente:** Enrico Bini

> [!warning] Fonte non ufficiale
> Questo indice è basato sul documento del **Team Studentesco** e sul portale del corso, **non** sul documento ufficiale del corso di laurea che riporta i programmi. Codice, crediti e docenti vanno **verificati** su Campusnet o sul Moodle del corso.

| | |
|---|---|
| **Crediti** | 6 CFU · 48 ore in aula |
| **Semestre** | 2° |

---

## Programma

> ⚠️ Questo è uno dei pochi corsi di cui il **documento RSS ufficiale** fornisce il programma per esteso.

| Argomento | Note |
|---|---|
| Architettura a processore singolo: pre-fetch, branch prediction, pipeline | 📄 [[Pipeline e Branch Prediction]] |
| Esecuzione out-of-order e stallo | 📄 [[Out-of-Order e Stallo]] |
| Architettura multiprocessore: acceleratori, contesa sul bus | 📄 [[Multiprocessore e Bus Contention]] |
| Gerarchia di memoria: cache, località | 📄 [[Cache e Localita]] |
| Politiche avanzate di scheduling, locking, pinning | 📄 [[Scheduling Avanzato]] |
| Linux: scheduling classes, trace-cmd | 📄 [[Linux Scheduling e trace-cmd]] |
| Performance counters | 📄 [[Performance Counters]] |
| Linux: filesystem procfs | 📄 [[procfs]] |

---

## Esame

- **Prova scritta** (obbligatoria)
- **Prova orale**: **obbligatoria** per chi ha ≥ 25/30 allo scritto, **facoltativa** per gli altri
- Solo con lo scritto (≤ 24): voto finale = voto dello scritto
- Con l'orale: il voto finale è determinato dall'orale

---

## Prerequisiti

- **Architettura degli Elaboratori** (1° anno) — **diretto**: questo è il livello successivo
- **Sistemi Operativi** (2° anno) — lo scheduling è il ponte fra i due corsi
- **Ricerca Operativa** — alcuni concetti di ottimizzazione

> 💡 **Il filo che lega i due corsi di architettura.** Al primo anno hai visto come funziona una CPU. Qui vedi **perché** funziona male: la pipeline va riempita, il branch prediction sbaglia, la cache manca. E come si rimedia agendo dall'interfaccia del sistema operativo: è il motivo per cui tutto il programma è su Linux.

## Collegamento

- [[Programma - Architettura degli Elaboratori]] — il prerequisito diretto
- [[Indice - Sistemi Operativi]] — lo scheduling è il ponte

## Link

- [[Indice generale - Terzo Anno]]
