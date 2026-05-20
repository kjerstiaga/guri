# Guris medisinapp

Enkel helse- og treningsapp for en person med Parkinsons sykdom. Designet for å brukes direkte på mobil — stor skrift, få valg, ingen installasjon.

🔗 **[Åpne appen](https://[brukernavn].github.io/[repo-navn])**

---

## Hva appen gjør

### 💊 Medisin-siden
- Viser neste Sinemet-dose med nedtelling
- Fire store knapper å trykke på:
  - **Jeg tok medisinen** — med valg om hvordan hun har det etterpå
  - **Jeg er stiv / skjelver** — registrerer symptomer
  - **Jeg har smerter** — sted og type
  - **Jeg har det bra** — med plass til en kommentar
- Logg over hva som er registrert i dag

### 🏃 Trening-siden
- Én enkel øvelse per dag
- Stor grønn knapp: "Jeg gjorde det!"
- Knapp for å bytte til en annen øvelse
- 7-dagers streak for motivasjon
- Forklaring på hvorfor øvelsen er bra

**Øvelsene:** Reise seg fra stol, tråkke på stedet, knytte neven, puste dypt, snu hodet, strekke armene, gå ti skritt, klappe hendene.

---

## Medisintider

```
07:00 — 11:00 — 16:00 — 20:00
```

For å endre tidene: åpne `index.html` i et tekstredigeringsprogram og finn denne linjen:

```js
const SINEMET = ['07:00','11:00','16:00','20:00'];
```

---

## Teknisk

- Én HTML-fil — ingen rammeverk, ingen avhengigheter
- Fungerer uten internett etter første lasting (font lastes fra Google Fonts)
- Data lagres i nettleserens `localStorage` — forlater aldri enheten
- Font: [Atkinson Hyperlegible](https://brailleinstitute.org/freefont) — designet for lesbarhet

---

## Viktig om data

Data lagres kun i nettleseren på den enheten appen brukes på. Sletting av nettleserdata fjerner all historikk. For å dele observasjoner med pårørende eller lege — si det videre muntlig eller noter det ned.

---

## Tilhørende pårørendeverktøy

Dette er Guris egen enkle versjon. Det finnes også en utvidet versjon (`guri-tracker-v3.html`) for pårørende med wearing off-analyse, søvnlogg, fallregistrering og rapport til lege.

---

*Laget med Claude (Anthropic) · Mai 2026*
