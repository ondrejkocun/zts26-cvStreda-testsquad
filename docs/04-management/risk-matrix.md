# Analýza rizík – ParaBank

D = dopad, P = pravdepodobnosť (nízky / stredný / vysoký)

| Oblasť | D | P | Úroveň | TOP 3 |
|---|---|---|---|---|
| Registrácia | stredný | stredná | 🟡 stredné | |
| Prihlásenie | vysoký | stredná | 🟠 vysoké | ⭐ 2 |
| Prehľad účtov | stredný | nízka | 🟢 nízke | |
| Otvorenie účtu | stredný | stredná | 🟡 stredné | |
| Prevod peňazí | vysoký | vysoká | 🔴 kritické | ⭐ 1 |
| Platba faktúry | vysoký | stredná | 🟠 vysoké | ⭐ 3 |
| Žiadosť o pôžičku | stredný | stredná | 🟡 stredné | |
| Kontaktné údaje | nízky | stredná | 🟢 nízke | |

## Prečo TOP 3

1. **Prevod peňazí** – veľa neplatných vstupov (záporná suma, `abc!`, suma nad zostatok, rovnaký účet) a chyba znamená priamu stratu peňazí.
2. **Prihlásenie** – je bránou ku všetkým funkciám, chyba znamená únik údajov alebo že sa používateľ nedostane k účtu.
3. **Platba faktúry** – formulár má veľa polí a peniaze odídu tretej strane, odkiaľ sa ťažko vracajú.
