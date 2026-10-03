# Appunti — Primo anno Informatica (UniTO)

Libreria di appunti del **primo anno** del corso di laurea in Informatica dell'Università di Torino, in formato Markdown e organizzata per [Obsidian](https://obsidian.md).

> [!warning] Materiale personale
> Questi appunti **non** sono materiale ufficiale dell'Università. Sono le mie note di studio, ricavate dai programmi dei corsi, dal materiale del Corso di Riallineamento (OFA) e dalle mie elaborazioni. Per le fonti autogradite fare sempre riferimento al materiale pubblicato dall'ateneo.

---

## Struttura

```
appunti/
├── .obsidian/        configurazione del vault
└── 1_anno/           primo anno di laurea
    ├── Indice generale.md          mappa di tutti i corsi
    ├── Piano di Studio.md         il piano studi completo
    ├── Metodo di Studio.md        come studiare, in 4 fasi
    ├── Risorse degli studenti.md  materiale utile trovato online
    ├── OFA/                       Corso di Riallineamento di Matematica
    └── [una cartella per ogni corso]
```

Le cartelle sono divise per **anno di corso**: `1_anno/`, e in futuro `2_anno/` e così via.

---

## I corsi del primo anno

| Corso | Codice | CFU | Note |
|---|---|---|---|
| **Matematica Discreta, Algebra e Geometria** | INF0328 | 9 | 4 |
| **Programmazione I** | MFN0582 | 9 | 2 |
| **Fondamenti dell'Informatica** | INF0348 | 9 | 5 |
| **Lingua Inglese I** | L-LIN/12 | 3 | 20 |
| **Analisi Matematica** | MFN0570 | 9 | 3 |
| **Architettura degli Elaboratori** | INF0326 | 9 | 2 |
| **Programmazione II** | INF0330 | 9 | 2 |
| **Ricerca Operativa** | INF0327 | 9 | 2 |
| **OFA** — Corso di Riallineamento | — | nessuno | 26 |

Ogni corso ha almeno due note fisse:

- **`Programma - <Corso>.md`** — il programma ufficiale, con codice, CFU e argomenti
- **`Indice - <Corso>.md`** — la mappa delle lezioni, con lo stato di ciascuna

> 💡 **Perché gli indici hanno nomi unici.** Ogni corso ha un file `Indice - <Nome>.md` invece del solito `00 - Indice.md`: con molti corsi, file omonimi renderebbero ambigui i link `[[...]]` di Obsidian.

---

## Lo stato di avanzamento

Le note usano due simboli:

| Simbolo | Significato |
|---|---|
| ✅ | **scritta** |
| 📄 | **da scrivere** (placeholder con il link alla nota futura) |

**Corso di Riallineamento (OFA)** — 9 moduli, **12 lezioni scritte** su 20, più le note di riepilogo:

| Modulo | Stato |
|---|---|
| 1. Linguaggio, numeri e simbologia | ✅ completo |
| 2. Fattorizzazione di polinomi | ✅ completo |
| 3. Equazioni e disequazioni di 1° e 2° grado | ✅ completo |
| 4. Equazioni fratte, irrazionali, con valore assoluto | ✅ completo |
| 5. Geometria analitica | ✅ completo |
| 6. Funzioni reali di variabile reale | 🔶 in corso (6.1 scritta) |
| 7. Esponenziali e logaritmi | 📄 |
| 8. Trigonometria | 📄 |
| 9. Statistica e probabilità | 📄 |

> 📌 **Il Modulo 9 non è urgente:** probabilità e statistic non fanno parte di nessuno degli esami del primo anno.

Gli altri corsi hanno il programma e l'indice, e le prime lezioni iniziate.

---

## Note trasversali

| Nota | A cosa serve |
|---|---|
| [[Metodo di Studio]] | il metodo in 4 fasi: apprendimento, esercizi, simulazioni, verifica |
| [[Risorse degli studenti]] | dove trovare appunti, esercizi e prove d'esame degli anni passati |
| [[Prerequisiti del Primo Anno]] | confronto fra la mia lista di prerequisiti e i corsi che li richiedono |
| [[Quadro riassuntivo dei 9 moduli]] | tutte le formule chiave dell'OFA, con i trabocchetti |
| [[Piano di Studio]] | il piano studi completo del corso di laurea |

---

## Come usare il vault in Obsidian

1. Installa [Obsidian](https://obsidian.md) (gratuito)
2. **Apri la cartella come vault**: *Open folder as vault* e scegli questa cartella
3. Parti da **`Indice generale.md`**, che rimanda a tutto il resto

Le note usano i wikilink `[[...]]`, le callout `> [!info]` e le tabelle, quindi si leggono bene anche fuori da Obsidian (per esempio con Typora, Obsidian mobile o un editor qualsiasi).

> ⚙️ **Se usi Obsidian Sync**: tieni presente che versiona gli stessi file di Git. I due sistemi possono entrare in conflitto. Per questo nel `.gitignore` è escluso `workspace.json`, che cambia a ogni sessione e produrrebbe conflitti inutili.

---

## Convenzioni

| Simbolo | Vuol dire |
|---|---|
| ✅ | contenuto scritto e verificato |
| 📄 | ancora da scrivere |
| 📁 | percorso o cartella |
| ⚠️ | errore o trabocchetto da evitare |
| 💡 | spiegazione o intuizione utile |
| ❓ | informazione non verificata |

I nomi dei file seguono `Programma - <Corso>.md`, `Indice - <Corso>.md` e `<Modulo>.<Lezione> - <Titolo>.md`.

---

## Licenza

Le note sono mie e sono rilasciate per uso personale e didattico. Chi le riutilizza deve fare riferimento alle fonti originali — in particolare ai programmi dei corsi e al materiale OFA dell'Università di Torino.