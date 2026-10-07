# Poznámky k systému

## Testovaná aplikácia

- Aplikácia: ParaBank
- URL: `https://parabank.parasoft.com/parabank/`
- Testovací používateľ: `john`
- Heslo: `demo`

## Testovaný rozsah

Po prihlásení sa overujú tieto funkcie:

- domovská stránka a pravý horný panel,
- vytvorenie bežného a sporiaceho účtu,
- prehľad účtov,
- posielanie peňazí,
- platenie účtov,
- vyhľadanie transakcie,
- úprava osobných údajov,
- žiadosť o pôžičku,
- odhlásenie.

Osobitná pozornosť je venovaná funkcii **Transfer funds** a validácii vstupov:

- záporná suma,
- nečíselné znaky (`abc!`),
- suma vyššia ako zostatok na účte,
- odoslanie na rovnaký účet,
- prázdna suma.

