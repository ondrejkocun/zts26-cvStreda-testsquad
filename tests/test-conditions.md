# Testovacie podmienky

## Predpoklady

1. Aplikácia ParaBank je dostupná.
2. Používateľ sa prihlási údajmi `john` / `demo`.
3. Používateľ má k dispozícii aspoň dva existujúce účty.
4. Sú známe čísla účtov odosielateľa a príjemcu.

## Testovacie scenáre

### Prihlásenie a navigácia

- Prihlásenie používateľa `john` heslom `demo`.
- Zobrazenie domovskej stránky.
- Kontrola pravého horného panela.
- Kontrola dostupnosti hlavných funkcií.
- Odhlásenie používateľa.

### Správa účtov a používateľského profilu

- Vytvorenie bežného účtu.
- Vytvorenie sporiaceho účtu.
- Zobrazenie prehľadu účtov.
- Úprava osobných údajov.
- Požiadanie o pôžičku.

### Platby a transakcie

- Poslanie peňazí medzi účtami.
- Zaplatenie účtu.
- Vyhľadanie transakcie.
- Kontrola chybovej hlášky pri zadanej prázdnej sume.

### Negatívne prípady pri prevode

- Odoslanie zápornej sumy.
- Zadanie nečíselných znakov.
- Odoslanie sumy vyššej ako zostatok.
- Odoslanie na rovnaký účet.

