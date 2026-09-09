# Johanne og Sondre — bryllaupsside

Bryllaupsnettsida til Johanne og Sondre, hosta på GitHub Pages med eige
domene ([www.johanneogsondre.no](https://www.johanneogsondre.no)). Sida er
éi fil: `index.html`. Bryllaupsdatoen er **29. mai 2027**.

## Filer

- `index.html` — heile sida (struktur, styling og skript i éi fil, inkludert
  bileta som base64).
- `CNAME` — **må aldri slettast eller endrast**. Krevst for det eigne
  domenet på GitHub Pages.
- `README.md`
- `spill.html` — eige "snurr hjulet"-spel. Ikkje lenkja frå `index.html`
  lenger etter redesignet (sjå under), men fila ligg framleis i repoet.

## Reglar for endringar

- Innhaldet på sida skal vere på **bokmål**.
- Behald design, fargar og tone som dei er — ikkje gjer om på layout,
  fargepalett (`--paper`, `--card`, `--ink`, `--muted`, `--accent`,
  `--line`, `--shadow`) eller skrifttypar utan at det er eksplisitt bedt
  om.
- Ikkje rør `CNAME`.
- Gjer berre dei endringane som er eksplisitt bedt om — ikkje "forbetre"
  eller endre anna innhald på eiga hand.
- Passordgata (`#password-gate`, `var PASSORD` nedst i skriptet) er berre
  klientside-fnising, ikkje reell sikkerheit — den held nysgjerrige ute,
  ikkje motiverte personar.
- Sida er hosta på **GitHub Pages**, ikkje Netlify. Skjema (`<form>`) kan
  difor **ikkje** bruke `data-netlify="true"` eller elles stole på at
  GitHub Pages tek imot innsendingar — det finst ingen backend. Sjå eige
  avsnitt under om dei to skjemaa på sida.

## Skjema (toastmaster-kontakt og RSVP)

Sida har to `<form>`-element: `#toastmaster-form` (kontakt toastmaster) og
`#svar-form` (RSVP, med moglegheit for å leggje til fleire personar).
Ingen av dei er kopla til noka reell innsendingsløysing enno — eit script
(`disableFormSubmit(...)` nær botnen av fila) fangar opp `submit`,
hindrar sidelasting/datatap, og viser i staden ei tydeleg tekstmelding om
at funksjonen ikkje er aktivert enno, med telefonnummera til Johanne og
Sondre som alternativ.

Brudeparet ordnar sjølv eit ekte skjema-baksystem (t.d. Google Form,
Formspree e.l.) og gir beskjed når det er klart. **Når** ei ekte
skjema-løysing/lenkje ligg føre:

- Kople dei to skjemaa til den løysinga (t.d. `action`-attributt til eit
  Formspree-endepunkt, eller erstatt skjemaet med ei lenkje til eit
  Google Form) i staden for `disableFormSubmit`.
- **Vér obs på lenkjer med redigeringstilgang** (t.d. ei Google
  Sheets-lenkje av typen `.../edit?usp=drivesdk`) — slike lenkjer gir alle
  som klikkar på dei redigeringstilgang til heile arket, ikkje berre eit
  skjema for å melde seg på. Slike lenkjer skal **aldri** publiserast
  direkte på ei offentleg side. Spør brudeparet om ei visningslenkje eller
  eit ekte skjema/endepunkt i staden dersom du berre får ei edit-lenkje.

## Kontaktinfo / sensitive verdiar i sida

Desse felta inneheld verdiar som må haldast oppdaterte og kan endre seg:

- **Telefonnummer til Johanne og Sondre** — i footeren (`tel:`-lenkjer),
  brukt som kontakt generelt og som midlertidig RSVP-alternativ medan
  skjemaa ikkje er aktiverte.
- **Toastmaster-kontaktskjema** — `#toastmaster-form`, sjå eige avsnitt
  over.
- **RSVP-skjema** — `#svar-form`, sjå eige avsnitt over. RSVP-frist er
  **1. februar**.
- **Passord** — `var PASSORD` nedst i `<script>`.
- **Vielsestad/-tid** — Vålerenga kirke, kl. 14.30.
- **Festlokale** — Kruttverket.

Desse verdiane skal **aldri** fyllast ut med oppdikta/gjetta verdiar —
berre med det brudeparet faktisk oppgir, sidan sida er live og brukt av
ekte gjester til RSVP og kontakt.

Merk: denne versjonen av sida har **ingen** eiga "ønskeliste"/Vipps-seksjon
(gåve-seksjonen seier berre at brudeparet ikkje ønskjer gåver, men tek
gjerne imot bidrag til bryllupsreisa). Dersom eit Vipps-nummer skal leggjast
til seinare, må plassering avklarast eksplisitt før det gjerast.

Bryllaupsdato er **29. mai 2027**, og passordet er sett til **`29mai`**
(matchar datoen).
