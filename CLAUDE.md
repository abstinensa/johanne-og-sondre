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
- `spill.html` — eige "snurr hjulet"-spel ("Hvilken bryllupsgjest er du?"),
  lenkja frå ein eigen kort-seksjon (`#spill`) i `index.html`. Fila har sin
  eigen, uendra passordgate i den gamle festival-stilen (sjå eigen kode
  der) — han er ikkje visuelt oppdatert til den nye fargepaletten.

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

RSVP (`#svar`) er eit innebygd Google-skjema, «Bryllupsinvitasjon -
Svarskjema». Det er den einaste svarvegen. Bruk den offentlege
visningsadressa (`/viewform`), og `?embedded=true` i iframe. Ikkje bruk
redigerings- eller publish-editor-parametrar.

`#toastmaster-form` (kontakt toastmaster) er ikkje kopla til noka reell
innsendingsløysing enno — eit script (`disableFormSubmit(...)` nær botnen
av fila) fangar opp `submit`, hindrar sidelasting/datatap, og viser i
staden ei tydeleg tekstmelding om at funksjonen ikkje er aktivert enno,
med telefonnummera til Johanne og Sondre som alternativ.

**Når** ei ekte løysing for toastmaster ligg føre:

- Kople toastmaster-skjemaet til den løysinga (t.d. `action`-attributt til
  eit Formspree-endepunkt, eller erstatt skjemaet med ei lenkje) i staden
  for `disableFormSubmit`. Ikkje byt ut RSVP-en med noko anna enn det
  Google-skjemaet brudeparet har oppgitt.
- **Vér obs på lenkjer med redigeringstilgang** (t.d. ei Google
  Sheets-lenkje av typen `.../edit?usp=drivesdk`) — slike lenkjer gir alle
  som klikkar på dei redigeringstilgang til heile arket, ikkje berre eit
  skjema for å melde seg på. Slike lenkjer skal **aldri** publiserast
  direkte på ei offentleg side. Spør brudeparet om ei visningslenkje eller
  eit ekte skjema/endepunkt i staden dersom du berre får ei edit-lenkje.

## Kontaktinfo / sensitive verdiar i sida

Desse felta inneheld verdiar som må haldast oppdaterte og kan endre seg:

- **Telefonnummer til Johanne og Sondre** — i footeren (`tel:`-lenkjer),
  brukt som kontakt generelt og som alternativ for toastmaster-skjemaet
  medan det ikkje er aktivert.
- **Toastmaster-kontaktskjema** — `#toastmaster-form`, sjå eige avsnitt
  over.
- **RSVP-skjema** — Google Form i `#svar`, sjå eige avsnitt over.
  RSVP-frist er **15. januar 2027** (skjemaet seier 15.01.27).
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
