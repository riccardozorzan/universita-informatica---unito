# Sistemi di Numerazione

L'informatica lavora solo con **numeri in base 2**, perché le componenti elettroniche hanno solo due stati. Noi scriviamo in base 10 per comodità: il computer converte.

---

## I sistemi posizionali

In base *b*, ogni cifra ha un valore pari a *cifra × b^posizione* (posizione contata da destra, da 0).

$$(123)_{10} = 1\cdot10^2 + 2\cdot10^1 + 3\cdot10^0$$

---

## I quattro sistemi usati

| Base | Nome | Cifre | Esempio | Dove si usa |
|---|---|---|---|---|
| **2** | binario | 0 1 | 1011 | Internamente: il linguaggio della macchina |
| **8** | ottale | 0-7 | 13 | Nei vecchi sistemi, raggruppando 3 bit |
| **10** | decimale | 0-9 | 11 | Come parliamo noi |
| **16** | esadecimale | 0-9 A-F | B | Indirizzi di memoria, colori, dump di dati |

> 💡 **Regola chiave:** le basi **8** e **16** sono potenze di 2 ($8 = 2^3$, $16 = 2^4$), quindi la conversione col binario è puramente un raggruppamento di cifre.

---

## Binario → decimale

Leggi le cifre da destra e moltiplica per potenze crescenti di 2.

> $(1011)_2 = 1\cdot2^3 + 0\cdot2^2 + 1\cdot2^1 + 1\cdot2^0 = 8+0+2+1 = (11)_{10}$

### Tabella delle potenze di 2

| $2^n$ | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|---|---|---|---|---|---|---|---|---|
| **valore** | 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |

---

## Decimale → binario

Due modi:

**1. Divisioni successive** — dividi per 2 e leggi i resti dal basso:

> 11 → 11/2 = 5 resto **1** → 5/2 = 2 resto **1** → 2/2 = 1 resto **0** → 1/2 = 0 resto **1**
> Leggendo dal basso: **1011**

**2. Sottrarre potenze** — trova la più grande potenza di 2 ≤ il numero e procedi:

> 11 = 8 + 2 + 1 → **1011**

---

## Binario ↔ esadecimale

Ogni cifra esadecimale corrisponde a **4 bit**. Basta raggruppare di 4 in 4, da destra.

> $(11010110)_2$ → `1101 0110` → **D6** → $(D6)_{16}$

| Hex | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | A | B | C | D | E | F |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Bin** | 0000 | 0001 | 0010 | 0011 | 0100 | 0101 | 0110 | 0111 | 1000 | 1001 | 1010 | 1011 | 1100 | 1101 | 1110 | 1111 |

---

## Byte e intervalli

Il **byte** è l'unità di indirizzamento della memoria: **8 bit**.

> $(255)_{10} = (11111111)_2 = (FF)_{16}$

| Tipo | Bit | Byte | Intervallo decimale |
|---|---|---|---|
| unsigned char | 8 | 1 | 0 → 255 |
| char (con segno) | 8 | 1 | -128 → 127 |
| unsigned short | 16 | 2 | 0 → 65.535 |
| short (con segno) | 16 | 2 | -32.768 → 32.767 |
| unsigned int | 32 | 4 | 0 → 4.294.967.295 |
| int (con segno) | 32 | 4 | -2.147.483.648 → 2.147.483.647 |
| long long | 64 | 8 | -9.2 × 10¹⁸ → 9.2 × 10¹⁸ |

> ⚠️ **Attenzione — il segno:** nel **complemento a due** (lo standard) il bit più significativo è il segno. Il numero più negativo non ha un positivo corrispondente:
>
> - int a 32 bit: da **-2.147.483.648** a **2.147.483.647**
> - unsigned int a 32 bit: da **0** a **4.294.967.295**
> - `-1` in unsigned è **4.294.967.295**, non errore: è semplicemente il bit-pattern riinterpretato

---

## Operazioni in base 2

### Addizione

Come la somma decimale, ma le cifre sono solo 0 e 1.

```
   1 0 1 1   (11)
+  0 1 1 0   (6)
───────────
  1 0 0 1   (17)
```

Il riporto si genera solo quando `1 + 1 = 10` (1 con riporto di 1).

### Sottrazione

Uguale all'addizione, ma con **riporto preso in prestito**:

```
  1 0 1 0   (10)
-   0 1 1   (3)
──────────
  0 1 1 1   (7)
```

---

## Esempi contesto informatico

- **Indirizzo di memoria** `0x7FFE3A20` → in esadecimale, così è compatto e leggibile nei dump di memoria.
- **Codice colore HTML** `#FF5733` → `#FF` = rosso massimo, `57` = verde medio, `33` = blu debole.
- **Numerazione di riga** in un editor di testo → mostrata in esadecimale perché gli indirizzi fisici sono in quel formato.
- **Un file da 1 MB** (1.048.576 byte) scritto in base 2 occupa 8.388.608 bit, cioè 20 cifre binarie contro 7 decimali.

---

## Riepilogo

- La macchina ragiona **solo in base 2** (bit)
- Noi scriviamo in **base 10**, il programmatore spesso in **base 16**
- 1 byte = 8 bit → intervallo unsigned: 0-255
- Base 8 e 16 sono potenze di 2 → conversione col binario per raggruppamento (3 bit / 4 bit)

---

## Link

- [[Programma - Fondamenti dell'Informatica]] — il programma di questo corso
- [[Codifica dei Caratteri]] — come i caratteri diventano numeri
- [[Rappresentazione degli Interi]] — complemento a 1 e a 2
- [[Numeri Reali e IEEE 754]] — la virgola mobile
- [[Programma - Architettura degli Elaboratori]] — la rappresentazione fisica di tutto questo
