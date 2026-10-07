# Testovacie záznamy

## TC-Transfer-01 – Transfer funds

### Základné údaje

- **ID:** `TC-Transfer-01`
- **Názov:** Transfer funds
- **Prerekvizity:** Otvorená stránka ParaBank, prihlásený používateľ `john` / `demo`, dva existujúce účty
- **Testovacie dáta:**
  - účet odosielateľa: `12345`
  - účet príjemcu: `12456`
  - suma prevodu: `500`

### Kroky

1. Vybrať účet odosielateľa `12345`.
2. Vybrať účet príjemcu `12456`.
3. Zadať sumu `500`.
4. Kliknúť na tlačidlo **Transfer**.

### Výsledky

- **Očakávaný výsledok:** Zobrazí sa hláška **Transfer complete**.
- **Aktuálny výsledok:** Na doplnenie po vykonaní testu.
- **Status:** `PASS` / `FAIL` / `BLOCKED`

## Negatívne testy funkcie Transfer funds

| Test | Vstup | Očakávané správanie |
|---|---|---|
| Záporná suma | `-500` | Prevádzka je odmietnutá a zobrazí sa zrozumiteľná chybová hláška. |
| Nečíselný vstup | `abc!` | Prevádzka je odmietnutá a zobrazí sa validačná chyba. |
| Nedostatočný zostatok | Suma vyššia ako zostatok | Prevádzka je odmietnutá bez neoprávneného prevodu. |
| Rovnaký účet | Odosielateľ = príjemca | Prevádzka je odmietnutá. |
| Prázdna suma | Prázdne pole | Zobrazí sa správna chybová hláška pre povinné pole. |

