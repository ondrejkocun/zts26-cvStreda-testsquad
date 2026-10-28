# Vybrané testy

Rozpočet: **12 bodov**

## Vybrané testovacie prípady

| ID | Testovacia podmienka / scenár | Cena | Riziko |
|---|---|---|---|
| TC07 | Prevod – platný prevod medzi účtami | 2 | ⭐ 1 Prevod peňazí |
| TC08 | Prevod – neplatný alebo hraničný vstup | 2 | ⭐ 1 Prevod peňazí |
| TC01 | Prihlásenie – platné údaje | 1 | ⭐ 2 Prihlásenie |
| TC02 | Prihlásenie – nesprávne heslo | 1 | ⭐ 2 Prihlásenie |
| TC09 | Platba faktúry – základný scenár | 2 | ⭐ 3 Platba faktúry |
| TC06 | Otvorenie nového účtu – základný scenár | 2 | príprava druhého účtu pre prevod |
| | **Spolu** | **10 / 12** | |

## Pokryté TOP 3 riziká

1. **Prevod peňazí** – TC07, TC08
2. **Prihlásenie** – TC01, TC02
3. **Platba faktúry** – TC09

## Vedome nepokryté riziko

**Žiadosť o pôžičku (TC12)** – stredné riziko, ale najdrahší test (3 body). Za tú cenu získame viac informácie z TOP 3.

## Prečo je tento výber lepší než náhodný

Takmer celý rozpočet ide do oblastí s najvyšším rizikom, takže pri vydaní vieme, že funkcie, kde chyba znamená stratu peňazí alebo prístup k účtu, sú otestované.

## Testovacie sady

| Sada | Názov | TC | Účel |
|---|---|---|---|
| 01 ⚡ rýchla | Dymová sada (smoke) | TC01, TC06 | Dá sa prihlásiť a otvoriť účet? Ak nie, zostavenie nie je vhodné na ďalšie testovanie. |
| 02 | Pohyb peňazí | TC07, TC08, TC09 | Odchádzajú peniaze správne a neplatné prevody sú odmietnuté? |
| 03 | Ochrana prístupu | TC02 | Dostane sa k účtu niekto bez správneho hesla? |
