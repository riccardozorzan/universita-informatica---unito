# Appunti — Primo anno Informatica (UniTO)

Libreria di appunti del **primo anno** del corso di laurea in Informatica dell'Università di Torino, in formato Markdown e organizzata per [Obsidian](https://obsidian.md).

> [!warning] Materiale personale
> Questi appunti **non** sono materiale ufficiale dell'Università. Sono le mie note di studio, ricavate dai programmi dei corsi, dal materiale del Corso di Riallineamento (OFA) e dalle mie elaborazioni. Per le fonti autogradite fare sempre riferimento al materiale pubblicato dall'ateneo.

---

## Struttura

```
appunti/
├── .obsidian/        configurazione del vault
├── 1_anno/           primo anno di laurea
├── 2_anno/           secondo anno
└── 3_anno/           terzo anno
```

Le cartelle sono divise per **anno di corso**. Ogni anno ha un `Indice generale` che mappa tutti i suoi corsi; ogni corso ha almeno un `Indice - <Corso>.md` con codice, crediti, ore, semestre e docenti.

Alcuni corsi hanno anche una cartella `pdf/` con il materiale delle biblioteche. Questi file **restano nel vault** e sono apribili da Obsidian, ma sono esclusi da Git: sono quasi un gigabyte di opere protette da copyright, e Git non li comprimerebbe ulteriormente.

Nel primo anno ci sono anche le note trasversali:

| Nota | A cosa serve |
|---|---|
| `Piano di Studio.md` | il piano studi completo del corso di laurea |
| `Metodo di Studio.md` | come studiare, in 4 fasi |
| `Risorse degli studenti.md` | materiale utile trovato online |
| `OFA/` | Corso di Riallineamento di Matematica |

---

## Gli anni della laurea

| Anno | Indice | Corsi con indice |
|---|---|---|
| **1° anno** | [[Indice generale]] | 8 insegnamenti + OFA, con le lezioni scritte |
| **2° anno** | [[Indice generale - Secondo Anno]] | 9 insegnamenti |
| **3° anno** | [[Indice generale - Terzo Anno]] | 20 insegnamenti (elenco da verificare) |

> ⚠️ Gli indici del 2° e 3° anno sono basati sul **documento ufficiale del corso di laurea** per codici, CFU, ore e docenti. Il programma dettagliato è disponibile solo per alcuni corsi; per gli altri l'indice rimanda al Moodle del rispettivo corso. **Gli indici del 3° anno sono da verificare**: l'elenco ufficiale ne conferma soltanto 4.

## I corsi del primo anno

| Corso | Codice | CFU | Sem. | Note |
|---|---|---|---|---|
| **Matematica Discreta, Algebra e Geometria** | INF0328 | 12 | 1° | I |
| **Programmazione I** | MFN0582 | 9 | 1° | I |
| **Fondamenti dell'Informatica** | INF0348 | 9 | 1° | I |
| **Analisi Matematica** | MFN0570 | 9 | 2° | II |
| **Architettura degli Elaboratori** | INF0326 | 6 | 2° | II |
| **Programmazione II** | INF0330 | 6 | 2° | II |
| **Ricerca Operativa** | INF0327 | 6 | 2° | II |
| **Lingua Inglese I** | MFN0590 | 3 | 2° | II |
| **OFA** — Corso di Riallineamento | — | nessuno | — | 9 moduli |

Totale: **60 CFU**, il carico del primo anno. I dati sono tratti dalle schede ufficiali del corso per l'anno accademico 2026/2027.

---

## Lo stato di avanzamento

Le note usano due simboli:

| Simbolo | Significato |
|---|---|
| ✅ | **scritta** |
| 📄 | **da scrivere** (placeholder con il link alla nota futura) |

**Corso di Riallineamento (OFA) — completo.** Tutti e 9 i moduli sono scritti, per un totale di **19 lezioni**, ciascuna con teoria, esercizi e test di autovalutazione con le risposte.

| Modulo | Lezioni | Stato |
|---|---|---|
| 1. Linguaggio, numeri e simbologia | 1.1 · 1.2 | ✅ completo |
| 2. Fattorizzazione di polinomi | 2.1 | ✅ completo |
| 3. Equazioni e disequazioni di 1° e 2° grado | 3.1 · 3.2 · 3.3 | ✅ completo |
| 4. Equazioni fratte, irrazionali, con valore assoluto | 4.1 · 4.2 · 4.3 | ✅ completo |
| 5. Geometria analitica | 5.1 · 5.2 | ✅ completo |
| 6. Funzioni reali di variabile reale | 6.1 · 6.2 | ✅ completo |
| 7. Esponenziali e logaritmi | 7.1 · 7.2 | ✅ completo |
| 8. Trigonometria | 8.1 · 8.2 | ✅ completo |
| 9. Statistica e probabilità | 9.1 · 9.2 | ✅ completo |

> 📌 **Il Modulo 9 non è urgente:** probabilità e statistica non fanno parte di nessuno degli esami del primo anno. Chi ha fretta può rimandarlo.

> ⚠️ **Alcune soluzioni del materiale OFA sono imprecise**, e le note le correggono con la verifica in calcolo simbolico. I casi documentati: esercizi 6 e 7 del Modulo 7.2, ed esercizi 6, 7 e 10 del Modulo 8.2.

**Altri corsi del primo anno.** Hanno il programma e l'indice; le note di studio sono iniziate solo dove servono di più:

| Corso | Note di studio |
|---|---|
| **Analisi Matematica** | ✅ funzioni elementari |
| **Lingua Inglese I** | ✅ linkers, condizioni, *used to* |
| gli altri 6 corsi | 📄 |

---

## Da dove cominciare

| Vuoi preparare | Parti da |
|---|---|
| un esame di matematica | [[Prerequisiti del Primo Anno]] — dice **quali moduli OFA** servono e in che ordine |
| il test di fine modulo | [[Quadro riassuntivo dei 9 moduli]] — tutte le formule chiave in una pagina, con i trabocchetti |
| la prima lezione di un corso | `Indice - <Corso>.md`, che rimanda a tutto il resto |
| come studiare in generale | [[Metodo di Studio]] |

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

> ⚙️ **Se usi Obsidian Sync**: tieni presente che versiona gli stessi file di Git. I due sistemi possono entrare in conflitto. Per questo nel `.gitignore` sono esclusi i file che cambiano a ogni sessione (`workspace.json` e simili) e i PDF delle biblioteche.

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