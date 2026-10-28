# Ekvivalenčné triedy a analýza hraničných hodnôt

## Testovaný vstup

- Funkcia: **Transfer funds**
- Pole: **Amount** (suma prevodu)
- Predpoklad: zostatok na účte odosielateľa je `Z` (napr. `Z = 1000`)

## Ekvivalenčné triedy

| ID | Trieda | Príklad vstupu | Typ | Očakávané správanie |
|---|---|---|---|---|
| EC1 | Kladná suma v rozsahu `0 < suma ≤ Z` | `500` | platná | Prevod sa vykoná, zobrazí sa **Transfer complete**. |
| EC2 | Záporná suma | `-500` | neplatná | Prevod je odmietnutý, zobrazí sa chybová hláška. |
| EC3 | Nulová suma | `0` | neplatná | Prevod je odmietnutý. |
| EC4 | Suma vyššia ako zostatok `suma > Z` | `1500` | neplatná | Prevod je odmietnutý bez zmeny zostatkov. |
| EC5 | Nečíselný vstup | `abc!` | neplatná | Zobrazí sa validačná chyba. |
| EC6 | Prázdne pole | *(prázdne)* | neplatná | Zobrazí sa chyba pre povinné pole. |

## Hraničné hodnoty

| ID | Hodnota | Hranica | Očakávané správanie |
|---|---|---|---|
| BVA1 | `-0.01` | tesne pod nulou | odmietnuté |
| BVA2 | `0` | dolná hranica | odmietnuté |
| BVA3 | `0.01` | tesne nad nulou | prevod sa vykoná |
| BVA4 | `Z - 0.01` | tesne pod zostatkom | prevod sa vykoná |
| BVA5 | `Z` | horná hranica | prevod sa vykoná |
| BVA6 | `Z + 0.01` | tesne nad zostatkom | odmietnuté |

## Poznámky

- Hodnotu `Z` treba pred testom zistiť v **Accounts Overview**.
- Pri každom neplatnom vstupe overiť aj to, že sa zostatky na účtoch nezmenili.
