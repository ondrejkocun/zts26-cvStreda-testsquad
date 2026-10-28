# Rozhodovacia tabuľka – prihlásenie

## Podmienky a akcie

| | R1 | R2 | R3 | R4 | R5 |
|---|---|---|---|---|---|
| **C1** Username vyplnený | N | A | A | A | A |
| **C2** Heslo vyplnené | - | N | A | A | A |
| **C3** Username existuje | - | - | N | A | A |
| **C4** Heslo správne | - | - | - | N | A |
| **Výsledok** | Chyba: zadajte meno a heslo | Chyba: zadajte heslo | Chyba: zákazník neexistuje | Chyba: nesprávne heslo | Prihlásenie |

Legenda: `A` – áno, `N` – nie, `-` – na hodnote nezáleží.

## Pokrytie pravidiel testami

| Pravidlo | Testovací prípad |
|---|---|
| R1 | na doplnenie |
| R2 | na doplnenie |
| R3 | na doplnenie |
| R4 | [TC-031](test-records/TC-031.md) |
| R5 | na doplnenie |
